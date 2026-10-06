# Data Architecture Blueprint

Here is the high-level data flow for the RetailMart Azure Data Engineering project:

```mermaid
graph TD
    A[Raw CSV Data] -->|Ingest| B(Azure Data Factory)
    B -->|Load| C[(ADLS Gen2 - Bronze)]
    C -->|Read| D[Azure Databricks]
    D -->|Clean & Format| E[(ADLS Gen2 - Silver)]
    E -->|Star Schema| F[(ADLS Gen2 - Gold)]
    F -->|Serve| G[Azure SQL Database]
    G -->|Analytics| H[Power BI]
