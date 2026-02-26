pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning repository...'
                git 'https://github.com/clause18/jenkins-demo.git'
            }
        }
        
        stage('Build') {
            steps {
                echo 'Building the application...'
                // For Python app
                bat 'echo Building Python app...'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Testing the application...'
                // Run your test
                bat 'python --version'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Simulate deployment
                bat 'echo Application deployed successfully!'
            }
        }
    }
    
    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
