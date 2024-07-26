pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        echo '1 -stage'
      }
    }

    stage('QA') {
      parallel {
        stage('QA') {
          steps {
            echo 'qa completd'
          }
        }

        stage('Dev ') {
          steps {
            echo 'completed'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deployed '
      }
    }

  }
  environment {
    QA = 'QA'
  }
}