pipeline {
  agent any
  stages {
    stage('Teste') {
      steps {
        echo 'Hello'
      }
    }
    stage('Shell') {
      steps {
        parallel(
          "Shell": {
            sh '/usr/games/fortune'
            sh 'date --rfc-2822'
            
          },
          "Sleep": {
            sleep 10
            
          }
        )
      }
    }
    stage('End') {
      steps {
        echo 'Acabou'
      }
    }
  }
}