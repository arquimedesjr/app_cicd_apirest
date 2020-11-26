pipeline {
  agent any
  stages{
    stage ('GIT Checkout'){
      steps{
         git credentialsId: 'github', url: 'https://github.com/arquimedesjr/app_cicd_apirest' 
      }
    }
  }
}
