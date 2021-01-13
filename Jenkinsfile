pipeline {
    agent any
    stages {
        stage('CreateS3Bucket') {
            steps {
                sh "aws cloudformation create-stack --stack-name LeoJenkinsS3bucketCF --template-body file://creates3bucket.json --region 'us-east-2'"
            }
        }
        stage('CreateEC2instance') {
            steps {
                sh "aws ec2 run-instances --image-id ami-09558250a3419e7d0 --key-name leo-kp-ohio --instance-type t2.micro --region us-east-2 --subnet-id subnet-fa166e80 --security-group-ids sg-0f0b0eb448eeccce1 --count 1"
    }
}
