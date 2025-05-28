pipeline {
    agent any

    stages {
        stage('Pull from GitHub') {
            steps {
                git branch: 'main', url: 'https://github.com/Sandhyaravi14/cloud-project.git'
            }
        }

        stage('Install Flask') {
            steps {
                bat 'pip install flask'
            }
        }

        stage('Run Flask App') {
            steps {
                bat 'python app.py'
            }
        }
    }
}