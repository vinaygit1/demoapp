node {
      stage('git checkout')
  git 'https://github.com/vinaygit1/demoapp.git'
   }
   stage ('compiling the code'){
       mvnhome = tool name: 'maven', type: 'maven'
       sh "${mvnhome}/bin/mvn package"
  }

