pipeline {

  agent any
  
  parameters {
    
    choice(name: 'VERSION' , choices: ['1.1.0' , '1.2.0' , '1.3.0'] , description: 'version which is used to deploy to PROD')
    booleanParam(name: 'executeTests', defaultValue: true , description: '')
    
  }
  

  
  stages {
  
    stage("build") {
      
      steps {
         echo ' Testing out building of the application %date% %time% '
        
      }
    }
        stage("test") {
          when {
            expression {
                params.executeTests
            }
          }
      
      steps {
                 echo ' Testing out the application %date% %time%  '
         
        
      }
    }
        stage("deploy") {
      
      steps {
                 echo ' deplpying the application %date% %time%  '

        
      }
    }
  }
  post {
    always { 
      echo ' finalize '
  }
}
}



  
