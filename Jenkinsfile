node{
 stage ('scm checkout'){
      git 'https://github.com/vinaygit1/demoapp.git'
      }
stage ('compiling the code'){
def mvnhome = tool name: 'maven', type: 'maven'
      sh "${mvnhome}/bin/mvn package"
 stage('SonarQube analysis') {
  def mvnhome = tool name: 'maven', type: 'maven'
    withSonarQubeEnv('sonar') {
     sh "${mvnhome}/bin/mvn sonar:sonar"
    }
  }
}
}
