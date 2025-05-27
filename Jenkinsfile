pipeline {
    agent any

    stages {
        stage('Pull from GitHub') {
            steps {
                git 'https://github.com/Sandhyaravi14/cloud-project.git'
            }
        }

        stage('Install Flask') {
            steps {
                sh 'pip install flask'
            }
        }

        stage('Run Flask App') {
            steps {
                bat 'start /b python app.py'

            }
        }
    }
}