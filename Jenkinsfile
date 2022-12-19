pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building code'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing code'
          }
        }

        stage('Deploy') {
          steps {
            echo 'Deployed'
          }
        }

      }
    }

  }
}