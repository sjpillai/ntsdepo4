pipeline {
  agent any
  stages {
    stage('pull SCM') {
      steps {
        echo 'Pull scm stage successful'
      }
    }

    stage('Deploy_dev') {
      parallel {
        stage('Deploy_dev') {
          steps {
            echo 'Deploy DEV success'
          }
        }

        stage('Deploy_QA') {
          steps {
            echo 'Deploy QA success'
          }
        }

      }
    }

    stage('Deploy_PROD') {
      steps {
        echo 'Deploy PROD success'
      }
    }

  }
}