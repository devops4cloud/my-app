node {
   stage('SCM Checkout') {
   git 'https://github.com/devops4cloud/my-app/'
   }
   stage('Compile-Package'){
      sh 'mvn package'
   }
}
