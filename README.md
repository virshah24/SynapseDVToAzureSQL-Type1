# SynapseDVToAzureSQL-Type1
This ADF template should help customers rapidly deploy Data Flow pipelines to help synchronize (Type-1) Synapse SQL Serverless with existing or new Azure SQL DB. 

# Overview
In November 2021 Microsoft announced deprecation of Data Export Service (DES); an add-on feature available via Microsoft AppSource which provides the ability to replicate data from Microsoft Dataverse to an Azure SQL store in a customer-owned Azure subscription. Data Export Service will continue to work and will be fully supported until it reaches end-of-support and end-of-life a year from this announcement date, in November 2022. Through this notice Microsoft allows customers sufficient time to plan and onboard to Azure Synapse Link for Dataverse which is a successor to Data Export Service.

# Problem Statement
However, customers who are already using Azure SQL DB in their current architecture heavily, and there are other dependencies or issues (code change, other Azure services integration with Azure SQL, performance etc.) adopting Azure Synapse Link for Dataverse leveraging SQL Serverless (Lake Database) are left without any choice at this time. This ADF template should help customers rapidly deploy Data Flow pipelines to help synchronize (Type-1) Synapse SQL Serverless with thier existing or new Azure SQL DB. 

![image](https://user-images.githubusercontent.com/45402166/169075709-9bcfee45-e0e5-4f4b-9176-a9d61f4ced64.png)
