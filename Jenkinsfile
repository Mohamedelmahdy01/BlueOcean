pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Completed'
      }
    }

    stage('Test stages') {
      parallel {
        stage('Test stages') {
          steps {
            echo 'tseststep'
          }
        }

        stage('test1') {
          steps {
            echo 'tsest1'
            echo 'test1.1'
          }
        }

        stage('test2') {
          steps {
            echo 'test2'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        input(message: 'Are you sure to deploy', ok: 'Yes, i am sure')
        echo 'Deploy statge'
      }
    }

  }
}