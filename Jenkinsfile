pipeline { 
    agent any
    tools {
        maven "maven"
    }
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
                  
        stage('Maven build'){
          steps{
                
                script{
                    
                    sh 'mvn clean install'
                }
            }
        }
        
}
}
