pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                script {
                    echo "Branch: ${env.BRANCH_NAME}"
                }
                git url: 'https://github.com/teodoracioca/test-multibranch-repo.git', credentialsId: 'github_credential'
            }
        }
        stage('Build') {
            steps {
                echo "Building the project"
            }
        }
        stage('Test') {
            steps {
                echo "Running tests"
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying the project"
            }
        }
    }
}
