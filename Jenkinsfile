pipeline {
    agent {
        docker {
            image 'node:14'
            args '-v /var/run/docker.sock:/var/run/docker.sock'
        }
    }
    stages {
        stage('Build') {
            steps {
                script {
                    sh 'npm install'
                }
            }
        }
        stage('Test') {
            steps {
                script {
                    sh 'npm test'
                }
            }
        }
        stage('Deploy') {
            steps {
                script {
                    sh 'echo "Deploying to production"'
                }
            }
        }
    }
}
