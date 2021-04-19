pipeline {
    agent {
        docker {
            image 'node:lts-buster-slim'
            args '-p 3000:3000'
        }
    }
    environment { 
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Here is where we execute tests"'
            }
        }
        stage('Package') { 
            steps {
                sh 'echo "I am packaging :)"' 
            }
        }
    }
}