pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }
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
