pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        withAWS(credentials:'aws-static', region:'eu-east-1') {
          s3Upload(file:'index.html', bucket:'udacityjenkinsnano', path:'index.html') 
        }
      }
    }
  }
}
        
