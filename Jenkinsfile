pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Building the ClinaNG application'
          }
        }

        stage('Regression Test') {
          steps {
            echo 'Testing the application'
          }
        }

        stage('Smoke Test') {
          steps {
            echo 'Deploy the application'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying the app'
      }
    }

  }
}