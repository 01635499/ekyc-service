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
             
              sh 'mvn -f ./ekyc-eureka-server-master/pom.xml -B -DskipTests clean package' 
        }
    }
     stage('Deploy') {
      steps {
        echo 'Deploying'
        sh './jenkins/scripts/deliver.sh'
      }
    }
    
   }
}
