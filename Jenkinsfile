pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Clonning the repository'
                // e.g., sh 'mvn clean install' or 'npm build'
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
                sh 'pytest --maxfail=1 --disable-warning -q'
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

