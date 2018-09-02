pipeline {
    agent any

    environment { HOME="." }

    stages {
        stage('Source') {
            steps {
                sh 'git checkout -f'
                sh 'git pull origin feature/pipeline'
            }
        }

        stage('Pre-Install') {
            agent {
                docker {
                    image 'node:8'
                    // args '-v $PWD:/usr/src/app'
                }
            }
            steps {
                // sh 'mkdir -p ~/.npm-global'
                // sh "npm config set prefix '~/.npm-global'"
                // sh 'export PATH=~/.npm-global/bin:$PATH'
                // sh '. ~/.profile'
                // sh 'rm package-lock.json'
                // sh 'npm install -g npm@latest --verbose'

                // sh 'rm package-lock.json'
                sh 'npm install'
            }
        }

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
