pipeline {
    agent any
    stages {
        stage('Compile') {
            steps {
                bat 'javac Hello.java'
            }
        }
        stage('Run') {
            steps {
                bat 'java Hello'
            }
        }
    }
    post {
        success { echo 'BUILD SUCCESSFUL' }
        failure { echo 'BUILD FAILED' }
    }
}
