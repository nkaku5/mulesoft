pipeline{

	agent any
	stages{
		stage('Build Application'){
			steps{
				bat 'mvn clean install'
			}
		}
		
		stage('Deploy Application in to CloudHub'){
			steps{
				bat 'mvn clean package deploy -DmuleDeploy'
			}
		}
	}

}