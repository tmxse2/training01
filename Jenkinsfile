pipeline {
   agent any
   stages {
     stage ('build') {
       steps {
         bat 'mvn clean package'
       }
     }
        
      stage ('deploy') {
       steps {
         bat 'git remote set-url origin https://tmxse2@github.com/tmxse2/training01.git'
         bat 'git add .'
         bat 'git checkout main'
         bat 'git commit -m "Jenkins commit"'      
         bat 'git push origin main'          
       }
     }
   }
 }
