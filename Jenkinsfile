pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }

    stage('Test-Firefox') {
      parallel {
        stage('Test-Firefox') {
          steps {
            sh 'echo "testing in firefox"'
          }
        }

        stage('Test-Chrome') {
          steps {
            sh 'echo \'Test-chrome\''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying//,,,,'
      }
    }

  }
}