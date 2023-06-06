pipeline { 
    agent any
    stages {
        stage('Git Checkout'){
            
                     steps{
                
                        script{
                            git 'https://github.com/Maddalarajesh/hello-world.git'
                        }
                     }
                  }
                   stage('unit Testing'){
            
                      steps{
                
                       script{
                    
                         sh 'mvn test'
                       }
                          
                      }
                       
                   }
                   stage('Integration testing'){
            
            steps{
                
                script{
                    
                    sh 'mvn verify -DskipUnitTests'
                }
            }
        }
        stage('Maven build'){
          steps{
                
                script{
                    
                    sh 'mvn clean install'
                }
            }
        }
        
}
}
