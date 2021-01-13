pipeline {
    agent any
    stages {
        stage('Create EC2') {
            steps {
                sh "aws ec2 run-instances --image-id ami-09558250a3419e7d0 --key-name leo-kp-ohio --instance-type t2.micro --region us-east-2 --subnet-id subnet-fa166e80 --security-group-ids sg-0f0b0eb448eeccce1 --count 1"
            }
        }
    }
}
