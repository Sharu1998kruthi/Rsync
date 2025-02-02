pipeline {
    agent any

    environment {
            SSH_PRIVATE_KEY_PATH = 'C:/Users/THIS PC/.ssh'
    }
    stages {
        stage('transfer ZIP from serve 1 to server 2 using rsync') {
            steps {
                script {
                   
                }
            }
        }
    }
    post {
        success {
            echo 'file copy successfull'
        }
        failure {
            echo 'file copy failed'
        }
    }
}
