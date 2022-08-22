pipeline {
   agent any
   stages {
     stage ('build') {
       steps {
         bat 'mvn clean package'
       }
     }
        
      stage('archive artifacts') {
        steps {
          archiveArtifacts artifacts: 'ROOT.war'
        }
      }
   }
 }
