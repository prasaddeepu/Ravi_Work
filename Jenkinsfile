@Library('shared-library@master') _
pipeline {
   agent any
   environment {
        //int BN =  buildnumber1(JFROG_ID)
         JFROG_ID = credentials('jfrogid')
         //int inval = "${BN}"
       
      }
    

   stages {
      stage('Hello') {
         steps {
		 
		 
		 
           
    
    
	 script{
			
       
        build(job: "env_test_myjenk")
        build(job: "env_test_myjenk")
		build(job: "env_test_myjenk")
		build(job: "env_test_myjenk")
                   
                        
                                       
                    
       }
	   }
         
		 
      }
      }
}

def  buildnumber1(String JFROG_ID) {
 String url = "https://jfrgfreetst.jfrog.io/artifactory/api/storage/example-repo-local/?sort"
  int Bnumber = sh(script: "curl -u $JFROG_ID -s $url | grep uri |awk '{print \$3}'| sed 's+\"++g' | sed 's+/++g' | sed 's+,++g' |wc -l",returnStdout: true).trim()
  return Bnumber

}
