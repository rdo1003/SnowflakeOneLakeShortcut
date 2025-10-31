# Fabric + Snowflake Power BI Copilot Demo 

## Overview

This demo showcases how to integrate Snowflake with Microsoft Fabric (via shortcut) and leverage Power BI Copilot for conversational analytics and automated report generation.

**Demo Objectives**
- Connect Snowflake to Fabric using Shortcut.
- Create a semantic model in Fabric.
- Build Power BI Copilot reports to:
  - Chat with the data.
  - Generate reports from the semantic model.

**Architecture**
- Snowflake: Serves as the data warehouse for transactional data.
- Microsoft Fabric: Hosts the semantic model and integrates with OneLake.
- Power BI Copilot: Enables natural language queries and report creation.

**Prerequisites**
- Create a free Snowflake trial or connect to an existing Snowflake instance
  <img width="595" height="347" alt="image" src="https://github.com/user-attachments/assets/92669297-eefc-47c0-8532-ff385f98df4f" />

- Sample Data -S&P500 Historical Stock Prices
  - https://www.kaggle.com/datasets/camnugent/sandp500?resource=download
- Fabric Workspace Setting
  - Enable Delta Lake to Apache Iceberg table format virtualization (Preview) in OneLake.


## Step-by-Step Guide
1. Connect to Snowflake DB
    - Use a Shortcut in Fabric to link Snowflake.
2. Create Semantic Model
    - Build a structured model in Fabric for optimized reporting.
3. Build Power BI Copilot Reports
    - Use Copilot to chat with data and auto-generate reports.

## Connecting from PBI

<img width="704" height="473" alt="image" src="https://github.com/user-attachments/assets/6e0c9b8a-8e34-4d3e-873d-653223f9a334" />

- Select More... search for Snowflake
  
<img width="506" height="144" alt="image" src="https://github.com/user-attachments/assets/0d9887a8-ff7b-426c-9b5b-61a23416b6ea" />

- Enter your Snowflake Server name & Warehouse name (Snowflake Warehouse must be running)
<img width="519" height="199" alt="image" src="https://github.com/user-attachments/assets/32340258-5846-4d84-81b6-75671ca4a538" />


## Helpful Resources

- [Configure Snowflake for Single sign-on with Microsoft Entra ID](#https://learn.microsoft.com/en-us/entra/identity/sso/snowflake)
  
- [Use Iceberg tables with OneLake](#https://learn.microsoft.com/en-us/fabric/onelake/onelake-iceberg-tables#create-a-table-shortcut-to-an-iceberg-table)


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
