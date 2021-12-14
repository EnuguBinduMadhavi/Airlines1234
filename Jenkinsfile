 pipeline {
   agent any
   stages {
     stage('Build') {
       steps {
            echo "build success"    
       }
     }
 
     stage('Test') {
       steps {
           echo "mvn test starts"
        
       }
     }
 
      stage('Deploy Development') {
       steps {
             bat "mvn clean package deploy -DmuleVersion=4.4.0 -Dusername=Apisero2511 -Dpassword=Apisero2511 -DapplicationName=airlines-ws-omvk958 -Denvironment=Sandbox -Dworkers=1 -DworkerType=Micro -DmuleDeploy"
             echo "deploy success"      
 }}}}