    pipeline {
        agent any
        
        stages {
            stage('Cleaning stage') {
                steps {
                    script {
                        echo "This stage is removing old containers and images"
                        
                    }
                }
            }
            
            stage('Buidling stage') {
                steps {
                    script {
                        echo "This is building the docker image from Dockerfile and creating a new image from latest code"
                    }
                }
            }
            
            stage('Testing code') {
                steps {
                    script {
                        echo "Automation scripts can be executed here"
                    }
                }
            }
        }
    }
}
