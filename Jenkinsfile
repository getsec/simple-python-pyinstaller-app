pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo $(pwd)
                pip install -r requirements.txt
            }
        }
        stage('Test') {
            steps {
                echo $(pwd)
                flake8 scripts/
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
