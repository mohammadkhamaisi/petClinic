pipeline {
	agent {label 'slave'}
	stages{
	  stage('Clone'){ 
	  	steps{
			git branch: 'main' , url: 'https://github.com/spring-projects/spring-petclinic'
			sh 'cd spring-petclinic'

		}
	  }
	  stage('Build'){ 
	  	steps{ 
			script{ 
				"./mvnw package"
			} 
		}
	  }
	}
}
