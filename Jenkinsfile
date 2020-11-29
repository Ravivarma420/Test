pipeline {
agent {
label 'latestnode'
}

stages {

stage ('Checkout') 
{
steps
    {
    
        checkout scm
        
    }
}
stage ('Build1')
 {
        steps
        {
            sh "cd /home/ubuntu/workspace/pipeline/account-service ; mvn clean install "
    
        }
 
   }
    
}
}

