pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=nmdevsecops -Dsonar.organization=nmdevsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=f3308b53dac15f4c993724fbe789a688ae4f1292'
			}
        } 
  }
}
