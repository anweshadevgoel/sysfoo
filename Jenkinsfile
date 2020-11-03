pipeline {

  agent any

  tools {
  //name of the tool configured on Jenkins
   maven 'Maven 3.6.3'
  }
  
  stages{
    stage('build'){
      steps {
      //to get the syntax, you can use pipeline syntax: shell script
       sh 'mvn compile'
      }
    } 
    
    stage('test'){
      steps {
      sh 'mvn clean test'
      }
    } 
    
    stage('package'){
      steps {
      sh 'mvn package -DskipTests'
      }
    } 
    
  }
}
