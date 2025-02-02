pipeline {
    agent any
    
    stages {
        stage('transfer ZIP from serve 1 to server 2 using rsync') {
            steps {
                script {
                    sh '''rsync -avz -e "ssh -i /home/ubuntu/.ssh -o StrictHostKeyChecking=no" 3.91.222.233:/home/ubuntu/copy.zip 3.84.251.255:/home/ubuntu/rsync'''
                }
            }
        }
    }
}
