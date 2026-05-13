cat > Jenkinsfile << 'EOF'
pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/acpx1337x2/jenkins-node.git/'
            }
        }

        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run App') {
            steps {
                sh 'node app.js'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}
EOF