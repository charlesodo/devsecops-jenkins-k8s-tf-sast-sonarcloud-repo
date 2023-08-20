pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp0001 -Dsonar.organization=asgbuggywebapp0001 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=42a5777c1bcb7df74daefa735eb0022a85ff2613'
			}
        } 
  }
}
