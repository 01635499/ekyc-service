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
              sh 'pwd' 
              sh 'cd ./ekyc-eureka-server-master'
              sh 'mvn -B -DskipTests clean package' 
            }
        }
  }
}
