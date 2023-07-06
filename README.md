# Azure Data Factory

## What us Azure Data Factory (ADF)?
- A cloud-based data integration service that allows you to orchestrate and automate data movement and data transformation
- Microsoft's main data engineering tool
- PaaS solution
- Data integration service
- Orchestration and automation
- Data transformation
- ETL vs ELT
  - ETL
    - Transform before loading
    - Designed for realibility
  - ELT
    - Transform after loading (on DW)
    - Designed for agility
## SSIS vs ADF
- ADF has event based trigge
  - For example, when a file is added to a blob storage
- ADF can run SSIS packages
## ADF Considerations
- Two versions
  - ADF v2 the current and improved version
- Build options
  - Portal
	- PowerShell
	- .NET
	- Python
	- REST
	- ARM
- Highly integrated
  - DevOps
  - Key Vault
  - Monitor
  - Automation
- Not a data storage  
## ADF Main Elements
- Activity: Copy, Move, Transform, etc.
- Pipeline: Logical grouping of activities - unit of work
- Integration Runtime: Computing infrastructure of ADF
- Trigger: Power switch
- Linked Service: Where data is? A connection to source, Blog Storage, SQL Server, etc.
- Dataset: Data to work with. File, SQL Table, etc.



