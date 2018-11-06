pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        
      }
    }
    stage('Test') {
      steps {
        echo 'Testing..'
      }
    }
    stage('Deploy') {
      steps {
        sh 'docker run -d -p 5000:5000 my-flask-image'
      }
    }
  }
}
