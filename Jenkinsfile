pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        sh 'ls -lah'
        sh 'echo \'Hello World\''
        sh '''echo \'"This 
         is a multiline"\''''
      }
    }
  }
}