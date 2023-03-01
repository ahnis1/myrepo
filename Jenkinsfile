pipeline {
    agent any
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Example') {
            steps {
                echo 'Deleting old container and image'
                sh 'whoami'
                sh 'pwd'
                
            }
        }
    }
}
