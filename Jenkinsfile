pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh '''#!/usr/bin/env bash
                    echo "krok przed"'''
                sh '''#!/usr/bin/env bash
                    echo "pierwsza linia"
                    sudo docker ps -a
                    echo $?
                    echo "druga linia"'''
            }
        }
    }
}
