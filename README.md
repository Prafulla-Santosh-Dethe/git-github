# git-github
pipeline{
   agent any
    stages{
          stage('build'){
             steps{
                echo 'running build process...'
             }
          }
          stage('test'){
              steps{
                  input 'do u want to continue'
              }
           }
      }
}      
