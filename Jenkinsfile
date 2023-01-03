pipeline {
    agent {
        node {
            label 'nodejs'
        }
    }
    stages {
        stage('Checkout') {
            steps {
                sh 'git clone https://github.com/wachira90/test-build-reactjs.git'
            }
        }
        stage('Install dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
    }
}
