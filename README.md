# Overview

Udacity Azure DevOps CI/CD Pipeline Project

## Project Plan
* https://trello.com/b/91hVTfGz/ci-cd-pipeline
* Spreadsheet is located in Document work card in Trello

## Instructions
* [Architectural Diagram](https://trello.com/c/adlRpLEp/12-architecture-diagram)

* Log in to Azure Portal and launch Azure Cloud Shell by clicking the shell icon at the top.

* Clone your repo into the shell by running git clone "URL"

* cd into your repo and deploy the webapp using the following command and adding your own ApplicationName <az webapp up -n ApplicationName>

* Once it's been successfully deploy access the URL https://ApplicationName.azurewebsites.net/ [screenshot](https://trello.com/c/Kg4ePvfC/7-deploy-flask-ml-api)

* Log in to [Azure DevOps](https://dev.azure.com/) to build a pipeline.

* Create a New Project then go to project settings and add a Service Connection

* Select Azure Resource Manager and make sure you select the correct Resource Group

* Now create a new pipeline linked to your GitHub account.

* Under Configure select Python to Linux Web App on Azure and run the pipeline

* After pipeline finish the build check if your website deployed successfully. [screenshot](https://trello.com/c/GsZPwFdb/5-build-a-azure-pipeline)

* Now everytime you make a change to your code the pipeline will execute.

* You can also lint and test your code using GitHub Actions. 

* Create a YAML file and add necesary steps to lint and test your code. 

* To test and lint your code you can create a Makefile that runs based of a requirements.txt file that has all the dependencies needed. [screenshot](https://trello.com/c/clOyJkVS/4-set-up-github-actions-to-build-and-test-code)

```bash
jonathan [ ~/ci-cd-pipeline ]$ ./make_predict_azure_app.sh 
Port: 443
Model not loaded
```
> 

## Enhancements

We can improve this project project by using a GitHub pipeline that way we centralize everything and don't have to work with multiple platforms.

## Demo 

https://youtu.be/p6PS7PHcAps


