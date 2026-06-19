pipeline{
	agent any
	tools{
	maven 'maven'
	}
	
	stages{
		stage('Checkout'){
			steps{
				git branch:'master',url:'https://github.com/bitcsedevops194/maven-1bi24cs416.git'
				}
		}
		stage('Build'){
			steps{
				sh 'mvn clean package'
			}
		}
		stage('Test'){
			steps{
				sh 'mvn test'
			}
		}
		
}
}
