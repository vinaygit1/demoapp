pipeline {
  agent any
  stages {
    stage('SCM CheckOut') {
      steps {
        git(url: 'https://github.com/ranjeetgill/demoapp.git', branch: 'master')
      }
    }
    stage('Message') {
      steps {
        echo 'Code Downloaded from GitHub Successfully'
      }
    }
    stage('Build') {
      steps {
        sh 'mvn clean install -f pom.xml'
      }
    }
  }
}