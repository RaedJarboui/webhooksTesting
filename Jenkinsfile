pipeline {
agent any
stages{
stages {
    stage('Ok') {
        steps {
            echo "Ok"
        }
    }
}
   post {
    always {
        emailext body: 'A Test EMail', recipientProviders: [[$class: 'DevelopersRecipientProvider'], [$class: 'RequesterRecipientProvider']], subject: 'Test'
    }
}
  
}
