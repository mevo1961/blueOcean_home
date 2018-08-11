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
        stage('Step_3') {
          steps {
            mail(subject: 'Testmail', body: 'Hallo Meinolf, das ist eine Testmail von Jenkins / blueOcean', to: 'mevo1961@gmail.com', from: 'jenkins@nokia.com')
          }
        }
      }
    }
  }
}