pipeline {
    agent {
        docker {
            image 'node:8-stretch'
        }
    }

    environment { HOME="." }

    stages {
        stage('Install') {
            steps {
                sh 'npm install'
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
