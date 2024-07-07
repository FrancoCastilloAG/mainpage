pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout del repositorio Git
                checkout scm
            }
        }
        stage('Build') {
            steps {
                // Construcción de la aplicación
                sh 'npm install'
            }
        }
        stage('Deploy') {
            steps {
                // Despliegue de la aplicación
                sh 'npm start &'
            }
        }
    }
}
