pipeline {
  agent any
  stages {
    stage('Stage_1') {
      parallel {
        stage('Step_1') {
          steps {
            sh './scripts/helloWorld.py'
            sh 'date'
          }
        }
        stage('Step_2') {
          steps {
            echo 'Hello!'
            sh 'date'
          }
        }
        stage('Step_3') {
          steps {
            mail(subject: 'Testmail', body: 'Hallo Meinolf, das ist eine Testmail von Jenkins / blueOcean', to: 'meinolf.vogt@gmx.de', from: 'mevo1961@gmail.com')
            sh 'date'
          }
        }
        stage('Step_4') {
          steps {
            sleep 30
            sh 'date'
          }
        }
      }
    }
    stage('Stage_2') {
      steps {
        sh 'date'
      }
    }
  }
}