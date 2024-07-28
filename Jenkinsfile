pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                bat run 'npm install'
            }
        }
        stage('Test') {
            steps {
                sudo './jenkins/scripts/test.sh'
            }
        }
    }
}