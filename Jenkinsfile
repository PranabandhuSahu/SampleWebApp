pipeline {
    agent any
    tools {
         git 'Default'
         jdk 'JAVA_HOME'
         maven 'M2_HOME'
        }
    stages {
        
        stage('Code Checkout') {
            steps {
                echo "code checkout"
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/PranabandhuSahu/SampleWebApp.git']]])
            }
        }

        stage('Build Code') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Deploy - Production') {
            steps {
               echo "deploy to server"
            }
        }
    }
}
