pipeline {
    agent {
        docker {
            image 'node:8-stretch'
            // args '-v $PWD:/usr/src/app'
        }
    }

    environment { HOME="." }

    stages {
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
