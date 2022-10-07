pipeline {
  agent any
    environment {
        JAVA_HOME= "/var/jenkins_home/tools/hudson.model.JDK/JDK17/jdk-17.0.4.1"
    }
    
    
  stages {


      stage('jdk 17') {
    tools {
        maven 'mvnapp'
        jdk 'JDK17'
  }
      steps {
          sh 'echo $JAVA_HOME'
          sh 'java -version'
          sh 'javac -version'
          sh 'mvn clean package'
        }
      }
  }
}
