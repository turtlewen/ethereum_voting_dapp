pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        build 'build html'
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sleep 1
          }
        }
        stage('') {
          steps {
            sleep(unit: 'SECONDS', time: 1)
          }
        }
      }
    }
  }
}