pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                // e.g., sh 'mvn clean install' or 'npm build'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
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

