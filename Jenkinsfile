pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecuritygurubuggywebapp -Dsonar.organization=asecuritygurubuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=a11f7eaaaa7b484e86f45e387b210e63dfa99cef'
			}
        } 
  }
}
