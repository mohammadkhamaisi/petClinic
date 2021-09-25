
pipeline
{

//running on the slave label
agent {label 'slave'};

stages{
	stage('Clone And Build Project'){
		steps{
			//cloning the project PetClinic
			git branch: 'main', url: 'https://github.com/spring-projects/spring-petclinic'
			
			//entering the spring-petclinic directory
			sh 'cd spring-petclinic'

			//building the application
			script{
				"./mvnw package"
			      }
		     }
					}
      }
}
