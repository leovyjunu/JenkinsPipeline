pipeline {
    agent any
    stages {
        stage('CreateS3Bucket') {
            steps {
                sh "aws cloudformation create-stack --stack-name LeoJenkinsS3bucketCF --template-body file://creates3bucket.json --region 'us-east-2'"
            }
        } 
    }
}
