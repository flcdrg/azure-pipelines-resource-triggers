# Azure Pipelines resource triggers

Azure Pipelines resource triggers demo, with examples of [pipeline triggers](https://learn.microsoft.com/en-us/azure/devops/pipelines/process/pipeline-triggers?view=azure-devops&WT.mc_id=DOP-MVP-5001655)

```mermaid
%%{init: {"flowchart": {"htmlLabels": true}} }%%
flowchart LR;
    A["<a href='https://dev.azure.com/gardiner/GitHub%20Builds/_build?definitionId=18'>main</a>"]
    B["<a href='https://dev.azure.com/gardiner/GitHub%20Builds/_build?definitionId=19'>trigger</a>"]
    C["<a href='https://dev.azure.com/gardiner/GitHub%20Builds/_build?definitionId=26'>trigger stage</a>"]
    D["<a href='https://dev.azure.com/gardiner/GitHub%20Builds/_build?definitionId=21'>trigger params</a>"]
    E["<a href='https://dev.azure.com/gardiner/GitHub%20Builds/_build?definitionId=22'>trigger params default</a>"]
    F["<a href='https://dev.azure.com/gardiner/GitHub%20Builds/_build?definitionId=20'>double trigger</a>"]
    A-->B;
    A-->C;
    A-->D;
    A-->E;
    A-->F;
    B-->F;
    C-->F;

```

* [![Build Status](https://dev.azure.com/gardiner/GitHub%20Builds/_apis/build/status%2FAzure%20Pipelines%20Resource%20Triggers%2Fflcdrg.azure-pipelines-resource-double-trigger?branchName=main)](https://dev.azure.com/gardiner/GitHub%20Builds/_build/latest?definitionId=20&branchName=main)