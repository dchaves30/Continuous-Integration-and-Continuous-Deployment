pipeline {
  agent any
  stages {
    stage('Lint HTML') {
      steps {
        withAWS(region: 'us-west-2', credentials: 'dchaves') {
          sh 'tidy -q -e *.html'
        }

      }
    }
    stage('Upload to AWS') {
      steps {
        s3Upload(bucket: 'udacity-project04', pathStyleAccessEnabled: true, payloadSigningEnabled: true)
      }
    }
  }
}