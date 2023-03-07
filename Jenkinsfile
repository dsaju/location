pipeline {
  agent any
  tools { 
        maven 'maven_3.5.2'  
    }
   stages{
    /*stage('Build') {
            steps {	
		sh 'mvn install'
	    }
    } */
	
    /*stage('Test') {
            steps {	
		sh 'mvn test'
	    }
    } */
	   
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=snyctraining -Dsonar.organization=snyctraining -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=51c09a8725c7a66d57594f42e74b2a53a055aa20'
	    }
    } 
   }
}
