pipeline {
  agent any
  stages {
    stage('Checkout from GITHUB') {
      steps {
        git(url: 'https://github.com/vinaygit1/demoapp.git', branch: 'master')
      }
    }
    stage('Build_war') {
      steps {
        sh 'clean install'
      }
    }
    stage('jobcomplete') {
      steps {
        echo 'BUILD IS COMPLETE'
      }
    }
  }
}