pipeline {
	agent any
	stages {
		stage('Build')	{
			steps {
				sh 'cd main && g++ hello.cpp -o brah'
				echo 'Build Stage Successful'
			}
		}
		stage('Test')	{
			steps {
				sh './brah'
				echo 'Test Stage Successful'
			}
		}
		stage('Deploy')	{
			steps {
				echo 'Deploy Stage Successful'
			}
		}
	}
	post {
		failure {
			echo 'Pipeline failed'
		}
	}
}
