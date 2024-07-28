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
                @echo off

				sh "%CD%\jenkins\scripts\test.sh"
            }
        }
    }
}