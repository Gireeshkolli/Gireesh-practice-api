pipeline {
 agent any
	 stages {
		stage('Build') {
			steps {
				bat 'mvn clean install'
			}
		}
		stage('Test') {
			steps{
				bat 'mvn test'
			}
		}
		stage('Deployment') {
			steps{
				bat 'mvn deploy -DmuleDeploy'
			}
		}
	}
}

				