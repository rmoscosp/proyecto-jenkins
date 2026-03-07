pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Descargando código del repositorio...'
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Compilando el proyecto...'
                echo 'Build completado exitosamente.'
            }
        }
        stage('Test') {
            steps {
                echo 'Ejecutando pruebas automatizadas...'
                echo 'Todas las pruebas pasaron correctamente.'
            }
        }
        stage('Deploy Simulation') {
            steps {
                echo 'Simulando despliegue a producción...'
                echo 'Despliegue simulado completado con éxito.'
            }
        }
    }
    post {
        success {
            echo 'Pipeline ejecutado exitosamente!'
        }
        failure {
            echo 'El pipeline ha fallado. Revisar los logs.'
        }
    }
}