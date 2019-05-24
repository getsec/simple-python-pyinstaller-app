pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'pip install -r requirements.txt'

            }
        }
        stage('Test') {
            steps {
                sh '''
                    echo $(pwd)
                    flake8 scripts/
                '''
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
