pipeline{
  agent any
  stages{
    stage('Upload to AWS'){
      steps{
        withAWS(region:'us-west-2', credentials:'IDofAwsCredentials') {
          s3Upload(file:'index.html', bucket:'project3-jenkins-pipeline', path:'index.html')
        }
      }
    }
  }
}
