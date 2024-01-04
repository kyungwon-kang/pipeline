pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh 'echo "test2"'
        sleep 1
      }
    }

    stage('111') {
      steps {
        sh 'echo 111'
      }
    }

    stage('222') {
      parallel {
        stage('222') {
          steps {
            sh 'echo 222'
          }
        }

        stage('333') {
          steps {
            sh 'echo 333'
          }
        }

      }
    }

    stage('444') {
      steps {
        echo '444'
      }
    }

  }
}