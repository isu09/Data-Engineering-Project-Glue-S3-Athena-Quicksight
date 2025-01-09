# Project: End-to-End Data Engineering Pipeline for Spotify

## Overview:
Developed an end-to-end data pipeline for Spotify's data processing and analytics using AWS services. The pipeline ingests, transforms, and stores data for querying and visualization to derive business insights.

## Key Responsibilities & Achievements:

### Data Ingestion & Staging Layer:
- Managed the ingestion of raw data into the staging layer for further processing, ensuring data was properly stored in Amazon S3.

### ETL Pipeline with AWS Glue:
- Built a robust ETL pipeline using AWS Glue to transform the data from the staging layer and move it to a data warehouse (S3 DW).
- Utilized AWS Glue to automate data extraction, transformation, and loading tasks, streamlining the data flow.

### Glue Crawler for Data Cataloging:
- Configured AWS Glue Crawlers to automatically discover and catalog datasets, creating databases and populating tables for query processing.

### Data Querying with AWS Athena:
- Leveraged AWS Athena to run SQL queries on the data stored in S3, enabling efficient ad-hoc querying without needing to move the data.

### Data Visualization with AWS QuickSight:
- Utilized AWS QuickSight to create interactive dashboards and visualizations, providing actionable business insights based on the queried data.

## Technologies Used:
- **AWS Glue:** Automated ETL processes and data transformation.
- **AWS Athena:** Enabled fast, serverless querying of data stored in Amazon S3.
- **AWS QuickSight:** Visualized data and provided business insights.
- **Amazon S3:** Stored raw and transformed datasets.
- **AWS Glue Crawlers:** Automated schema discovery and cataloging of datasets.

## Results:
- **Efficient Data Pipeline:** Streamlined end-to-end data processing and storage with AWS Glue and Athena.
- **Actionable Insights:** Provided business insights through visualizations in AWS QuickSight, enabling better decision-making.



#STEPS: Data-Engineering-Project-Glue-S3-Athena-Quicksight


![image](https://github.com/user-attachments/assets/f90b3b64-0dd4-4d8c-b6b1-b65393bb44a1)

DataSet used in the Project - Spotify Dataset 2023  -Kaagle Link :Raw Data- https://shorturl.at/qBUX5 - The cleansed data is attached as Three CSV file. 

track.csv.

albums.csv (zipped) - unzip.

artist.csv.

AWS Cloud - IAM - create IAM User - Attach Permission- ACCESS S3 FULL ACCESS - GLUE FULL ACCESS - ATHENA FULL ACCESS - QUICKSIGHT FULL ACCESS.

AWS S3 - CREATE Bucket - unique Name.
         Folder - staging/  , datawarehouse/
         ![image](https://github.com/user-attachments/assets/c374ff5a-5d4e-4f66-b2a6-3fca44b44752)


        Upload Files to S3 staging/
        ![image](https://github.com/user-attachments/assets/74cc3032-9aca-4603-a484-11b7e886bdb9)


AWS Glue - moving data from staging layer to dataware house in S3 using Glue ETL.

           Use Visual ETL IN Glue - so Dragged and Dropped the source and Destination and EXTRACT TRANSFORM AND LOAD Done Visually.
           ![image](https://github.com/user-attachments/assets/0c675027-1b2e-43f2-86ec-d6e6c81d2847)
           
           ![image](https://github.com/user-attachments/assets/7d13a0ef-52ec-4d28-9dd4-05ae9ae3968b)

AWS Glue - create Crawler - to infer the Schema from S3 - IAM role to access S3 (already created). Glue Database should be created.

           So, create Glue Database- spotify.

           Now can select Database during Crawler creation.

Automatic Glue Table is created by inferring Schema from S3
![image](https://github.com/user-attachments/assets/7fcac141-de8d-4817-aa5b-bc593980d2de)

AWS Athena- can write simple query on top of S3.

Launch Notebook edition - Select Data source as S3 Catalog and Database .

Inorder to run query in Athena, we need to create Bucket(output) to store the result of Athena Query.


![image](https://github.com/user-attachments/assets/0eea5069-5716-4934-8ac4-8884904f6a2a)

We can see the output in S3 Bucket of Athena.

![image](https://github.com/user-attachments/assets/7d53be66-d648-401f-bebe-3c6bed1fff79)

Quicksight - Visualization - can visualize the Data.

Signup in Quicksight.

Allow access to Service.

Create Datasets in Quicksight.

Select Source as-Athena-in Quicksight- we can visualize - hit and publish to the customer.

![image](https://github.com/user-attachments/assets/8dfe614b-b4b9-4b04-bd3c-c7df7a772890)











                          

                          










           







