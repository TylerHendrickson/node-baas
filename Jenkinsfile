pipeline {
    agent {
        docker {
            image 'node:8-stretch'
        }
    }

    environment { HOME="." }

    stages {
        stage('Pre-Install') {
            steps {
                sh 'npm i -g npm'
            }
        }

        stage('Install') {
            steps {
                sh 'pwd'
                // sh 'rm -rf ./node_modules' TODO: Need this?
                sh 'npm ci --verbose'
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
