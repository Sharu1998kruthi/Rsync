pipeline {
    agent any
    
    stages {
        stage('transfer ZIP from serve 1 to server 2 using rsync') {
            steps {
                script {
                    sh "scp -i /C/Users/THIS PC/.ssh/id_rsa -o StrictHostKeyChecking=no ‪C:/Users/THIS PC/Desktop/SS Training/Vagrantfile.rar Ubuntu@3.91.222.233:/home/ubuntu/scp"
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
