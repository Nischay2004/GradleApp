pipeline{
	agent any
	tools{
		gradle 'Gradle'
		jdk 'JDK'
	}
	
	stages{
		stage('Checkout'){
			steps {
				git 'https://github.com/Nischay2004/GradleApp.git'
			}
		}
		
		stage('Build'){
			steps {
				sh 'gradle build'
			}
		}
		
		stage('Test'){
			steps{
				sh 'gradle test'
			}
		}
		
		stage('Run Application'){
			steps {
				sh 'gradle run'
			}
		}
	}
}
