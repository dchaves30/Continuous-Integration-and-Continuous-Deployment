pipeline {
    agent any
    stages {
      stage(‘Lint HTML’) {
        steps {
          withAWS(region:’us-west-2’,credentials:’dchaves’)
          sh ‘tidy -q -e *.html’
        }
      stage(‘Upload to AWS’) {
        steps {
           {
            s3Upload(pathStyleAccessEnabled:true, payloadSigningEnabled: true, file:’index.html’, bucket:’udacity-project04’)
          }
        }
      }
    }
}
