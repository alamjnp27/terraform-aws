pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=alamdeen-project -Dsonar.organization=alamdeen-organisation -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=79045dce998106f6a0243eb862f24277991503a9'
			}
        } 
  }
}
