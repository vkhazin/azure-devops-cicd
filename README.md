# azure-devops-cicd

## Scope

* Create a hello-world Azure function with Http trigger using dotnet core 2.2 C# running on Linux
* Store code in Bitbucket.org
* On commit to `master` branch of the Bitbucket.org repo, trigger a build
* Build to compile the code, to run unit tests, and to create a deployment artifact with version number
* Upload generated artifact to Azure Artifacts
* Deploy generated binary artifact to Azure function
* Document steps and provide walk through

--------------------------------------------------------------

# Create Function App in Azure

* Step 1:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/AZ%201.PNG)

* Step 2:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/AZ%202.PNG)

* Step 3:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/AZ%203.PNG)

* Step 4:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/AZ%204.PNG)
