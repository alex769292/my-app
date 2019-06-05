node{
	stage('SCM checkout'){		
		git 'https://github.com/alex769292/my-app'
	}
	stage('Compile-Package'){
	 	def mvnHome = tool name: 'maven-3', type: 'maven'
		bat "${mvnHome}/bin/mvn package"
	}
	stage('Email Notification'){
		mail bcc: '', body: 'Hi', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'alexandruobreja79@gmail.com'
 }
}
	      
	
