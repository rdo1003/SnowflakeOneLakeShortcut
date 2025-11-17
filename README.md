# Fabric + Snowflake Power BI Copilot Demo 

## Overview

The demo shows how to integrate Snowflake with Microsoft Fabric using a OneLake Shortcut so you can query Snowflake data in Fabric without copying it. It walks through creating the shortcut, enabling Iceberg/metadata virtualization where needed, then building a Fabric semantic model on top of that data. Then use Power BI Copilot to chat with the dataset and auto‑generate reports from the semantic model, illustrating conversational analytics on Snowflake‑hosted transactional data with minimal movement and fast time‑to‑insight.

**Demo Objectives**
- Connect Snowflake to Fabric using Shortcut.
- Create a semantic model in Fabric.
- Build Power BI Copilot reports to:
  - Chat with the data.
  - Generate reports from the semantic model.

**Architecture**
  
<img width="206" height="286" alt="image" src="https://github.com/user-attachments/assets/83e426be-b686-40e7-9cdf-2484627a9e16" />

- Snowflake: Serves as the data warehouse for transactional data.
- Microsoft Fabric: Hosts the semantic model and integrates with OneLake.
- Power BI Copilot: Enables natural language queries and report creation.

**Prerequisites**
- Create a free Snowflake trial or connect to an existing Snowflake instance
  <img width="595" height="347" alt="image" src="https://github.com/user-attachments/assets/92669297-eefc-47c0-8532-ff385f98df4f" />

- Ingest data into Snowflake -e.g. sample data -S&P500 Historical Stock Prices https://www.kaggle.com/datasets/camnugent/sandp500?resource=download
- Fabric Workspace Setting
  - Enable Delta Lake to Apache Iceberg table format virtualization (Preview) tenant setting via Fabric Admin Portal.
- Power BI Copilot enabled in the Fabric admin portal

## Step-by-Step Guide
1. Connect to Snowflake DB  -Follow "_Connect to your Snowflake instance in any cloud_" section from [Tutorial: Configure a Microsoft Fabric Mirrored Database From Snowflake](https://learn.microsoft.com/en-us/fabric/mirroring/snowflake-tutorial)
   ***Please note: The above tutorial is only referenced here for Snowflake Database connection details; we are not mirroring Snowflake***
    - Use a Shortcut in Fabric to link Snowflake.
3. Create Semantic Model
    - View your Iceberg tables in OneLake
      
        <img width="299" height="350" alt="image" src="https://github.com/user-attachments/assets/7f852a16-261d-4891-9b61-426ac2a3ce17" />

    - Build a structured model in Fabric for optimized reporting.
4. Build Power BI Copilot Reports
    - Use Copilot to chat with data and auto-generate reports.

## Connecting from PBI

<img width="704" height="473" alt="image" src="https://github.com/user-attachments/assets/6e0c9b8a-8e34-4d3e-873d-653223f9a334" />

- Select More... search for Snowflake
  
<img width="506" height="144" alt="image" src="https://github.com/user-attachments/assets/0d9887a8-ff7b-426c-9b5b-61a23416b6ea" />

- Enter your Snowflake Server name & Warehouse name (Snowflake Warehouse must be running)
<img width="519" height="199" alt="image" src="https://github.com/user-attachments/assets/32340258-5846-4d84-81b6-75671ca4a538" />


## Helpful Resources

- [Use Iceberg tables with OneLake](https://learn.microsoft.com/en-us/fabric/onelake/onelake-iceberg-tables#create-a-table-shortcut-to-an-iceberg-table)

- [Configure Snowflake for Single sign-on with Microsoft Entra ID](https://learn.microsoft.com/en-us/entra/identity/saas-apps/snowflake-tutorial) -optional



    ### Copilot & AI Features
    
    
    - [Copilot in Power BI Overview](https://learn.microsoft.com/en-us/power-bi/create-reports/copilot-introduction)
    
    - [Create Reports with Copilot](https://learn.microsoft.com/en-us/power-bi/create-reports/copilot-create-desktop-report)
    
    - [Copilot in Power BI Service - Summarize a report](https://learn.microsoft.com/en-us/power-bi/create-reports/copilot-pane-summarize-content)
    
    - [Copilot to create DAX](https://learn.microsoft.com/en-us/dax/dax-copilot?toc=%2Fpower-bi%2Fcreate-reports%2FTOC.json&bc=%2Fpower-bi%2Fcreate-reports%2Fbreadcrumb%2Ftoc.json)


## Demo Highlights

- Snowflake acts as the data warehouse.
- All transactional data resides in Snowflake.
- Fabric provides OneLake integration and semantic modeling.
- Power BI Copilot delivers AI-driven insights and reporting.
