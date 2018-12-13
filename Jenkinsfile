pipeline {
  agent any
  stages {
    stage('Init') {
      steps {
        echo 'eKYC service'
      }
    } 
    stage('Build') { 
      
        steps {
              sh 'pwd' 
              dir('ekyc-eureka-server-master'){ 
              sh 'pwd'
              }   
              sh 'mvn -B -DskipTests clean package' 
            }
        }
  }
}
