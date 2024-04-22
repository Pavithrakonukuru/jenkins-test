Pipeline {
    agent any
    stages {
        stage ('git checkout') {
            steps {
                sh "export AWS_DEFAULT_REGION=ap-south-1"
                sh "aws cloudformation create-stack --stack-name iamuser --template-body file://iamuser.json --region 'ap-south-1'"
            }
        }
    }
}