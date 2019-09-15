properties([
  parameters([
    string(name: 'DEPLOY_ENV', defaultValue: 'TESTING', description: 'The target environment')
   ])
])
node("master"){
    
    stage("workspace clean") {
    deleteDir()
   }
   
     stage("checkout scm") {
    checkout scm
  }
}
