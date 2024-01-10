// Declarative pipeline
pipeline {
	// agent any
	agent {
		docker { image 'node:20.10.0-alpine3.19' }
	}
	stages{
		stage("build") {
			steps {
				sh 'node --version'
				echo "Build"
			}
		}
		stage("Test") {
			steps {
				echo "Test"
			}
		}
		stage("Integration Test") {
			steps {
				echo "Integration Test"
			}
		}
	
	}
	post{
		always{
			echo 'I am awesom.I run always'
		}
		success{
			echo 'I run when you are successful'
		}
		failure{
			echo 'I run when you are fail'
		}
	}
}
	



















// Scripting pipeline
// node {
// 	stage('Build') {
// 		echo "Build"
// 	}
// 	stage('Test') {
// 		echo "Test"
// 	}
// 	stage('IntegrationTest') {
// 		echo "Test"
// 	}
// }
