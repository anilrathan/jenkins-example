pipeline {
	agent any
	stages {
		stage('---clean---'){
			steps {
				tool name: 'mvn3.6.0', type: 'maven'
				sh "mvn clean"
			}
		}
		stage('---test---') {
			steps {
				tool name: 'mvn3.5.4', type: 'maven'
				sh "mvn test"
			}
		}
		stage('---package---'){
			steps {
				tool name: 'maven3.3.3', type: 'maven'
				sh "mvn package"
			}
		}
	}
}
