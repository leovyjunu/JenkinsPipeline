pipeline {
    agent any
    stages {
        stage('CreateS3Bucket') {
            steps {
                sh "aws cloudformation create-stack --stack-name leos3bucket2 --template-body file://creates3bucket.json --region 'us-east-2'"
            }
        }
    }
}
