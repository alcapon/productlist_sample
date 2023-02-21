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
        sh 'rsync -avu --delete "/var/lib/jenkins/workspace/testpipe_main/" "/srv/http"'
        echo 'Delopy finnish'
      }
    }

  }
}