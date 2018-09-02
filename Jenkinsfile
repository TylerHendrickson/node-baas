pipeline {
    agent {
        docker {
            image 'node:8'
            // args '-v $PWD:/usr/src/app'
        }
    }

    environment { HOME="." }

    stages {
        stage('Source') {
            checkout scm
        }

        stage('Install') {
            steps {
                sh 'pwd'
                sh 'npm install --verbose'
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
