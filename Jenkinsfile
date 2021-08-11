pipeline {
    agent {docker {
        image 'docker:latest'
        args '-v /var/run/docker.sock:/var/run/docker.sock'
    }}
    stages {
        stage('Checkout') {
            steps {
                echo "krok przed"
                sh '''echo "pierwsza linia"
                    docker ps -a
                    echo $?
                    echo "druga linia"'''
            }
        }
    }
}
