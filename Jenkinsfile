node{
	stage('SCM checkout'){		
		git 'https://github.com/alex769292/my-app'
	}
	stage('Compile-Package'){
	 	def mvnHome = tool name: 'maven-3', type: 'maven'
		bat "${mvnHome}/bin/mvn package"
 }
}
	      
	
