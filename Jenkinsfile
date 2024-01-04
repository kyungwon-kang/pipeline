pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh 'echo "test2"'
        sleep 3
      }
    }

    stage('111') {
      steps {
        sh 'echo 111'
        sleep 3
      }
    }

    stage('222') {
      parallel {
        stage('222') {
          steps {
            sh 'echo 222'
            sleep 3
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
        sleep 3
      }
    }

  }
}