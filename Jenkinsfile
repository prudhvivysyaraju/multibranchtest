pipeline {
    agent any
    stages {
        stage('Submit Stack') {
            steps {
            sh "aws cloudformation create-stack --stack-name s3bucket --template-body file://simples3cft.json --region 'ap-southeast-2'"
              }
             }
            }
            }
