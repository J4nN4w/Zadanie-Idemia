pipeline {
    agent {docker {
        image 'docker:latest'
        args '-v /var/run/docker.sock:/var/run/docker.sock'
    }}
    stages {
        stage('Checkout') {
            steps {
                sh '''
                    docker ps -a'''
            }
        }
    }
}
