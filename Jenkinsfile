pipeline {
    agent any
    stages {
        stage('Clone Repo') {
          steps {
            sh 'whoami'
            sh 'git clone https://github.com/prudhvivysyaraju/multibranchtest.git'
            }
    }
 stage('Submit production Stack') {
            steps {
            sh 'whoami'
            sh "aws cloudformation create-stack --stack-name s3bucket --template-body file://simplests3bucket.json --region 'ap-southeast-2'"
              }
             }
            }
            }
