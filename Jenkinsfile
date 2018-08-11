pipeline {
  agent any
  stages {
    stage('Step_1') {
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