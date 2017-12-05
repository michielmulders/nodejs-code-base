node('NodeJS 6.12.0') {

    currentBuild.result = "SUCCESS"

    try {

       stage('Checkout'){

          checkout scm
       }

       stage('Build'){

         steps {
                sh 'export PATH=/usr/local/bin:$PATH'
                sh 'node -v'
                echo "Build Stage"
                sh 'npm install'
                sh 'npm run test' 
            }
       }
        
    }
    catch (err) {

        currentBuild.result = "FAILURE"

        throw err
    }

}
