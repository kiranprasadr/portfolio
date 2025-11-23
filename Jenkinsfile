pipeline {
    agent any

    stages {
        stage('Start') {
            steps {
                echo 'Pipeline started'
            }
        }

        stage('docker build') {
            steps {
                echo 'Hello from Jenkins'
                sh 'docker build -t portfolio:latest .'

            }
        }

        stage('End') {
            steps {
                echo 'Pipeline finished'
            }
        }
    }
}
