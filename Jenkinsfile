pipeline {
    agent any
    
    environment {
        SRC_SERVER = "100.24.44.137"    //Source EC2 instance (Server 1)
        DEST_SERVER = "3.89.118.120"    //Destination EC2 instance (server 2)
        ZIP_FILE = "/home/ubuntu/Server1" //path of ZIP file on server 1
        DEST_PATH = "/home/ubuntu/Server2" //path of Destination folder in server 2
        SSH_KEY = "/home/ubuntu/.ssh"     // Private key for SSH access
    }
    stages {
        stage('transfer ZIP from serve 1 to server 2 using rsync') {
            steps {
                script {
                    sh '''rsync -avz -e "ssh -i $SSH_KEY" $SRC_SERVER $DEST_SERVER:$DEST_PATH'''
                }
            }
        }
    }
}
