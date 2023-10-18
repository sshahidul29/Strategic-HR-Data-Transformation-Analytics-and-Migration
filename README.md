# Business Scenario: 
A leading e-commerce organization operating across multiple locations in Bangladesh is taking a proactive step to optimize its human resources management through the implementation of robust data analytics. The main goal is to establish an Enterprise Data Warehouse along with Data Mart Cubes. It comprises three distinct Business Processes, each with end-to-end design, development and Analysis.
#### Business Processes: 1. MisConduct Analysis, 2. Overtime Analysis and 3. Absent Analysis 
## Enterprise Data Warehouse was built in MSSQL Server using SSMS

- Designed and implemented Enterprise Data Warehouse (EDW) using Ralph Kimball’s Dimensional Modelling Approach.
- Created and configured Staging, EDW, and Control Framework databases on MS SQL Server. 

![HR](https://github.com/sshahidul29/Strategic-HR-Data-Transformation-Analytics-and-Migration/blob/main/Fugure/HREDW1.PNG)  

Figure 1: Enterprise Data Warehouse using Ralph Kimball’s Dimensional Modelling Approach.

## ETL Pipeline was built in Visual Studio using SSIS

- The project aimed to create an ETL (Extract, Transform, Load) pipeline for data extraction, transformation, and loading into SQL Server Databases from the flat file (CSV).
- Designed SQL Server Integration Service (SSIS) packages and wrote T-SQL scripts for extraction, transformation, and loading (ETL) of data from flat file (CSV) to a staging area and subsequently to the data warehouse.
- Created a metric table for an audit of Source Count, Pre-Count, Destination Count, and Post Count for ODS, Source Count, and Destination Count Staging database, and Pre, Current, Post, Type1, and Type2 Counts for EDW using the Control framework database.
- Implemented server agent for automated data loading and scheduling.
  
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
