pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh 'echo "test"'
        bat 'test'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'build'
          }
        }

        stage('build par') {
          steps {
            echo 'parallel'
          }
        }

      }
    }

  }
}