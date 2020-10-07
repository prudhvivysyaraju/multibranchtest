pipeline {
    agent any
    stages {
        stage('Clone Repo') {
          steps {
            sh 'rm -rf dockertest1'
            sh 'git clone https://github.com/prudhvivysyaraju/multibranchtest.git'
            }
    }
 stage('Submit production Stack') {
            steps {
            sh "aws cloudformation create-stack --stack-name s3bucket --template-body file://simples3bucket.json --region 'ap-southeast-2'"
              }
             }
            }
            }
