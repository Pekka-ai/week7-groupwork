# week7-groupwork

# Synapse & ETL Project 🔎📊

### 1. Data Modeling Plan
**🎯 Objective:** Create a data model based on the use case

**📍 Steps:**
* Gather requirements to know what data points are needed
* Design data model
* Define relationships

**🌟 Final result:**
Star schema with one fact table and five dimension tables, containing various data about municipalities in Finland

![image](https://github.com/user-attachments/assets/967ab18f-005e-47ac-bdd8-9032355f14c4)


### 2. Create a shared Synapse Workspace
**🎯 Objective:** Set up a shared workspace in Azure Synapse Analytics

**📍 Steps:**
* Create Synapse Workspace
* Ensure that everyone has appropriate access to workspace
* Set up SQL dedicated pool and Spark pool

**🌟 Final result:**
Shared Synapse Workspace for the team, including Data Lake, SQL Dedicated Pool and Spark Pool

### 3. Integrate GitHub version control
**🎯 Objective:** Use GitHub to track and manage changes in code and pipeline configurations

**📍 Steps:**
* Create GitHub repository and invite collaborators
* Set up GitHub repository in Synapse Workspace
* Set up new branches for everyone's work

**🌟 Final result:**
Public repository to be able to use project as a "portfolio"

### 4. Design pipeline process
**🎯 Objective:** Design the ETL pipeline

**📍 Steps:**
* Define how data needs to extracted from the source systems
* Transform data
* Load data to target system

**🌟 Final result:**
One dataset will be loaded using REST as source, other datasets loaded from source manually to Data Lake in CSV or .xls. Everyone works on their dedicated dataset individually and they'll be combined after.

### 5. Create pipeline(s)
**🎯 Objective:** Implement the ETL process as a pipeline

**📍 Steps:**
* Create pipeline
* Add needed activities
* Test pipeline

**🌟 Final result:**  
🔄️ Pipeline with 
* Execution of another pipeline, that includes a copy data activity to sink Paavo-dataset from a REST API source to Data Lake and a notebook to transform the data
* Notebooks for all the other datasets to transform the data and load the data as tables to Data Lake
* Master notebook to merge previously loaded tables to fact and dimension tables and load the new tables to Data Lake
* Copy data activities to sink the resulting tables from Data Lake to Data Warehouse (SQL Dedicated Pool)

![image](https://github.com/user-attachments/assets/a504b5a7-6ecb-47ff-ba40-ac5db3938dc7)


### 6. Use loaded data in Power BI to create a report
**🎯 Objective:** Use Power BI to visualize and report

**📍 Steps:**
* Connect Power BI to Synapse
* Import data
* Build visualizations
* Create measures and calculations
* Publish report
* Create app

**🌟 Final result:**
Power BI report with a simple dashboard on basic data about municipalities, e.g, amount of residents, incomes etc and multiple pages with e.g. correlations
