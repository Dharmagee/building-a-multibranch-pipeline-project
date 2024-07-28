pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Build completed'
            }
        }
        stage('Test') {
            steps {
               echo 'Test Completed'
            }
        }
    }
	
	  stage('Deliver for development') {
            when {
                branch 'development'
            }
            steps {
                echo 'Development Deployment done'
            }
        }
		
		 stage('Deploy for production') {
            when {
                branch 'production'
            }
            steps {
                echo 'Production Deployment done'
            }
        }
}