properties([parameters([choice(choices: ['abc_abc', 'abc_xyz', 'both'], description: 'Enter the value', name: 'archive')])])
node("master"){
    
    stage("workspace clean") {
    deleteDir()
   }
   
     stage("checkout scm") {
    checkout scm
  }
      stage("build") {
          
    try {
        dir("${archive}"){
            
        sh "dir"
            }
         }catch(Exception ex) {
      error "Error encountered while building the rpm. Please go through the logs for more details"
    }
  }

}
