pipeline{
		agent any 
		
		stages{
			stage ('GIT'){
				steps {
					 git 'https://github.com/MonicaRamesh25/Today_class.git'
						}
						}
			stage ('BUILD'){
				steps {
						sh label: '', script: 'mvn clean'
						sh label: '', script: 'mvn install'
					}
						}
			stage ('Deployment'){
				steps {
						sh label: '', script: 'cp -rp "/var/lib/jenkins/workspace/Pipeline_project/target/hippo.war" "/opt/apache-tomcat/webapps"'
					}
					    	}
			}
				
		}
