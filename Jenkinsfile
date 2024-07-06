pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops-sandbox_devsecops-sandbox -Dsonar.organization=devsecops-sandbox -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=9add58d3efc15bee0071a49a932f69b217f0f719'
			}
        } 
  }
}
