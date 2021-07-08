pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello build stage world!"'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Hello test stage world!"'
            }
        }
        stage('Deliver for development') {
            when {
                branch 'development'
            }
            steps {
                sh 'echo "in the development branch"'
            }
        }
        stage('Deploy for production') {
            when {
                branch 'production'
            }
            steps {
                sh 'echo "in the production branch"'
            }
        }
    }
}
