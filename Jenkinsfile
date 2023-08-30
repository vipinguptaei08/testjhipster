pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        
        stage('Build') {
            steps {
                sh './gradlew build'
            }
        }
        
        stage('Test') {
            steps {
                sh './gradlew test'
            }
        }
        
        stage('Deploy') {
            steps {
                sh 'echo "Deploying the app"'
                // Add deployment steps here (e.g., copying files to a server)
            }
        }
    }
}
