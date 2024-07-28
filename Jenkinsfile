pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Build Completed'
            }
        }
        stage('Test') {
            steps {
                 echo 'Test Completed'
            }
        }
        stage('Deliver for development') {
            when {
                branch 'development' 
            }
            steps {
                 echo 'Dev Completed'
            }
        }
        stage('Deploy for production') {
            when {
                branch 'production'  
            }
            steps {
                 echo 'Prod Completed'
            }
        }
    }
}