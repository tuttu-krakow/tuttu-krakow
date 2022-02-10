pipeline {

  agent any
  
  stages {
  
    stage("build") {
      
      steps {
         echo ' Testing out building of the application %date% %time% '
        
      }
    }
        stage("test") {
      
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



  
