pipeline {
  agent any
  stages {
    stage('from SCM') {
      steps {
        echo 'SCM stage successful'
      }
    }

    stage('Deploy_Dev') {
      parallel {
        stage('Deploy_Dev') {
          steps {
            echo 'DEV_successful'
          }
        }

        stage('Deploy_QA') {
          steps {
            echo 'QA_successful'
          }
        }

      }
    }

    stage('Deploy_prod') {
      steps {
        echo 'Prod successful'
      }
    }

  }
}