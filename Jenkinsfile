pipline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        withAWS(region:'eu-east-1', credentials:'aws-static') {
          s3Upload(file:'index.html', bucket:'udacityjenkinsnano', path:'index.html')        }
      }
    }
  }
}
        
