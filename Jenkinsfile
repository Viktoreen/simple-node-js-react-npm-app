pipeline {
    agent any
    tools {nodejs "node"}

    stages {
        stage('Build') {
            steps {

                bat 'npm install'

            }
        }
        stage('Test') {
            steps {
                echo 'Testing and testing again..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}