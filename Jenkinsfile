properties([parameters([choice(choices: ['abc', 'xyz', 'both'], description: 'Enter the value', name: 'archive')])])
node("master"){
    
    stage("workspace clean") {
    deleteDir()
   }
   
     stage("checkout scm") {
    checkout scm
  }
}
