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
        stage('Cloning') {
            steps {
                sh "git clone https://github.com/contentful/the-example-app.nodejs.git"
            }
        }
        stage('Dependencies installation') {
            steps {
                sh 'npm install'
            }
        }
        stage('Deploy') {
            steps {
                sh 'npm start'
            }
        }
    }
}
