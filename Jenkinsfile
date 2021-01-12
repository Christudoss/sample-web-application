pipeline{

      agent {
                any {
                image 'maven'
                args '-v $HOME/.m2:/root/.m2'
                }
            }
        
	
        stages{

              stage('Quality Gate Status Check'){
                  steps{
                      script{
			      def mvnHome = tool name: 'Maven  setting', type: 'maven'
			      sh "${mvnHome}/bin/mvn clean install"
                 	}

               	 }  
              }	
		
            }	       	     	         
}
