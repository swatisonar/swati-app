pipeline {
    agent any

    environment {
        // Define environment variables here
        MY_VAR = 'value'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Example build command
                sh './build.sh'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example test command
                sh './run_tests.sh'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Example deploy command
                sh './deploy.sh'
            }
        }
    }

    post {
        success {
            echo 'The pipeline has succeeded.'
        }
        failure {
            echo 'The pipeline has failed.'
        }
        always {
            echo 'Cleaning up resources...'
        }
    }
}
