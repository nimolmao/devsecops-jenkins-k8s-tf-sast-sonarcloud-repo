pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopsbuggy -Dsonar.organization=devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=66e2b1a10d5c902a8f5364bd0a799662890c452e'
			}
        } 
  }
}
