pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        sh 'tidy -q -e *.html'
      }
    }
  }
}