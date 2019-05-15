pipeline {
  agent any
  stages {
    stage('Parallel 1') {
      parallel {
        stage('krok 1') {
          steps {
            echo 'Hello 1.1'
            echo 'Hello 1.2'
          }
        }
        stage('Parallel 2') {
          steps {
            timeout(time: 20)
            echo 'Stage 2'
          }
        }
      }
    }
    stage('Opoznienie') {
      steps {
        sleep 1
      }
    }
  }
}