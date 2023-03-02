pipeline {
    agent any
    options {
        // Timeout counter starts AFTER agent is allocated
        timeout(time: 1, unit: 'SECONDS')
    }
    stages {
        stage('Image Building') {
            steps {
                echo 'Deleting old image'
                sh '''docker ps'''
                sh '''docker rm --force nodehelloworld '''
                echo 'Deleting old image'
                sh '''docker rmi nodehelloworld -f'''
                sh '''docker ps'''
                
                
            }
        }
        stage('Container Deployment') {
            steps {
                echo 'creating new container from image'
                //sh '''docker build -t nodehelloworld .'''
                
                //sh '''docker run -d -p 3030:3030 --name nodehelloworld nodehelloworld'''
                
                
            }
        }
    }
}
