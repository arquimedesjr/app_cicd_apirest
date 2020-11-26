node {
  
    stage ('SCM Checkout'){
            git 'https://github.com/arquimedesjr/app_cicd_apirest'
         
    }
    
    stage ('Compile-package'){
            bat 'mvn package'
         
    }
    
}
