
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/ayu1907/jenkinsdemo'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Building Python application"'
                sh 'ls -l'
            }
        }

        stage('Test') {
            steps {
                sh 'python3 --version'
                sh 'python3 hello.py'
            }
        }

        stage('Docker Deploy') {
            steps {
                sh 'echo "Docker deployment stage"'
            }
        }
    }
}
