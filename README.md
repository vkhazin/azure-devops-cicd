# azure-devops-cicd

## Scope

* Create a hello-world Azure function with Http trigger using dotnet core 2.2 C#
* Store code in Bitbucket.org
* On commit to `master` branch of the Bitbucket.org repo, trigger a build
* Build to compile the code, to run unit tests, and to create a deployment artifact with version number
* Upload generated artifact to Azure Artifacts
* Deploy generated binary artifact to Azure function
* Document steps and provide walk through
