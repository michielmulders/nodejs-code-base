pipeline {
    agent any
    docker.image('node:6-alpine').withRun('-p 3000:3000') {
            echo "docker node"
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
