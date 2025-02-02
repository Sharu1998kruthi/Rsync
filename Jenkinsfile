pipeline {
    agent any

    environment {
            SSH_PRIVATE_KEY_PATH = ''/c/Users/THIS\ PC/.ssh/id_rsa'
    }
    stages {
        stage('transfer ZIP from serve 1 to server 2 using rsync') {
            steps {
                script {
                    sh """scp -i {SSH_PRIVATE_KEY_PATH} -o StrictHostKeyChecking=no ‪C:/Users/THIS PC/Desktop/SS Training/Vagrantfile.rar Ubuntu@3.91.222.233:/home/ubuntu/scp"""
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
