pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                dir('C:/ProgramData/Jenkins/.jenkins/workspace/jdg/') {
                    docker.run('node:14', '-v /var/run/docker.sock:/var/run/docker.sock')
                }
            }
        }
    }
}








// pipeline {
//     agent {
//         docker {
//             image 'node:14'
//             args '-v /var/run/docker.sock:/var/run/docker.sock'
//         }
//     }
//     stages {
//         stage('Build') {
//             steps {
//                 script {
//                     bat 'npm install'
//                 }
//             }
//         }
//         stage('Test') {
//             steps {
//                 script {
//                     bat 'npm test'
//                 }
//             }
//         }
//         stage('Deploy') {
//             steps {
//                 script {
//                     bat 'echo "Deploying to production"'
//                 }
//             }
//         }
//     }
// }
