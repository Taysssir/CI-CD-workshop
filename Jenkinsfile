pipeline {
    /*agent {
        docker {
            //image 'node:6-alpine'
            image 'node:14.17.6'
            args '-p 3000:3000'
        }
    }*/
    agent any
    stages {
        stage('Deploy') {
            steps {
                dir("the-example-app.nodejs") {
                    sh "pwd"
                    sh 'npm start'
                    }
            }
        }
    }
}
