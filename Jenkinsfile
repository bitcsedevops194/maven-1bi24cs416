pipeline{
	agent any
	tools{
	maven 'Maven'
	}
	
	stages{
		stage('Checkout'){
			steps{
				git branch:'master',url:'https://github.com/bitcsedevops194/maven-1bi24cs416.git'
				}
		}
		stage('Build'){
			steps{
				sh 'mvn compile'
				
				}
		}
		stage('Test'){
			steps{
				sh 'mvn test'
				
				}
		}
		stage('Run Application'){
			steps{
				sh 'java -jar target/maven-1bi24cs416-1.0-SNAPSHOT.jar'
				}
		}
	}
}
