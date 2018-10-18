pipeline {
    agent any
    stages {
   		 
   		 stage('build') {
            steps {
             	withMaven(maven : 'Apache Maven 3.5.2') {
                	sh 'mvn --version'
                }
            }
         }
    
        stage('compile') {
            steps {
            	withMaven(maven : 'Apache Maven 3.5.2') {
                	sh 'mvn clean compile'
                }
            }
        }
    }
}