pipeline {
    agent any
    stages {
        stage('Clone Repo') {
          steps {
            sh 'rm -rf dockertest1'
            sh 'git clone https://github.com/mavrick202/dockertest1.git'
            }
    }
 stage('Submit production Stack') {
            steps {
            sh "aws cloudformation create-stack --stack-name s31bucket --template-body file://simples3bucket.json --region 'ap-southeast-2'"
              }
             }
            }
            }
