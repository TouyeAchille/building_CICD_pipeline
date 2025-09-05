# Overview

<TODO: complete this with an overview of your project>

## Project Plan
<TODO: Project Plan

* A link to a Trello board for the project
* A link to a spreadsheet that includes the original and final project plan>

## Instructions for running this Python project

<TODO:  
* Architectural Diagram (Shows how key parts of the system work)>

<git@github.com>:TouyeAchille/building_CICD_pipeline.git

Include screenshots with explicit steps to create that work. Be sure to at least include the following screenshots:

To run this project follow step below :

 1 - Fork this repository to your github account
 
2 - In Azure Cloud Shell, clone your forked repository to Azure with the following command and Change directory to the cloned repository folder.
- Option 1 :
![Install dependencies]("screenshot/Screenshot 2025-09-05 at 12.35.02.png")

- Option 2 :

* Create public/private rsa key pair via ssh command and take your public key in '/home/odl_user/.ssh/id_rsa.pub'(replacing with your path) then, put this keys in the repository you fork.
![Install dependencies]("screenshot/screenshot/Screenshot 2025-09-05 at 11.57.39.png")

* git clone your forked repository with follow command and Change directory to the cloned repository folder 
![Install dependencies]("screenshot/Screenshot 2025-09-05 at 13.23.03.png")

3 - Create and activate virtualenv
![venv]("screenshot/Screenshot 2025-09-05 at 13.03.32.png")

4- Install dependencies  and lint the code via  `make all` command from the `Makefile` 
![Install dependencies]("screenshot/Screenshot 2025-09-05 at 13.23.03.png")

5- build and run the app locally
Run the app locally to make sure it works.


6 - Create and deploy the web app
Run the `az webapp up` command to provision the App Service web app and do the first Manuel deployment to check if every it ok
![deploy the web app]("screenshot/Screenshot 2025-09-05 at 13.58.24.png")


* Successful deploy of the project in Azure Pipelines.  [Note the official documentation should be referred to and double checked as you setup CI/CD](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops).

7 -Running Azure App Service from Azure Pipelines automatic deployment

- Create your Azure Devvops Organization and create a project

* Connect your Azure DevOps project to your Azure subscription (From Project Settings, select Pipelines > Service connections)

- 

* Successful prediction from deployed flask app in Azure Cloud Shell.  [Use this file as a template for the deployed prediction](https://github.com/udacity/nd082-Azure-Cloud-DevOps-Starter-Code/blob/master/C2-AgileDevelopmentwithAzure/project/starter_files/flask-sklearn/make_predict_azure_app.sh).
The output should look similar to this:

* Prediction run against a working deployed Azure Application.
![deploy the web app]("screenshot/Screenshot 2025-09-05 at 14.21.55.png")

* Output of streamed log files from deployed application
![deploy the web app]("screenshot/Screenshot 2025-09-05 at 14.41.30.png")
 

## Enhancements

<TODO: A short description of how to improve the project in the future>

## Demo 

<TODO: Add link Screencast on YouTube>


