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
                sh 'python3 --version'
                sh 'python3 Ayush.py'
                // e.g., sh 'mvn clean install' or 'npm build'
            }
        }
        stage('Test') {
            steps {
                sh 'apt install python3.10-venv'
                sh 'python3 -m venv venv'
                sh '. venv/bin/activate && pip install pytest'
                sh '. venv/bin/activate && pytest --maxfail=1 --disable-warnings -q'
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
