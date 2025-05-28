pipeline {
    agent any

    stage('Pull from GitHub') {
    steps {
        git branch: 'main', url: 'https://github.com/Sandhyaravi14/cloud-project.git'
    }
}

        stage('Install Flask') {
            steps {
                sh 'pip install flask'
            }
        }

        stage('Run Flask App') {
            steps {
                sh 'python app.py'
            }
        }
    }
}