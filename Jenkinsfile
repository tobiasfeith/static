pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        withAWS(credentials:'AKIAZQBYRF7SSQCD7RES') {
          s3Upload(file:'.', bucket:'jenkins-20200429', path:'.')
        }
      }
    }
  }
}
