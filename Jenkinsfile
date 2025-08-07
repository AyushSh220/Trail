pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning the repository'
                // e.g., sh 'git clone <repo_url>'
            }
        }
        stage('Build') {
            steps {
                sh 'python --version'
                sh 'python3 Ayush.py'
                // e.g., sh 'mvn clean install' or 'npm build'
            }
        }
        stage('Test') {
            steps {
                sh 'pytest --maxfail=1 --disable-warnings -q'
                // e.g., sh 'mvn test' or 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Your deployment commands here
            }
        }
    }
}
