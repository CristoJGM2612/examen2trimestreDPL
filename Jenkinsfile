pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                echo 'Despliegue de la aplicación'
                sh 'docker-compose up -d'
                
            }
        }
        stage('Test Integration') {
            steps {
                echo 'Comprobación del servidro SFTP'
                sh 'wget sftp://foo:pass@www.cristojaviergmsystem.com:9922/foo-home'
            }
        }
    }
}