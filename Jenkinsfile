pipeline {
    agent any
    
    stages {
        stage('transfer ZIP from serve 1 to server 2 using rsync') {
            steps {
                script {
                    sh '''rsync -avz copy.zip ubuntu@3.84.251.255:/home/ubuntu'''
                }
            }
        }
    }
}
