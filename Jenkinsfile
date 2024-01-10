// Declarative pipeline
pipeline {
	agent any
	// agent {
	// 	docker { image 'node:20.10.0-alpine3.19' }
	// }
	stages{
		stage("build") {
			steps {
				echo "Build"
				echo "PATH - $PATH"
				echo "BIULD_NUMBER - $env.BUILD_NUMBER"
				echo "BUILD_ID - $env.BUILD_ID"
				echo "JOB_NAME - $env.JOB_NAME"
				echo "BUILD_TAG - $env.BUILD_TAG"
				echo "BUILD_URL - $env.BUILD_URL"

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
