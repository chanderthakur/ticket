    properties(
    [
        parameters(
            [string(defaultValue: PRODUCTION_SERVER, description: 'Server to deploy the package to', name: 'deployServer')]
            )

    ]
       )
node("master"){
    
    stage("workspace clean") {
    deleteDir()
   }
   
     stage("checkout scm") {
    checkout scm
  }
}
