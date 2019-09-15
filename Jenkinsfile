
node("master"){

    properties(
    [
        parameters(
            [string(defaultValue: PRODUCTION_SERVER, description: 'Server to deploy the package to', name: 'deployServer')]
            )

    ]
    
    stage("workspace clean") {
    deleteDir()
   }
   
     stage("checkout scm") {
    checkout scm
  }
}
