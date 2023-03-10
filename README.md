# deploy-to-azure-demo

Click me
[![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Femtecinc%2Fdeploy-to-azure-demo%2Fmain%2Fazuredeploy.json)

This sample deploys an Azure Functions app with an Event Grid trigger to act as a webhook.

This template creates,

| resources | default_name | 
| :----- | :--- |
| Event Grid topic | customertopic | 
| Function App plan | funappplan | 
| Virtual network -- subnet | vnet-test -- function | 
| Azure Functions app -- function | test-functionapp -- CopyBlobFile | 
| Azure Storage account  | storageaccfun |
| Azure Storage account | storageacc   |

above default_name of resources can be modified and also should be unique. Event Grid topic endpoint and Access key needs to integrate and below is path to copy value from:

#### Go to Event Grid topic (customertopic) -> Overview -> Topic Endpoint
<img width="875" alt="image" src="https://user-images.githubusercontent.com/126143091/224275190-13777a90-d852-4b6c-b0d6-0fabdc32eca6.png">

#### Go to Event Grid topic (customertopic) -> Settings -> Access Key -> Key1/Key2
<img width="956" alt="image" src="https://user-images.githubusercontent.com/126143091/224274360-064e147d-9917-4373-abd1-e161a0b33215.png">
