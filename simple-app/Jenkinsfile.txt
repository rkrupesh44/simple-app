pipeline {
    agent any
	// tool generally comes under stages block
	tools {
	  maven 'maven3'
	}
	stages{
		stage('Build'){
			steps{
				// mvn clean package
				sh 'mvn clean package'
			}
		}
	}
	
}