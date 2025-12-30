pipeline{
 agent any 
  stages{
      stage ('Clone Repo'){
        steps{
         echo 'Code already cloned by jenkins'
            }
         }
       stage ('Build Docker Image'){
        steps{
           bat 'docker build -t devops-web .'
          }
       }
       stage ('Run Docker Container'){
      steps {
         bat '''
         docker rm -f devops-web || echo Container not running
         docker run -d -p 8085:80 --name devops-web devops-web
         '''
         }
      }
    }
 }

