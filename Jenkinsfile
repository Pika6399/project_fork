pipeline{

      agent {
	       lable{
		        lable "built-in"
				CustomWorkspace "/mnt/project"
		        }
	  
	  
	  }
      stages {
	       stage ("compile"){
		          steps{
				       sh "cd /root/.m2/repository"
					   sh "rm -rf *"
					   sh "cd /mnt/project/"
					   sh "mvn clean install"
				  
				  }
		   
		   }
		   
		   stage ("deploy"){
		         steps{
				       sh "cp LoginWebApp.war /mnt/servers/apache-tomcat-9.0.94/webapps/"
				 
				 
				 }
		   
		   
		   
		   }
	  
	  
	  
	  }




}
