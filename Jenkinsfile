pipeline {
    agent { label 'win11' }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

	stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy step...'
            }
        }
    }
}