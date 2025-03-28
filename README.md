# Descriptive Analysis of Vancity Bikeways Project
This phase presents an in-intensity descriptive analysis of the Vancity Bikeways dataset, specializing in visitors mild counts and their geographic distribution. The objective is to generate treasured insights for urban making plans, traffic management, and aid allocation.
Project Description:
The undertaking involves analysing traffic mild data throughout diverse geographical regions inside the Vancity Bikeways community. Using AWS offerings like Amazon S3, AWS Glue DataBrew, and Amazon Athena, the dataset is processed to discover high-traffic regions, traffic mild densities, and distribution patterns across exclusive zones. The findings may be used to improve site visitors control systems and tell future metropolis making plans selections.
Objective:
•	To identify areas with high traffic light density for better traffic management.
•	To classify traffic lights based on geographical zones and area types.
•	To establish a reliable framework for analyzing traffic patterns and urban planning.

Dataset:
The dataset comprises:
1.	Geo_Local_Area: Geographic region names (e.g., Downtown, West End, Kitsilano).
2.	Traffic_Light_Count: The number of traffic lighting according to geographical vicinity.
3.	Label: Classification of areas along with Residential, Commercial, and Industrial.
4.	Coordinates: Geographical reference factors (latitude and longitude).
Methodology:
1.	Data Collection:
o	Data sourced from the Vancity Bikeways dataset.
o	Uploaded to Amazon S3 (‘vancity-bikeways-raw-tarunjeet’).
2.	Data Cleaning & Profiling:
o	AWS Glue DataBrew: Used to clean the dataset, detect missing values, and standardize formats.
o	Transformation of data for accurate analysis.
o	Store cleaned data in Amazon S3 (‘vancity-bikeways-trf-tarunjeet’).
3.	Descriptive Analysis (Amazon Athena):
o	Analyzing traffic light counts per region.
o	Classifying data based on area types and monitoring trends.
o	Visualizing findings through pie charts, bar charts, and other graphical representations.

Tools & Technologies:
•	Amazon S3: Data storage and versioning.
•	AWS Glue DataBrew: Data cleaning, transformation, and profiling.
•	Amazon Athena: Querying data and performing statistical analysis.

Deliverables:
•	Cleaned datasets stored in Amazon S3.
•	Analysis report with detailed findings and visualizations.
•	Data documentation for future use.

Data Wrangling for Vancity Bikeways Project
This section outlines the process of cleaning, transforming, and consolidating the Vancity Bikeways dataset to ensure data accuracy, consistency, and usability.

Methodology:
1.	Data Ingestion (Amazon S3):
o	Data uploaded to Amazon S3 (‘vancity-bikeways-raw-tarunjeet’).
o	IAM roles and versioning enabled for security and rollback capabilities.
2.	Data Profiling (AWS Glue DataBrew):
o	Assessing completeness, accuracy, uniqueness, and consistency.
o	Identifying issues which include missing values, reproduction entries, and formatting errors.
3.	Data Cleaning & Transformation (AWS Glue DataBrew):
o	Removal of duplicates based on Geo_Local_Area and Coordinates.
o	Imputation of missing values using statistical methods.
o	Standardizing formats and correcting data inconsistencies.
o	Creating new attributes for enhanced analysis (e.g., Traffic Density).
o	Saving transformed data to Amazon S3 (‘vancity-bikeways-trf-tarunjeet’).
4.	Data Consolidation (AWS Glue & Amazon DynamoDB):
o	Structuring cleaned data into Amazon DynamoDB for efficient querying.
o	Schema includes attributes such as Geo_Local_Area, Traffic_Light_Count, Labels, Coordinates, and Timestamp.

Tools & Technologies:
•	Amazon S3: Data storage and management.
•	AWS Glue DataBrew: Data profiling, cleaning, and transformation.
•	Amazon DynamoDB: Structured data storage for efficient analysis.
•	IAM & KMS: Data security and access control.
•	Amazon Athena: Querying processed data.

Deliverables:
•	Cleaned and validated dataset stored in Amazon S3 and DynamoDB.
•	Data profiling and transformation reports.
•	Logs and documentation for tracking data quality.

Data Quality Control for Vancity Bikeways Project
This section outlines the framework for ensuring the quality, consistency, and reliability of the processed dataset. The DQC framework focuses on profiling, validating, and monitoring data integrity.

Methodology:
1.	Data Profiling:
o	Evaluating data for completeness, accuracy, and consistency.
o	Identifying and documenting quality issues.
2.	Data Validation:
o	Ensuring unique entries for geographical areas.
o	Checking numerical values and area type labels.
o	Validating data using Amazon Athena queries.
3.	Data Enrichment & Protection:
o	Consolidating data into Amazon DynamoDB.
o	Securing data through AWS KMS encryption and IAM policies.
o	Implementing version control for traceability.
4.	Monitoring & Reporting:
o	Monitoring data quality through Amazon CloudWatch and CloudTrail.
o	Generating logs for auditing purposes.
o	Creating dashboards for real-time tracking.
5.	Training & Documentation:
o	Creating guidelines for stakeholders to maintain data quality.
o	Ensuring best practices for data handling and governance.

Tools & Technologies:
•	AWS Glue DataBrew & Athena: Profiling and validation.
•	Amazon DynamoDB: Structured data storage.
•	Amazon CloudWatch & CloudTrail: Monitoring and logging.
•	IAM & KMS: Data security.

Deliverables:
•	Complete data quality metrics report.
•	Validated dataset ready for analysis.
•	Documentation of quality control procedures.

