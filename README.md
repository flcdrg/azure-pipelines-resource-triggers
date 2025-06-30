# Azure Pipelines resource triggers

Azure Pipelines resource triggers demo, with examples of [pipeline triggers](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/pipeline-triggers?view=azure-devops&WT.mc_id=DOP-MVP-5001655)

```mermaid
%%{init: {"flowchart": {"htmlLabels": true}} }%%
flowchart LR;
    A["<a href='https://dev.azure.com/gardiner/GitHub%20Builds/_build?definitionId=18'>main</a>
    <img src='https://dev.azure.com/gardiner/GitHub%20Builds/_apis/build/status%2FAzure%20Pipelines%20Resource%20Triggers%2Fflcdrg.azure-pipelines-resource-triggers-main?branchName=main' />"]
    B["<a href='https://dev.azure.com/gardiner/GitHub%20Builds/_build?definitionId=19'>trigger</a>
    <img src='https://dev.azure.com/gardiner/GitHub%20Builds/_apis/build/status%2FAzure%20Pipelines%20Resource%20Triggers%2Fflcdrg.azure-pipelines-resource-triggers-child?branchName=main'>
    "]
    C["<a href='https://dev.azure.com/gardiner/GitHub%20Builds/_build?definitionId=26'>trigger stage</a>
    <img src='https://dev.azure.com/gardiner/GitHub%20Builds/_apis/build/status%2FAzure%20Pipelines%20Resource%20Triggers%2Fflcdrg.azure-pipelines-resource-triggers-stage?branchName=main'>"]
    D["<a href='https://dev.azure.com/gardiner/GitHub%20Builds/_build?definitionId=21'>trigger params</a>
    <img src='https://dev.azure.com/gardiner/GitHub%20Builds/_apis/build/status%2FAzure%20Pipelines%20Resource%20Triggers%2Fflcdrg.azure-pipelines-resource-triggers-with-param?branchName=main'>"]
    E["<a href='https://dev.azure.com/gardiner/GitHub%20Builds/_build?definitionId=22'>trigger params default</a>
    <img src='https://dev.azure.com/gardiner/GitHub%20Builds/_apis/build/status%2FAzure%20Pipelines%20Resource%20Triggers%2Fflcdrg.azure-pipelines-resource-triggers-param-with-default?branchName=main'>"]
    F["<a href='https://dev.azure.com/gardiner/GitHub%20Builds/_build?definitionId=20'>double trigger</a>
    <img src='https://dev.azure.com/gardiner/GitHub%20Builds/_apis/build/status%2FAzure%20Pipelines%20Resource%20Triggers%2Fflcdrg.azure-pipelines-resource-double-trigger?branchName=main'>"]
    A-->B;
    A-->C;
    A-->D;
    A-->E;
    A-->F;
    B-->F;
    C-->F;

```
