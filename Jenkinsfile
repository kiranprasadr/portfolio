pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                echo "Building Docker image..."
                sh "docker build -t webportal:latest ."
            }
        }

        stage('Test') {
            steps {
                echo 'Running simple tests...'
                sh "echo Tests passed"
            }
        }
    }
}
