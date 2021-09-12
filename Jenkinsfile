pipeline {
    agent any
    stages {
        stage('Cloning') {
            steps {
                sh "git clone https://github.com/contentful/the-example-app.nodejs.git"
                sh "cd the-example-app.nodejs"
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
