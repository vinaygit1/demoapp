node {
   def mvnHome
   stage('Preparation') { // for display purposes
      // Get some code from a GitHub repository
      git 'https://github.com/vinaygit1/demoapp.git'
      
   }
  stage ('build the war file'){
    sh "mvn clean install"   
   } 
   stage ('deploytotomcat'){
   sh "sudo cp target/demoapp.war /opt/tomcat/apache-tomcat-8.0.50/webapps"
   }

   
}
