node {
   stage('SCM Checkout') {
      git 'https://github.com/devops4cloud/my-app/'
   }
   stage('Compile-Package'){
      def mvnHome = tool name: 'Maven 3', type: 'maven'
      sh "${mvnHome}/bin/mvn package"
   }
   stage('Email Notification'){
       mail bcc: '', body: 'Here are the results', cc: '', from: '', replyTo: '', subject: 'Jenkins Build Results', to: 'prasantha@gmail.com'
   }
}
