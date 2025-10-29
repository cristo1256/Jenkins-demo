pipeline {
    agent {
        docker { image 'python:3.10' }
    }
    stages {
        stage('Build') {
            steps {
                echo 'Preparando entorno...'
            }
        }
        stage('Test') {
            steps {
                sh 'pip install pytest'
                sh 'pytest --maxfail=1 --disable-warnings -q'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Desplegando aplicación (simulado)...'
            }
        }
    }
}
