pipeline {
    agent any
    stages {
        stage('Image Building') {
            steps {
                echo 'Removing old image and container'

                sh '''
                    docker rm --force nodehelloworld-container
                    docker rmi --force nodehelloworld
                    
                    docker build -t nodehelloworld .
                    
                    '''
                
                
            }
        }
        stage('Container Deployment') {
            steps {
                echo 'creating new container from image'
                
                sh '''docker run -d -p 3030:3030 --name nodehelloworld-container nodehelloworld'''
                
                
            }
        }
    }
}
