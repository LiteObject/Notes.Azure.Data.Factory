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
- Integration Runtime: Compute infrastructure that executes the activities within a pipeline
- Trigger: Power switch
- Linked Service: Where data is? A connection to source, Blog Storage, SQL Server, Amazon S3, Salesforce, etc.
- Dataset: data structures or files that are ingested or processed by Azure Data Factory, such as tables, blobs, or files.
## Activities & Pipelines
- Three types of activities:
  - Data Movement
  - Data Transformation
  - Data Control
## Integration Runtimes
- Data Flow execution
- Data Movement execution
- Dispatch of Activities
- SSIS Package execution
## Linked Services and Datasets
- Linked Services are like connection strings
- Two types:
  - Data Stores
  - External Compute 
- Datasets are about data structure
  - SQL Database/Table
  - Blob Storage/File
## Triggers
- Schedule: Periodic, forward looking only (next schedule time), runs on dates configured, fire and forget 
- Tumbling Window: Time-sliced - run every X number of hours, supports backfill, runs at fixed interval, retry, concurrency, system variables
- Event-based: Fired on Blob creation or deletion
## Copy Activity
- More than just copy - serialization, compression, column mapping
- 83 connectors and counting
- 6 different formats
- Enterprise features - incremental copy, resume from last failed run, etc.
