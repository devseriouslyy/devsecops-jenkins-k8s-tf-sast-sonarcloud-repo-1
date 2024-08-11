pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp238 -Dsonar.organization=asgbuggywebapp238 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c90ed52939253fdd4948957c6a795e56930242fc'
			}
        } 
  }
}
