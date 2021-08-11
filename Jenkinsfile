pipeline {
  
  agent {
    docker { image 'ubuntu'}
      
  
  stages {
    
    stage("test") {
      
      steps {
        bash '''
          #!/bin/bash
          sudo docker ps -a
          '''
      }
    }
  }
