pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'wget https://github.com/Saanvikanavya/java_mongo_jenkins/raw/master/org.mongodb.mongo-java-driver_3.8.2.jar'
      }
    }
    stage('Test') {
      steps {
        sh 'jmeter -n -t test-mongo.jmx -l test.jtl'
      }
    }
    stage('view_jtl') {
      steps {
        sh 'cat test.jtl'
      }
    }
  }
}