pipeline {
	agent any
	stages {
		stage('Clone Repository') {
			steps {
				git branch: 'main', url: 'https://github.com/SNEGHAJOSHE/sample-ci-demo.git'
			}
		}	
		stage('Build') {
			steps {
				echo 'Build step...'
			}
		}
		stage('Test') {
			steps {
				echo 'Running tests...'
				sh 'python3 hello.py'
			}
		}
	}
}
