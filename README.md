# Data subcription deployment

There are two ways for deployment:
### 1. ARM template

**Click me** (use CTRL+Click for new tab)

[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Femtecinc%2Fdeploy-to-azure-demo%2Fmain%2Fazuredeploy.json)


### 2. Powershell script

To download the script, find the file with name "bloomberg-infra.ps1" in same repo. 

Run this script in powershell. (**note-** please make sure script file and zipdeploy_content.zip file should present in same folder.)

## Overview
This sample deploys an Azure Functions app with an Event Grid trigger to act as a webhook within the vnet-subnet integration. 

## Resources
All default_name of resources **can be modified** and also must be **unique**. 

| resources | default_name | Comment |
| :----- | :--- | :--- |
| Event Grid topic | customertopic |   |
| Function App plan | funappplan |   |
| Virtual network (Subnet) | vnet-test (function) | Subnet Name i.e function is fix  |
| Azure Functions app (function) | test-functionapp (CopyBlobFile) | function name i.e CopyBlobFile is fix  |
| Azure Storage account  | storageaccfun | dedicatedly used for function related data |
| Azure Storage account | storageacc   | used as destination container to store blob files |

