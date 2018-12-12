pipeline {
  agent any
  stages {
    stage('Init') {
      steps {
        echo 'Hello World'
      }
    } 
    stage('Build') { 
            steps {
              sh 'cd ekyc-eureka-server-master'   
              sh 'mvn -B -DskipTests clean package' 
            }
        }
  }
}
