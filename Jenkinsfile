echo 'test hier'
export PATH=/usr/local/bin:$PATH

pipeline {
    stages {
        stage('Build') { 
            steps {
                sh 'npm install && npm run test' 
            }
        }
    }
}
