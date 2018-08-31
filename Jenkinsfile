pipeline {
    agent {
        docker {
            image 'node:9'
            args '-v $PWD:/usr/src/app'
        }
    }

    tools {nodejs "node"}

    stages {
        stage('Install') {
            steps {
                sh 'npm i -g npm'
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
