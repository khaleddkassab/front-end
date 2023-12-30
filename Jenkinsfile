pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Check out code from Git
                git branch: 'main', url: 'https://github.com/khaleddkassab/front-end.git'
                
                // Build Docker image for frontend
                sh 'docker build -t docker-compose.yaml .'
                // Replace 'frontend-image' with the name you want for your Docker image
            }
        }

        stage('Run') {
            steps {
                // Run Docker container for frontend
                sh 'docker run -p 3000:3000 docker-compose.yaml'
                // Replace 'frontend-image' with the name of your Docker image
            }
        }
    }
}
