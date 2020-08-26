pipeline('python_test/Python2') {                                             
    agent { node { label 'windows' } }
    stages
    {
      stage('python_test'){
            steps{
                jobDsl scriptText: "folder('python_test')",
                    ignoreExisting: true
                                                           
			definition {                                                                   
			  cpsScm {                                                                     
				scm {                                                                      
				  git('https://github.com/OperatorUNK/python2.git') {                      
					node ->                                                                
					node / gitConfigName('DSL User')                                       
					node / gitConfigEmail('me@me.com')                                
				  }                                                                        
				}                                                                          
				scriptPath('Jenkinsfile') 
				queue('python_test/Python2')
			  }
			 }
			}                                                                              
		}
	}		
 }                                                                                
