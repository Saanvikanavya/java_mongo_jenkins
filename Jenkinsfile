pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'wget https://github.com/Saanvikanavya/java_mongo_jenkins/raw/master/org.mongodb.mongo-java-driver_3.8.2.jar'
        sh 'cp org.mongodb.mongo-java-driver_3.8.2.jar $JAVA_HOME/jre/lib/ext/'
      }
    }
    stage('Test') {
      steps {
        sh 'jmeter -n -t test-mongo.jmx -l test.jtl'
      }
    }
  }
}
