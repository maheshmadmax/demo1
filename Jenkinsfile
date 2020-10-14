pipeline {
  agent any
  stages {
    stage('clone') {
      steps {
        git 'https://github.com/maheshmadmax/demo.git'
      }
    }

    stage('build') {
      steps {
        nodejs 'nodejs'
      }
    }

  }
}