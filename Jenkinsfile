node{
 stage ('scm checkout'){
      git 'https://github.com/vinaygit1/demoapp.git'
      }
stage ('compiling the code'){
 mvnhome = tool name: 'maven', type: 'maven'
      sh "${mvnhome}/bin/mvn package"
 stage('SonarQube analysis') {
   mvnhome = tool name: 'maven', type: 'maven'
    withSonarQubeEnv('sonarserver') {
     sh "${mvnhome}/bin/mvn sonar:sonar"      
    }
  }
}
}
