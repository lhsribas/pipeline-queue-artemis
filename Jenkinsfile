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
            echo "queue name: ${data.createroutins[0].name}"

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
