pipeline {
    agent { label 'win11' }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    credentialsId: 'ssh-jenkins',
                    url: 'https://github.com/DobleADev/qa-practice-minimal-factory-game.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy step...'
            }
        }
    }
}