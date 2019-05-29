pipeline {
    agent any
    tools {nodejs "node"}

    stages {
        stage('Build install') {
            steps {
                bat 'npm install'
            }
        }
        stage('Build install files') {
            steps {
                bat 'npm run build'
            }
        }
        stage('Test') {
            steps {
                bat 'npm run test -- --coverage'
            }
        }
        stage('Deploy') {
            steps {
                bat 'npm install -g serve'
                bat 'serve -s build'
                bat 'npm eject'
            }
        }
        /*stage('Eject') {
            steps {
                bat 'npm eject'
            }
        }*/
    }
}
