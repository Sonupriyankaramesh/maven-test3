pipeline{
	agent any
	tools{
		maven 'Maven'
	}
	stages{
		stage('Checkout')
		{
		steps{
		
			git "https://github.com/Sonupriyankaramesh/maven-test3.git"
			}
		}
		
		stage('Build'){
			steps{
				sh'mvn clean install'
			}
		}
		stage('Package')
		{
			steps
			{
				sh'mvn test'
			}
		}
	}
}
	
