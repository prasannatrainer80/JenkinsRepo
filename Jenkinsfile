pipeline {
    agent any

    tools {
        jdk 'Java17'
        maven 'Maven3'
    }

    stages {
        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

       stage('Run App') {
    	steps {
        	bat 'mvn spring-boot:run'
    		}
	}

    }
}
