pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build Docker images') {
            steps {
                bat 'docker compose build'
            }
        }
    }
}