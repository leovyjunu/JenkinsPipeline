pipeline {
    agent any
    stages {
        stage('CreateS3Bucket') {
            steps {
                sh "aws cloudformation create-stack --stack-name LeoThisCFisforS3Bucket --template-body file://creates3bucket.yaml --region 'us-east-2'"
            }
        } 
    }
}
