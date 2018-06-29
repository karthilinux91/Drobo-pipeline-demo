pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        bat 'hostname'
      }
    }
    stage('test') {
      steps {
        bat(script: 'hostnamegj', returnStatus: true, returnStdout: true)
      }
    }
    stage('deploy') {
      steps {
        bat 'hostname'
      }
    }
  }
}