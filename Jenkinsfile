pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Preparando entorno...'
            }
        }
        stage('Test') {
            steps {
                // Instala pytest en el contenedor/servidor donde corre Jenkins
                sh 'pip install pytest'
                // Ejecuta las pruebas
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
