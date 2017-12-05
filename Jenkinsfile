pipeline {
    stages {
        stage('Build') { 
            steps {
                export PATH=/usr/local/bin:$PATH
                echo "Build Stage"
                sh 'npm install'
                sh 'npm run test' 
            }
        }
    }
}
