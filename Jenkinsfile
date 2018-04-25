pipeline {
	agent any
	environment {
	MAVEN_HOME = '/root/maven/apache-maven-3.5.3'
	}
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
				sh "${MAVEN_HOME}/bin/mvn test"
			}
		}
	}
}
