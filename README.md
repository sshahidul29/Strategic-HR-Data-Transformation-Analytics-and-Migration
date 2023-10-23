## Business Scenario: 
A leading e-commerce organization operating across multiple locations in Bangladesh is taking a proactive step to optimize its human resources management through the implementation of robust data analytics. The main goal is to establish an Enterprise Data Warehouse along with Data Mart Cubes. It comprises three distinct Business Processes, each with end-to-end design, development and Analysis.
#### Business Processes: 1. MisConduct Analysis, 2. Overtime Analysis and 3. Absent Analysis
## Achievement:
- Created a strong data warehouse for accessing data for business analysis purposes.
- The Human Resources Management team successfully understood how changes in a salesperson's marital status affected their overtime hours.
- Based on the analysis of employee misconduct data as part of their ongoing strategy, Human Resources Management was able to enhance work ethics and improve customer satisfaction.
## Software requirements:
- MS SQL Server, SSMS, SSIS, SSAS, and Visual Studio.
- Windows OS

## System Development Life Cycle (SDLC)
- Agile Kanban Methodology
## Enterprise Data Warehouse was built in MS SQL Server using SSMS
- Conducted in collaboration with Managers, Project Managers, Technical Product Managers, Clients, Subject-matter experts and Data Governance representatives to obtain requirements, objectives, and business rules for the project.
- Conducted data profiling.
- Created the opportunity/stakeholder Matrix (it helps identify which business groups should be invited to the collaborative design sessions for each process-centric row).
- Constructed a Bubble Chart for communicating data models to a non-technical audience. 
- Created Bus Matrix (composition of Business process, Granularity, Facts, Fact Tables, and Dimensions).
- Designed and implemented Enterprise Data Warehouse (EDW) using Ralph Kimball’s Dimensional Modelling Approach.
- Created and configured Staging, EDW, and Control Framework databases on MS SQL Server.
![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HREDW1.PNG)  

Figure 1: Enterprise Data Warehouse using Ralph Kimball’s Dimensional Modelling Approach.

## ETL Pipeline was built in Visual Studio using SSIS
- The project aimed to create an ETL (Extract, Transform, Load) pipeline for data extraction, transformation, and loading into SQL Server Databases from the flat file (CSV).
- Produced ETL Mapping and Transformation Rules and data Quality documentation for the project.
- Developed and tested ETL processes/programs necessary to extract data from different data sources, Transformed and cleansed the data, and loaded it into a Staging database and Staging to Data Warehouse, using connection managers like OLE DB, Excel, Flat file, and ADO.NET.
- Created a metric table for an audit of Source Count, and Destination Count Staging database, and Pre, Current, Post, Type1, and Type2 Counts for EDW using the Control framework database.
- Design and Implement Ralph Kimball slowly changing dimension (SCD) Type 1 and 2.
- Troubleshooting and root cause analysis activities to fix bugs in the data integration process.
- Used the server agent to automate the ETL processes to ensure new data were loaded automatically into the Data Warehouse.
![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HRETL3.PNG)  

 Figure 2: Control-flow diagram for ETL Pipeline from flat file source to Staging database

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HRETL4.PNG)  

 Figure 3: Data-flow diagram of ETL Pipeline from flat file source to Staging Misconduct table

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HRETL2.PNG)  

Figure 4: Data-flow diagram for Incremental load of ETL Pipeline from flat file source to Staging Misconduct Analysis table

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HRETL1.PNG)  

Figure 5: Data-flow diagram for Incremental load of ETL Pipeline EDW FactAbsent Analysis table

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/Control.PNG)  

Figure 6: Control-flow diagram for ETL Pipeline to automate the system through SQL Server Agent

## Datamart was built using SSAS for Business Users

- Cubes were built using SQL Server Analysis Services (SSAS) for multi-dimensional and Tabular analysis for business users. These cubes support interactive dashboards and data visualizations for informed decision-making.

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/OverM.PNG)  

Figure 7: Overtime Cube for Multidimensional Analysis

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/OverT.PNG)  

Figure 8: Overtime Cube for Tabular Analysis

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/MisM.PNG)  

Figure 9: Misconduct Cube for Multidimensional Analysis

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/MisT.PNG)  

Figure 10: Misconduct Cube for Tabular Analysis

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/AbsM.PNG)  

Figure 11: Absent Cube for Multidimensional Analysis

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/AbsT.PNG)  

Figure 12: Absent Cube for Tabular Analysis
