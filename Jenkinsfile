pipeline {
	agent any
	
	stages {
		stage('Build') {
			steps {
				echo 'Building..'
				sh "${MAVEN_HOME}/bin/mvn clean package"
			}
		}
		stage('Test') {
			steps {
				echo 'Testing..'
			}
		}
		stage('Deploy') {
			steps {
				echo 'Deploying..'
			}
		}
	}
}
