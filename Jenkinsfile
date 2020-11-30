pipeline {
agent {
label 'latestnode'
}
properties([parameters([choice(choices: 'account-service\ncustomer-service', description: 'build with above params', name: 'microservices')])])  

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

