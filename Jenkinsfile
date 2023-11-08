pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=learning-devsecops -Dsonar.organization=learning-devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=dc85cf2515b0ec924104905e7a535b1c6b32088d'
			}
        } 
  }
}
