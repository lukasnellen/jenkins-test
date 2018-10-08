/* Requires the Docker Pipeline plugin */
/*
node('docker') {
    checkout scm
    stage('Build') {
        docker.image('python:3.5.1').inside {
            sh 'python --version'
        }
    }
}
*/

pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
    }
}
