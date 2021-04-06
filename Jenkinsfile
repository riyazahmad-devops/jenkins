node{
	stage('SCM Checkout'){
	git 'https://github.com/riyazahmad-devops/jenkins.git'
	
	}
    stage('Compile-Package'){
	//Get maven home path
	def mvnHome = tool name: 'maven-3', type: 'maven'
	sh "${mvnHome}/bin/mvn package"
	}
	stage('Email Notification'){
	 
	 mail bcc: '', body: '''hi

this mail from jenkins build''', cc: 'riyaz@8squarei.com', from: '', replyTo: '', subject: 'Hellow from jenkins', to: 'riyaz.nep@gmail.com'
	
	}
}
