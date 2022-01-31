pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                echo 'Probando servdor SFTP'
                sh 'wget sftp://foo:pass@www.cristojaviergmsystem.com:9922/foo-home'
            }
        }
        stage('Build') {
            steps {
                echo 'Building application...'
                sh 'sudo docker-compose up -d'
            }
        }
    }
}