pipeline {
    agent any

    stages {
        stage('docker compose up') {
            steps {
                sh 'docker compose up'
            }
        }

        stage('docker compose down') {
            steps {
                sh 'docker compose down'
            }
        }
    }

    post {
        always {
            sh 'docker logout'
        }
    }
}
