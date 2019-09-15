properties([parameters([choice(choices: ['abc', 'xyz', 'both'], description: 'Enter the value', name: 'archive')])])
node("master"){
    
    stage("workspace clean") {
    deleteDir()
   }
   
     stage("checkout scm") {
    checkout scm
  }
      stage("build") {
          
    try {
        dir("${env.WORKSPACE}\${archive}_abc"){
    sh "make"
        }
         }catch(Exception ex) {
      error "Error encountered while building the rpm. Please go through the logs for more details"
    }
  }

}
