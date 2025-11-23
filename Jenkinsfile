pipeline {
    agent any

    stages {
        stage('Start') {
            steps {
                echo 'Pipeline started'
            }
        }

    stage('Docker Build') {
        steps {
            script {
                def date = sh(script: "date +%Y%m%d%H%M%S", returnStdout: true).trim()
                sh "docker build -t portfolio:${date} ."
                   }
                }
        }

        stage('End') {
            steps {
                echo 'Pipeline finished'
            }
        }
    }
}
