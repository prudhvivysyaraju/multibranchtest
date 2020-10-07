pipeline {
    agent any
    stages {
        stage('Clone Repo') {
          steps {
            sh 'git clone https://github.com/prudhvivysyaraju/multibranchtest.git'
            }
    }
    stage('Submit Development Stack') {
            steps {
            sh "pip3 install awscli"
            sh "aws cloudformation create-stack --stack-name s3bucket --template-body file://simplests3bucket.json --region 'ap-southeast-2'"
              }
             }
            }
            }
