node {
    try {
        stage('Checkout') {
            echo 'Checking out code...'
            git 'https://github.com/clause18/jenkins-demo.git'
        }
        
        stage('Build') {
            echo 'Building...'
            bat 'echo Build stage completed'
        }
        
        stage('Test') {
            echo 'Testing...'
            bat 'python hello.py'
        }
        
        stage('Deploy') {
            echo 'Deploying...'
            bat 'echo Application deployed'
        }
        
        echo 'Pipeline completed successfully!'
    }
    catch (Exception e) {
        echo "Pipeline failed: ${e.message}"
        throw e
    }
}
