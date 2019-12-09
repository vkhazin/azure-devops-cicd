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

### Step 1.1:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/AZ%201.PNG)

### Step 1.2:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/AZ%202.PNG)

### Step 1.3:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/AZ%203.PNG)

### Step 1.4:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/AZ%204.PNG)

## 2: Create Build Pipeline - [Azure DevOps](http://devops.azure.com/)

### Step 2.1:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d1.PNG)

### Step 2.2:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d2.PNG)

### Step 2.3:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d3.PNG)

### Step 2.4:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d4.PNG)

### Step 2.5:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d5.PNG)

### Step 2.6:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d6.PNG)

### Step 2.7:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d7.PNG)

### Step 2.8:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/d8.PNG)

## 4: Create Bitbukcet Repository - [Bitbucket.org](https://bitbucket.org/)

### Step 4.1:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/B%201.PNG)

### Step 4.2:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/B%202.PNG)

### Step 4.3:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/B%203.PNG)

### Step 4.4:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/B%204.PNG)

## 5: Create Bitbukcet Repository - [Bitbucket.org](https://bitbucket.org/)

### Step 5.1: Create Visual Studio Project - Create Azure Function and Add Bitbucket as Source Control
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/VS%201.PNG)

### Step 5.2:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/VS%202.PNG)

### Step 5.3:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/VS%203.PNG)

### Step 5.4:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/VS%204.PNG)

### Step 5.5:
![](https://github.com/MuddassirNayyer/azure-devops-cicd/blob/master/Images/VS%205.PNG)
