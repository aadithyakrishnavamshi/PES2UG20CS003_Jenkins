pipeline {
	agent any
	stages {
		stage('Build')	{
			steps {
// 				sh 'cd main && g++ hello.cpp -o brah'
				sh 'cd main && g++ hello.cpp -o brah && dir'
				echo 'Build Stage Successful'
			}
		}
		stage('Test')	{
			steps {
				sh 'cd  main && ./brah'
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
