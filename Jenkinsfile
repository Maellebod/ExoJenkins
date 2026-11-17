pipeline {
    agent any

    stages {
        stage('Build et Run Docker') {
            steps {
                sh 'docker compose up -d --build'
            }
        }

        stage('Verification') {
            steps {
                sh 'docker compose ps'
            }
        }
    }
}