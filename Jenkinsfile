pipeline {
	agent any 
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build & compile') {
	           steps {
			  sh '/home/rushi/Documents/Devops-software/apache-maven-3.9.7/bin/mvn install'
	                 }}
		stage('Deployment'){
		   steps {
		sh 'cp target/GRRAS.war /home/rushi/Documents/Devops-software/apache-tomcat-9.0.89/webapp'
			}}	
}}
