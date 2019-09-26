pipeline {
  agent any
  stages {
    stage('Lint HTML') {
      steps {
         {
          sh 'tidy -q -e *.html'
        }

      }
    }
    stage('Upload to AWS') {
      steps {
        withAWS(region: 'us-west-2', credentials: 'dchaves')
        s3Upload(bucket: 'udacity-project04', pathStyleAccessEnabled: true, payloadSigningEnabled: true, file: 'index.html')
      }
    }
  }
}
