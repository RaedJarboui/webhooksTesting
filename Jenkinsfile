pipeline {
agent any
stages{
stage('clone and clean repo'){
steps {

echo "hi"
  echo "Raedd"
}

}
  
}
   post {
        always {
            emailext body: 'A Test EMail', recipientProviders: [[$class: 'DevelopersRecipientProvider'], [$class: 'RequesterRecipientProvider']], subject: 'Test'
        }
    }
  
}
