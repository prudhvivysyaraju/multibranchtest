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
            sh "cd /usr/local/bin/"
            sh "ls"
            sh "/usr/local/bin/aws cloudformation create-stack --stack-name s3bucket --template-body file://simples3bucket.json --region 'ap-southeast-2'"
              }
             }
            }
            }
