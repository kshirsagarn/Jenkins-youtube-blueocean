pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''
          date
          pwd 
'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test steps'
          }
        }

        stage('Test par') {
          steps {
            echo 'Test par'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
        sleep 10
      }
    }

  }
}