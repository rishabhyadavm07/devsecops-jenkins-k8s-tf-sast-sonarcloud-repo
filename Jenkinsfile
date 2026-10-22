pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=asgbuggywebapp1199 -Dsonar.organization=Devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=8577bc9db4fbfd1e861df106907b000d2a5d8a81'
			}
        } 
  }
}
