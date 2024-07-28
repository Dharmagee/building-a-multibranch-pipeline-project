pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sudo run 'npm install'
            }
        }
        stage('Test') {
            steps {
                sudo './jenkins/scripts/test.sh'
            }
        }
    }
}