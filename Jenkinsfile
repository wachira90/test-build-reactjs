pipeline {
    agent {
        node {
            label 'node'
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
