// Declarative pipeline
pipeline {
	// agent any
	agent {docker {image 'maven:3.6.3'}}
	stages{
		stage("build") {
			steps {
				echo "Build"
			}
		}
		stage("Test") {
			steps {
				sh 'mvn --version'
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
