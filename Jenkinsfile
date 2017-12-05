pipeline {
    agent {
        docker.image('node:6-alpine') {
            echo "docker node"
        }
    }
    stages {
        stage('Build') {
            steps {
                echo "Build Stage"
                sh 'npm install'
                sh 'npm run test'
            }
        }
    }
}
