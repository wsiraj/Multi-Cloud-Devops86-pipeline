pipeline {
  agent any
  stages {
    stage('Plan') {
      steps {
        echo 'plan the pipeline'
      }
    }

    stage('code') {
      steps {
        echo 'develop the code'
      }
    }

    stage('Biuld') {
      steps {
        echo 'code will be build'
      }
    }

    stage('deploy') {
      parallel {
        stage('deploy') {
          steps {
            echo 'code will be deploy'
          }
        }

        stage('test2') {
          steps {
            echo 'test2'
          }
        }

        stage('operate') {
          steps {
            echo 'operate'
          }
        }

      }
    }

  }
}