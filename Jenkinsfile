pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/acpx1337x2/jenkins-node.git'
            }
        }

        stage('Install') {
            steps {
                bat 'npm install'
            }
        }

        stage('Run App') {
            steps {
                bat 'node app.js'
            }
        }

        stage('Test') {
            steps {
                bat 'npm test'
            }
        }

    }
}