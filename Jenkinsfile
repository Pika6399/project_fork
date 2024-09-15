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
		   
		   
		   
		   
		   
		   }
	  
	  
	  
	  }




