pipeline {
    agent any
    stages {
        stage('Create EC2') {
            steps {
                sh "aws cloudformation create-stack --stack-name s3bucket --template-body file://creates3bucket.json --region 'us-east-2'"
            }
        }
    }
}
