pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build stage - nothing to compile'
            }
        }

        stage('Test') {
            steps {
                echo 'Test stage - placeholder for future tests'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy stage - serving static HTML'
            }
        }
    }
post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed! Please check the logs.'
        }
        always {
            echo 'Pipeline finished running (success or fail).'
        }
    }
}

