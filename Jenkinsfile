pipeline {
    agent any

    environment {
        IMAGE_NAME = 'devops-profile'
        CONTAINER_NAME = 'devops-profile-container'
    }

    stages {
        stage('Clone Repository') {
            steps {
                echo 'Cloning repository...'
                
                    git branch: 'main',
                       url : 'https://github.com/samidha1-1/devops-profile.git'
                
            }
        }

        stage('Build docker image') {
            steps {
                echo 'Building docker image...'
                sh '''
                docker build -t $IMAGE_NAME .
                '''
            }
        }

        stage('Stop old container') {
            steps {
                echo 'Stopping old docker container...'
                sh '''
                docker stop $CONTAINER_NAME || true
                docker rm $CONTAINER_NAME || true
                '''
            }
        }

        stage('Run new container') {
            steps {
                echo 'Running docker container...'
                sh '''
                docker run -d --name $CONTAINER_NAME -p 80:80 $IMAGE_NAME
                '''
            }
        }
    }
}
