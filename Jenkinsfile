pipeline {
    agent any
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Image Building') {
            steps {
                echo 'Deleting old container and image'
                sh 'whoami'
                 echo 'creating new image'
                sh 'pwd'
                
                
            }
        }
        stage('Container Deployment') {
            steps {
                echo 'creating container from image'
                sh 'whoami'
                sh 'pwd'
                sh 'docker ps'
                
                
            }
        }
    }
}
