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
    stage('FINAL') {
      steps {
        build(job: 'job1', propagate: true, quietPeriod: -2)
      }
    }
  }
}