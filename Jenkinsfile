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
        sh '/usr/games/fortune'
        sh 'date --rfc-2822'
      }
    }
  }
}