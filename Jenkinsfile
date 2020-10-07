pipeline {
    agent any
    stages {
        stage('Clone Repo') {
          steps {
            sh 'rm -rf dockertest1'
            sh 'git clone https://github.com/mavrick202/dockertest1.git'
            }
    }
    stage('Submit Development Stack') {
            steps {
            sh "aws cloudformation create-stack --stack-name s3bucket --template-body file://simplests3bucket.json --region 'ap-southeast-2'"
              }
             }
            }
            }
