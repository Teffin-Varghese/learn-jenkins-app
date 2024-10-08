pipeline {
    agent any

    stages {
        stage('Hello World') {
            steps {
                echo 'Hello, This is another test for jenkins on git'
                sh 'df -h'
                sh 'whoami'
                sh 'pwd'
            }
        }
    }

    post {
        always {
            echo 'Pipeline execution completed!'
        }
    }
}
