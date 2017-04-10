pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        parallel(
          "Stage1": {
            sh 'date'
            
          },
          "stage2": {
            sh 'pwd'
            
          },
          "stage3": {
            sh 'whoami'
            
          },
          "stage4": {
            mail(subject: 'subject Mail', body: 'Body Mail', to: 'william.jr.ng@sap.com')
            
          }
        )
      }
    }
    stage('finish') {
      steps {
        echo 'finish'
      }
    }
  }
}