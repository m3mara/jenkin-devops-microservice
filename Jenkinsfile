pipeline {
	// agent any
	agent {
		docker {
			image 'maven:3-alpine'
		}
	}
	stages {
		stage('Build') {
			steps {
				sh "mvn --version"
				echo "Build"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	} 

	post {
		always {
			echo 'Im awesome. i run always'
		}
		success {
			echo 'Im run when you are successful'
		}
		failure {
			echo 'Im run when you are fail'
		}
		// changed
	}
}