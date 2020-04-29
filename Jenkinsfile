pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        withAWS(credentials:'aws-static') {
          s3Upload(file:'.', bucket:'jenkins-20200429', path:'.')
        }
      }
    }
  }
}
