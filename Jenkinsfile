pipeline{
	agent any
	
	stages{
		stage('SCM'){
			steps{
				echo 'This is For Test Practising for Pipeline'
			}
		}
		stage('Code'){
			steps{
				//git Clon
				git 'https://github.com/rajaashkm/website.git'
			}
		}
		stage('Build'){
			steps{
				//Maven Build
				bat 'mvn clean test'
			}
		}
		stage('Compile'){
			steps{
				//Maven Compile
				bat 'mvn compile'
			}
		}
	}
}
