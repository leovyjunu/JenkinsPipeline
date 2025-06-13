pipeline {
    agent any
    stages {
        stage('CreateS3BucketviaCF') {
            steps {
                sh "aws cloudformation create-stack --stack-name LeoS3Bucket --template-body file://creates3bucket.yaml --region 'us-east-2'"
            }
        } 
    }
}
## test updated
