pipeline {
    agent any
    
    stages {
        stage('transfer ZIP from local to remote server') {
            steps {
                script {
                   sh 'scp -0 StrictHostKeyChecking=no \C\Users\THIS PC\Desktop\SS Training\Vagrantfile.rar ubuntu@52.1.224.87:/home/ubuntu/scp'
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
