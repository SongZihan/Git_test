pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'test stage'
      }
    }

    stage('deploy') {
      steps {
        ws(dir: '/tmp/git_test') {
          sh 'echo "test step" > log.log'
        }

      }
    }

  }
}