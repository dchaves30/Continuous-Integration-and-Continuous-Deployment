pipeline {
  agent any
  stages {
    stage('Build') {
      agent any
      steps {
        sh 'tidy -q -e *.html'
      }
    }
    stage('Upload to AWS') {
      steps {
        s3Upload(bucket: 'udacity-project-01', pathStyleAccessEnabled: true, payloadSigningEnabled: true, file: 'index.html', path: 'aws:s3:::udacity-project-01/*')
      }
    }
  }
}