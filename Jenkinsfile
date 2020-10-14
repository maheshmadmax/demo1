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
        nodejs(nodeJSInstallationName: 'nodejs', configId: 'nodejs') {
          sh '''npm install
npm test
./deploy'''
        }

      }
    }

  }
}