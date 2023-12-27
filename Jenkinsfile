pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'building'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
          }
        }

        stage('error') {
          steps {
            echo 'test para'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}