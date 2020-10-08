pipeline {
    agent any
    stages {
        stage('Clone Repo') {
          steps {
            sh 'git clone https://github.com/prudhvivysyaraju/multibranchtest.git'
            }
    }
    stages {
        stage('syntax-check') {
          steps {
            sh 'cfn-lint ./*.json'
            }
    }
        stages {
        stage('code push to s3_bucket') {
          steps {
            sh "/usr/local/bin/aws s3 cp simples3bucket.json s3://aws-logs-786678469955-ap-southeast-2/simples3bucket.json"
            }
    }
    stage('Submit Development Stack') {
            steps {
            sh 'cd /usr/local/bin/'
            sh 'ls'
            sh "/usr/local/bin/aws cloudformation create-stack --stack-name s3bucket --template-body file://simples3bucket.json --region 'ap-southeast-2'"
              }
             }
            }
            }
    }
}
