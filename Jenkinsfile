pipeline {
  agent any
  stages { 
    stage('Upload to AWS.') {
      steps {
        withAWS(credentials:'AKIARFC3GHJNLXKTJKGV') {
            s3Upload(file:'index.html', bucket:'udacityproject3', path:'index.html')
        }
      }
    }
  }
}
