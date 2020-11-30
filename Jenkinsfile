pipeline {
agent {
label 'latestnode'
}
parameters{
    choice(name: 'microservices',
       choices: 'account-service\ncustomer-service',
        description: 'build with below microservices')
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
            sh "cd /home/ubuntu/workspace/pipeline/${microservices} ; mvn clean install "
    
        }
 
   }
    
}
}

