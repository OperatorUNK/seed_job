folder('python_test')                                                            
                                                                                 
                                                                                 
pipelineJob('python_test/Python2') {                                             
  triggers {                                                                     
                                                                                 
  }                                                                              
  description = "Python 2 tests"                                                 
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
    }                                                                            
  }                                                                              
}                                                                                
                                                                                 
queue('python_test/Python2')
