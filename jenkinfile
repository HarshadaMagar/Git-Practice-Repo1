pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                echo "Checking out code from GitHub..."
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "Starting Build Process..."
                // Add your build command here
                echo "Build Completed!"
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying Application..."
                // Add deploy logic here, e.g., copying files, running scripts
                echo "Deployment Successful!"
            }
        }
    }

    post {
        success {
            echo "✅ Pipeline executed successfully!"
        }
        failure {
            echo "❌ Pipeline failed!"
        }
    }
}
