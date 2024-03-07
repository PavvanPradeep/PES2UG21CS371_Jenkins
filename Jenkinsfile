pipline {
  agent any
  stges {
    stage('Build') {
      steps {
        sh 'g++ -o task5 main/hello.cpp'
        echo 'Build Successful!'
      }
    }
    sage('Test') {
      steps {
        sh './task5'
        echo 'Test Successful!'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Successfully deployed!'
      }
    }
  }
  post {
    failure {
      echo 'Pipeline Failed!'
    }
  }
}
