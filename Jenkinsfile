pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggyapp-1 -Dsonar.organization=buggyapp-1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=aad348d7f3bfe089fd31d4e29ed1b3f3e24ee180'
			}
        } 
  }
}
