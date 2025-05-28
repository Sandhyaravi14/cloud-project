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
                bat '"C:\\Users\\sandh\\AppData\\Local\\Programs\\Python\\Python313\\Scripts\\pip.exe" install flask'
            }
        }

        stage('Run Flask App') {
    steps {
        bat 'start "" "C:\\Users\\sandh\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" app.py'
    }
}
    }
}