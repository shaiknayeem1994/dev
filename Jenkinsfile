pipeline 
{
  agent any
  stages {
    stage('Build Application') {
		steps {
        bat 'mvn clean install'
    }
	}
    stage('Deploy application to cloud hub') { 
      steps {
	  bat 'mvn package deploy -DmuleDeploy'
      }
    }
  }
}