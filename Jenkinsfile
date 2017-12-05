pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'export PATH=/usr/local/bin:$PATH'
                echo "Build Stage"
                sh 'npm install'
                sh 'npm run test' 
            }
        }
    }
}
