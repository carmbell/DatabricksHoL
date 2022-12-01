# Module 00 - Lab Environment Setup

**[Home](../README.md)** - [Next Module >](../Modules/module01.md)

## :loudspeaker: Introduction

In order to follow along with the Azure Databricks lab exercises, you need to provision a set of resources.

## :thinking: Prerequisites

* An [Azure account](https://azure.microsoft.com/free/) with an active subscription.
* Owner permissions within a Resource Group to create resources and manage role assignments.

    
## :test_tube: Lab Environment Setup

1. Right-click or `Ctrl + click` the button below to open the Azure Portal in a new window.

    [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Ftayganr%2Fpurviewlab%2Fmain%2Ftemplate%2Fazuredeploy.json)

2. Beneath the **Resource group** field, click **Create new** and provide a unique name (e.g. `databricks-rg`), then provide a unique Workspace Name (e.g. `DatabricksHoL`), select a [valid location](https://azure.microsoft.com/global-infrastructure/services/?products=purview&regions=all) (e.g. `East US 2`), select the Trail Pricing Tier, and then click **Review + create**.

    ![Deploy Template](../Images/module00/DbAzureDeploy.png)

3. Once the validation has passed, click **Create**.

    ![Create Resources](../images/module00/00.02-deploy-create.png)



## :tada: Summary

By successfully deploying the Microsoft Purview lab template, you have the Azure resources needed to follow along with the learning exercises.

[Continue >](../modules/module01.md)
