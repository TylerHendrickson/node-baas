pipeline {
    agent any
    stages {
        stage('Install') {
            steps {
                sh 'npm i -g npm@latest'
            }
        }
        stage('Build') {
            steps {
                sh 'npm ci'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
        stage('Generate AMI') {
            steps {
                sh 'echo "This is a step"'
            }
        }
    }
}
