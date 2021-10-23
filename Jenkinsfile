pipeline {
    agent any
    stages {
        
        stage('Code Checkout') {
            steps {
                echo "code checkout"
            }
        }

        stage('Build Code') {
            steps {
                echo "Building Maven Job"
            }
        }

        stage('Deploy - Production') {
            steps {
               echo "deploy to server"
            }
        }
    }
}
