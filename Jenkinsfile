pipeline {
    agent any
    tools {nodejs "node"}

    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        stage('Build') {
            steps {
                bat 'npm run Build'
            }
        }
        stage('Test') {
            steps {
                bat 'npm run test -- --coverage'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}