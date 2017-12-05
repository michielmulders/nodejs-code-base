pipeline {
    agent any
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
