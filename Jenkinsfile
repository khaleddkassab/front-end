pipeline {
    agent any

    stages {
        stage('Run') {
            steps {
                // Pull and run Docker container for frontend from Docker Hub
                sh 'docker run -p 3000:3000 khaleddkassab/clinic:FRONT-ENDDDD'
                // Replace 'khaleddkassab/clinic:FRONT-ENDDDD' with your actual Docker Hub image name and tag
            }
        }
    }
}
