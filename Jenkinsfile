pipeline {
    agent any
    environment {
        AWS_ACCESS_KEY_ID     = credentials('aws-accesskey')
        AWS_SECRET_ACCESS_KEY = credentials('aws-secretkey')
    }
    stages {
        stage('Submit Stack') {
            steps {
            sh "aws cloudformation create-stack --stack-name s3bucket --template-body file://simplests3cft.json --region 'us-east-1'"
              }
             }
            }
            }
