# SynapseDVToAzureSQL-Type1
This ADF template should help customers rapidly deploy Data Flow pipelines to help synchronize (Type-1) Synapse SQL Serverless with existing or new Azure SQL DB. 

# Overview
In November 2021 Microsoft announced deprecation of Data Export Service (DES); an add-on feature available via Microsoft AppSource which provides the ability to replicate data from Microsoft Dataverse to an Azure SQL store in a customer-owned Azure subscription. Data Export Service will continue to work and will be fully supported until it reaches end-of-support and end-of-life a year from this announcement date, in November 2022. Through this notice Microsoft allows customers sufficient time to plan and onboard to Azure Synapse Link for Dataverse which is a successor to Data Export Service.

# Problem Statement
However, customers who are already using Azure SQL DB in their current architecture heavily, and there are other dependencies or issues (code change, other Azure services integration with Azure SQL, performance etc.) adopting Azure Synapse Link for Dataverse leveraging SQL Serverless (Lake Database) are left without any choice at this time. This ADF template should help customers rapidly deploy Data Flow pipelines to help synchronize (Type-1) Synapse SQL Serverless with thier existing or new Azure SQL DB. 

![image](https://user-images.githubusercontent.com/45402166/169075709-9bcfee45-e0e5-4f4b-9176-a9d61f4ced64.png)

# How to deploy?

Prerequisites:
  - Power Platform environment with Synapse Link for Dataverse entities established with Azure Synapse workspace Lake Database
  - Requires Dataverse Entities to be synchronize with in-place update (default) settings.
  - Synapse (or ADF) Linked Services for:
      - Dataverse linked Lake Database (source) and
      - Azure SQL DB (target) 
  - Download *.zip Synapse Pipeline (ADF) template file from the GitHub link provided on this page to local system. Note: it contains Manifest and pipeline template *.json files
  - Import the *.zip template from Integrate -> Import from pipeline template feature of Synapse Pipeline (or ADF)
![image](https://user-images.githubusercontent.com/45402166/169075976-1c8bb3da-4577-41b4-9f06-c905b4ef62bf.png)

