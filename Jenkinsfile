pipeline {
    agent any

    stages {
        stage('build') {
            agent {
                docker {
                    image 'node:18-alpine'
                    reuseNode true
                }
            }
            steps {
                echo 'Hello, This is test#2 for jenkins on git'
                sh 'df -h'
                sh 'whoami'
                sh 'pwd'
                sh 'ls -la'
                sh 'node --version'
                sh 'npm --version'
                sh 'npm ci'
                sh 'npm run build'
                sh 'ls -la'
            }
        }
    }

    post {
        always {
            echo 'Pipeline execution completed!'
        }
    }
}
