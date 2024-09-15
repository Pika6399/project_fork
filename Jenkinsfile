pipeline{

      agent {
	       label{
		        label "built-in"
				customWorkspace "/mnt/project"
		        }
	  
	  
	  }
      stages {
	       stage ("compile"){
		          steps{           sh "git clone https://github.com/Pika6399/project_fork.git"
				           sh "cd /root/.m2/repository"
					   sh "rm -rf *"
					   sh "cd /mnt/project/project_fork"
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
