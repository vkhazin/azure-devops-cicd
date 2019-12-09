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

## 1: Create Function App in Azure - [Azure Portal](https://portal.azure.com/)

### Step 1.1: Create Function App in Azure Portal
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/AZ%201.PNG)

### Step 1.2: Click on Add
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/AZ%202.PNG)

### Step 1.3: Add Basic Information
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/AZ%203.PNG)

### Step 1.4: Change Hosting and Select Service Plan
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/AZ%204.PNG)


## 2: Create Build Pipeline - [Azure DevOps](http://devops.azure.com/)

### Step 2.1: Create a new Project
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d1.PNG)

### Step 2.2: Enter name and visibiliity of the Project
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d2.PNG)

### Step 2.3: Create Build Pipeline
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d3.PNG)

### Step 2.4: Select Classic Editor
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d4.PNG)

### Step 2.5: Choose Bitbucket and Authorize using OAuth or Username and Password
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d5.PNG)

### Step 2.6: Select the Repository and Branch
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d6.PNG)

### Step 2.7: Select Azure Functions for .Net template
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d7.PNG)

### Step 2.8: Enable Continuous Integration and save the pipeline
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d8.PNG)


## 3: Create Release Pipeline - [Azure DevOps](http://devops.azure.com/)

### Step 3.1:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d9.PNG)

### Step 3.2: Select 'Deploy a function app to Azure Functions' template
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d10.PNG)

### Step 3.3: Click on 'Add an Artifact'
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d11.PNG)

### Step 3.4: Select the Project, build pipeline (created in previous step) and let other options default
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d12.PNG)

### Step 3.5: Enable Continuous Deployment Trigger
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d13.PNG)

### Step 3.6:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d14.PNG)

### Step 3.7: Click on 'Job , Task' link under stages
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d15.PNG)

### Step 3.8: Select Azure Subscription, App Type (Windows Function App or Linux Function App), and App Service Name
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d16.PNG)

### Step 3.9: Save the release pipeline
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d17.PNG)


## 4: Create Bitbukcet Repository - [Bitbucket.org](https://bitbucket.org/)

### Step 4.1: Click on '+' icon
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/B%201.PNG)

### Step 4.2: Click on Repository
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/B%202.PNG)

### Step 4.3: Enter required Reposioty Information and create Repo
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/B%203.PNG)

### Step 4.4: Copy this Remote access Repository Link
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/B%204.PNG)


## 5: Create Visual Studio Project - Create Azure Function and Add Bitbucket as Source Control

### Step 5.1: Open Visual Studio and Create a new Project of type 'Azure Functions' 
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/VS%201.PNG)

### Step 5.2: Configure the new project
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/VS%202.PNG)

### Step 5.3: Create Http Trigger Function
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/VS%203.PNG)

### Step 5.4: Add project to source control
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/VS%204.PNG)

### Step 5.5: Use Remote Repository link here which you copied in previous step
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/VS%205.PNG)
