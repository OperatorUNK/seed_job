folder('python_test')
folder('python_test/Python2')


pipelineJob('python_test/Python2') {                                             
                                                                            
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
                                                                                 
queue('python_test/Python3')

folder('python_test/Python3')
pipelineJob('python_test/Python3') {                                             
                                                                            
  description = "Python 3 tests"                                                 
  definition {                                                                   
    cpsScm {                                                                     
      scm {                                                                      
        git('https://github.com/OperatorUNK/python3.git') {                      
          node ->                                                                
          node / gitConfigName('DSL User')                                       
          node / gitConfigEmail('me@me.com')                                
        }                                                                        
      }                                                                          
      scriptPath('Jenkinsfile')                                                  
    }                                                                            
  }                                                                              
}                                                                                
                                                                                 
queue('python_test/Python3')
