pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/<vivekthombre93-del>/<jenkinsfile>.git'
            }
        }

        stage('Install') {
            steps {
                sh 'python3 -m venv ven'
                sh 'source ven/bin/activate && pip install -r requirements.txt'
            }
        }

        stage('Run Python File') {
            steps {
                sh 'python3 vivek.py'
            }
        }
    }
}
