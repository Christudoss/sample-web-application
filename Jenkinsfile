pipeline{

      agent {
                any {
                image 'maven'
                args '-v $HOME/.m2:/root/.m2'
                }
            }
        def mvnHome = tool name: 'Maven  setting', type: 'maven'
	
        stages{

              stage('Quality Gate Status Check'){
                  steps{
                      script{
			      sh "${mvnHome}/bin/mvn clean install"
                 	}

               	 }  
              }	
		
            }	       	     	         
}
