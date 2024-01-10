pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=oniricobuggywebapp -Dsonar.organization=oniricobuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=1d29001b387151ee23f1d509339774ea3d1cc1ab'
			}
        } 
  }
}
