pipeline{

  agent{

    node { label 'maven' }

  }

  stages{

    stage("Create Queues"){
        
      steps{
          
        echo "creates queue"

        script{

          def data = readJSON file:'queue-newsletter-mail.json'
            
          for (int i=0; i <= data.createroutins.length; i++){
              
            echo "queue name: ${data.createroutins[0].name}"
            
          }
        }
      }
    }

    stage("Add Security"){
      
      steps{
        echo "Add security"
      }

    }
  }
}
