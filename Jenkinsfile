pipeline {
  agent any
  stages{
    stage ('GIT Checkout'){
      steps{
         git credentialsId: 'github', url: 'https://github.com/arquimedesjr/app_cicd_apirest' 
      }
    }
    stage ('Maven Build'){
      steps{
         bat 'mvn clean package' 
      }
    }
    stage('Test'){
     steps {
      
     }      
    }
   stage('Deploy') {
     steps {
        git credentialsId: 'heroku', url: 'https://git.heroku.com/apirestxampl.git'
        bat 'git remote add heroku https://git.heroku.com/apirestxampl.git'
        bat 'git push herocu master'
      }
    }
  }
}
