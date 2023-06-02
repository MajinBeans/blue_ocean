pipeline {
  agent any
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test'
          }
        }

        stage('Parallel') {
          steps {
            echo 'Parallel'
          }
        }

      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Build'
          }
        }

        stage('Run') {
          steps {
            echo 'Run'
          }
        }

      }
    }

    stage('Clean Up') {
      steps {
        echo 'Clean up'
      }
    }

  }
}