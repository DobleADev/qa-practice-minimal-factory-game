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


    
    post {
            success {
                publishChecks name: 'continuous-integration/jenkins', conclusion: 'SUCCESS'
            }
            failure {
                publishChecks name: 'continuous-integration/jenkins', conclusion: 'FAILURE'
            }
        }


}