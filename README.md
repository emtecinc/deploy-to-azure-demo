# deploy-to-azure-demo

Click me
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Femtecinc%2Fdeploy-to-azure-demo%2Fmain%2Fazuredeploy.json)

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
| Azure Storage account  | storageaccfun | dedicatedly used for store function data |
| Azure Storage account | storageacc   | used as destination container to store blob files |

## Get the Topic Endpoint & Access key
Event Grid topic endpoint and Access key needs to integrate and copy value from:
#### Go to Event Grid topic (customertopic) -> Overview -> Topic Endpoint
<img width="875" alt="image" src="https://user-images.githubusercontent.com/126143091/224275190-13777a90-d852-4b6c-b0d6-0fabdc32eca6.png">

#### Go to Event Grid topic (customertopic) -> Settings -> Access Key -> Key1/Key2
<img width="956" alt="image" src="https://user-images.githubusercontent.com/126143091/224274360-064e147d-9917-4373-abd1-e161a0b33215.png">
