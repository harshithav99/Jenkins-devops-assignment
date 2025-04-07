pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo '🔧 Building the application...'
            }
        }

        stage('Test') {
            steps {
                echo '✅ Running tests...'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo '🚀 Deploying to Staging...'
                bat '''
        	mkdir staging
        	copy index.html staging\\
		'''
            }
        }

        stage('Deploy to Production') {
            steps {
                echo '🚀 Deploying to Production...'
                bat '''
        	mkdir production
        	copy index.html production\\
		'''
            }
        }
    }

    post {
        success {
            echo '🎉 Deployment completed successfully.'
        }
        failure {
            echo '❌ Deployment failed.'
        }
    }
}
