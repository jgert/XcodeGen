pipeline {
  agent any
  stages {
    stage('Stage 1') {
      parallel {
        stage('Stage 1') {
          steps {
            sh 'echo "Test"'
            echo 'Hello 2'
          }
        }
        stage('Stage 2') {
          steps {
            timeout(time: 20)
            echo 'Stage 2'
          }
        }
      }
    }
    stage('error') {
      steps {
        sleep 1
      }
    }
  }
}