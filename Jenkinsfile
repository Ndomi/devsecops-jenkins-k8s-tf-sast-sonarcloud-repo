pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=ndomi -Dsonar.organization=ndomi -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=13b8ab011c1b05a41fcaad36b5b7feec6811b3a5'
			}
        } 
  }
}
