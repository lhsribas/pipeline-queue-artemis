pipeline{

  agent{

    node { label 'maven' }

  }

  stages{

    stage("Create Queues"){
        
        echo "creates queue"

        //def data = readJson file:'queue-newsletter-mail.json'
        //echo "queue name: ${data.createroutins[0].name}"
    }

    stage("Add Security"){
      
      echo "Add security"

    }

  }

}
