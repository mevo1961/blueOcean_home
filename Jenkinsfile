pipeline {
  agent any
  stages {
    stage('Steps') {
      parallel {
        stage('Step_1') {
          steps {
            sh './scripts/helloWorld.py'
          }
        }
        stage('Step_2') {
          steps {
            echo 'Hello!'
          }
        }
      }
    }
  }
}