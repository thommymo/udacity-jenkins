pipeline {
  agent any
  stages { 
    stage('Upload to AWS.') {
      steps {
        withAWS(region:'eu-central-1') {
            s3Upload(file:'index.html', bucket:'udacityproject3', path:'index.html')
        }
      }
    }
  }
}
