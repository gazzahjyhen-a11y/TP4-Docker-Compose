pipeline {
    agent any

    environment {
        DOCKER_HOST = 'npipe:////./pipe/dockerDesktopLinuxEngine'
    }

    stages {
        stage('Build Docker images') {
            steps {
                bat '"C:/Users/jyhen/.docker/cli-plugins/docker-compose.exe" build'
            }
        }
    }
}