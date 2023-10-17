# Business Scenario: 
A leading e-commerce organization operating across multiple locations in Bangladesh is taking a proactive step to optimize its human resources management through the implementation of robust data analytics. The main goal is to establish an Enterprise Data Warehouse along with Data Mart Cubes.
## Enterprise Data Warehouse was built in MSSQL Server using SSMS
- Led complete database lifecycle management including installation, upgrade, troubleshooting, migration, and security.
- Conducted stakeholder analysis and requirements gathering sessions, aligning data with business needs.
- Created Bus Matrix (composition of Business process, Granularity, Facts, Fact Tables, and Dimensions).
- Designed and implemented Enterprise Data Warehouse (EDW) using Ralph Kimball’s Dimensional Modelling Approach.
- Created and configured Staging, EDW, and Control Framework databases on MS SQL Server. 

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HREDW1.PNG)  

Figure 2: Enterprise Data Warehouse using Ralph Kimball’s Dimensional Modelling Approach.

## ETL Pipeline was built in Visual Studio using SSIS

- The project aimed to create an ETL (Extract, Transform, Load) pipeline for data extraction, transformation, and loading into SQL Server Databases from the flat-file (CSV) and OLDBE sources.
- Designed SQL Server Integration Service (SSIS) packages and wrote T-SQL scripts for extraction, transformation, and loading (ETL) of data from different data sources to ODS, ODS to a staging area and subsequently to the data warehouse.
- Created a metric table for an audit of Source Count, Pre-Count, Destination Count, and Post Count for ODS, Source Count, and Destination Count Staging database, and Pre, Current, Post, Type1, and Type2 Counts for EDW using the Control framework database.
- Implemented server agent for automated data loading and scheduling.
  
![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HREDW.PNG)  

 Figure 3: Control-flow diagram for ETL Pipeline from flat file source to ODS

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HREDW.PNG)  

 Figure 4: Data-flow diagram of ETL Pipeline from flat file source to ODS Product table

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HREDW.PNG)  

Figure 5: Data-flow diagram for Incremental load of ETL Pipeline from flat file source to ODS Purchase transactions table

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HREDW.PNG)  

 Figure 6: Control-flow diagram for ETL Pipeline for EDW

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HREDW.PNG)  

 Figure 7: Data-flow diagram of ETL Pipeline for EDW Dimension table

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HREDW.PNG)   

Figure 8: Data-flow diagram for Incremental load of ETL Pipeline EDW Fact table

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HREDW.PNG)  

Figure 9: Control-flow diagram for ETL Pipeline to automate the system through SQL Server Agent

## Datamart was built using SSAS for Business Users

- Cubes were built using SQL Server Analysis Services (SSAS) for multi-dimensional and Tabular analysis for business users. These cubes supported interactive dashboards and data visualizations for informed decision-making.

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HREDW.PNG)  

Figure 10: Purchase Cube for Multidimensional Analysis
