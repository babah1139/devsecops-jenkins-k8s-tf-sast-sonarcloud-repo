pipeline {
  agent any
  tools { 
        maven 'Maven'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecurityguru -Dsonar.organization=asecurityguru -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=1411675b025a0d1644199469dd69ae294d41d991'
			}
        } 
  }
}
