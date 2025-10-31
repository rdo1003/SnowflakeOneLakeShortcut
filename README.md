# Fabric + Snowflake Power BI Copilot Demo 

## Overview

This demo showcases how to integrate Snowflake with Microsoft Fabric and leverage Power BI Copilot for conversational analytics and automated report generation.

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
- Create a free Snoflake trial or connect to an existing Snowflake instance
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


## Helpful Resources

- Tutorial: Configure a Microsoft Fabric Mirrored Database From Snowflake https://learn.microsoft.com/en-us/fabric/data-engineering/mirrored-database-snowflake
- Configure Snowflake for Single sign-on with Microsoft Entra ID https://learn.microsoft.com/en-us/entra/identity/sso/snowflake
- Use Snowflake with Iceberg tables in OneLake https://learn.microsoft.com/en-us/fabric/onelake/iceberg-tables
- Use Iceberg tables with OneLake https://learn.microsoft.com/en-us/fabric/onelake/iceberg-tables


## Demo Highlights

- Snowflake acts as the data warehouse.
- All transactional data resides in Snowflake.
- Fabric provides OneLake integration and semantic modeling.
- Power BI Copilot delivers AI-driven insights and reporting.
