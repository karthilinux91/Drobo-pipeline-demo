pipeline {
  agent any
  stages {
    stage('SQA-Blink-01') {
      steps {
        bat 'perl SQA-Blink-01.pl -drobosn=DRB124701A00083 -number=5'
      }
    }
  }
}