pipeline {
    agent {
        node {
            label 'slave'
            
        }
        
    }
    
    stages {
        stage('git-clone') {
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/pia2896/game-of-life.git"
                
            }
            
        }
       stage('maven-build') {
           steps {
               
               sh "mvn test"
               
           }
           
       }
        
    } 
    
    
}
