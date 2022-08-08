pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed'
        retry(count: 3)
        sh 'wwwwwwwww'
      }
    }

    stage('Test2') {
      parallel {
        stage('Test2') {
          steps {
            echo 'Running Test2'
          }
        }

        stage('Test1') {
          steps {
            echo 'Running Test1'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        input(message: 'Are you sure to deploy?', ok: 'yes i am sure')
        echo 'Deployment completed'
      }
    }

    stage('error') {
      steps {
        echo 'New build completed succesfully'
      }
    }

  }
}