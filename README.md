# week7-groupwork

# Synapse & ETL Project

### 1. Data Modeling Plan
Objective: Create a data model based on the use case

Steps:
* Gather requirements to know what data points are needed
* Design data model
* Define relationships

Final result:
Star schema with one fact table and five dimension tables, containing various data about municipalities in Finland

### 2. Create a shared Synapse Workspace
Objective: Set up a shared workspace in Azure Synapse Analytics

Steps:
* Create Synapse Workspace
* Ensure that everyone has appropriate access to workspace
* Set up SQL dedicated pool and Spark pool

### 3. Integrate GitHub version control
Objective: Use GitHub to track and manage changes in code and pipeline configurations

Steps:
* Create GitHub repository and invite collaborators
* Set up GitHub repository in Synapse Workspace
* Set up new branches for everyone's work

Final result:
Public repository to be able to use project as a "portfolio"

### 4. Design pipeline process
Objective: Design the ETL pipeline

Steps:
* Define how data needs to extracted from the source systems
* Transform data
* Load data to target system

Final result:
One dataset will be loaded using REST as source, other datasets loaded from source manually to Data Lake in CSV or .xls

### 5. Create pipeline(s)
Objective: Implement the ETL process as a pipeline

Steps:
* Create pipeline
* Add needed activities
* Test pipeline

Final result: 
Pipeline with 
* Own notebooks for all datasets to transform the data and load the data as tables to Data Lake
* Master notebook to combine tables to fact and dimension tables and load the new tables to Data Lake

### 6. Use loaded data in PowerBI to create a report
Objective: Use PowerBI to visualize and report

Steps:
* Connect PowerBI to Synapse
* Import data
* Build visualizations
* Create measures and calculations
* Publish report
