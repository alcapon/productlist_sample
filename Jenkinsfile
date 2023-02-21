pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'test message'
      }
    }

    stage('build') {
      steps {
        echo 'This is build number ${BUILD_ID}'
      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}