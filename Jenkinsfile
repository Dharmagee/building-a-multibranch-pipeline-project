pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                 npm install
            }
        }
        stage('Test') {
            steps {
                sudo './jenkins/scripts/test.sh'
            }
        }
    }
}