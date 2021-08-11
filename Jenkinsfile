pipeline {
    agent docker { 
        image docker:latest
        args -v /var/run/docker.sock:/var/run/docker.sock
    }
    stages {
        stage('Checkout') {
            steps {
                echo "krok przed"
                sh '''#!/usr/bin/env bash
                    echo "pierwsza linia"
                    apt update
                    apt install -y docker.io
                    docker ps -a
                    echo $?
                    echo "druga linia"'''
            }
        }
    }
}
