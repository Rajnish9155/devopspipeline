pipeline {
  agent any
  stages {
    stage('Plan') {
      steps {
        echo 'This is Planning Stage'
      }
    }

    stage('Code') {
      steps {
        echo 'This is coding part'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'This is build Part'
          }
        }

        stage('Test') {
          steps {
            echo 'This is testing'
          }
        }

        stage('Release') {
          steps {
            echo 'Relasing the code'
          }
        }

        stage('Deploye') {
          steps {
            echo 'Deploying the code'
          }
        }

        stage('Operate') {
          steps {
            echo 'Operating the dev server'
          }
        }

      }
    }

  }
}