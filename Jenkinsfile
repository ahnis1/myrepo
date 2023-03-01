
pipeline {
    agent any
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Cleaning stage') {
            steps {
                echo 'This stage is removing old containers and images'
            }
        }
    }
    
    stages {
        stage('Buidling stage') {
            steps {
                echo 'This is building the docker image from Dockerfile and creating a new image from latest code'
            }
        }
    }
    
    stages {
        stage('Testing') {
            steps {
                echo 'Automation scripts can be executed here'
            }
        }
    }
}
