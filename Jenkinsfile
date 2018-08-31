pipeline {
    agent any

    tools {nodejs "node"}

    stages {
        stage('Install') {
            steps {
                sh 'npm ci'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
        stage('Bundle') {
            steps {
                sh 'echo "Coming soon!"'
            }
        }
        stage('Generate AMI') {
            steps {
                sh 'echo "Nothing yet!"'
            }
        }
    }
}
