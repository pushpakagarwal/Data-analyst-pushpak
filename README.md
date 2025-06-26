# Data-analyst-pushpak
Project: Capital Project Budget Analysis on AWS (2025)
This project has built and implemented a complete-stack Data Analytics Platform (DAP) to study a multi-year capital budget demand with the Amazon Web Services cloud environment. It was mainly targeting to derive insights out of the data on public project funds and also utilized the secure and scalable Amazon Web Services to ingest, transform, catalog, query, and govern data.
Pipelines Implemented:
Pipeline 1: Data Ingestion Pushed the raw Excel data to an S3 bucket called capital-projects-raw-pushpak in a defined folder path hierarchy (year, quarter and server).
Pipeline 2: Profiling of Data With the 20 columns and 740 rows, a schema, missing values, and data type analysis on the 20 columns with 740 rows were generated with correlation matrices and data type summaries at AWS Glue DataBrew.
Pipeline 3: Data Cleaning Applied transformations including null filtering, added categorical format (lowercasings) and converted budget value type. The clean data was re-exported back to the same S3 bucket to minimize costs as CSV and Parquet formatted.
Pipeline 4: Data Cataloging AWS Glue Crawler was set to catalog the cleaned data into the Glue Data Catalog as capital_project_db database such that downstream analytics could be done on Athena. SQL Analysis. 
Pipeline 5: SQL queries assessing budget demands according to the year and type of project and amount were written with the help of Amazon Athena. The findings were employed to settle the order of prioritization of funding by the type of service.
Pipeline 6: DAP estimated cost The estimated monthly price of each stage was calculated with the help of AWS Pricing Calculator in the following way: ingestion (0.01), profiling & cleaning (2.44), cataloging (0.41), summarization (10.41).
Pipeline 7: Security of Data Versioning and default encryption with AWS KMS in S3 bucket have been installed to afford secure storage of critical datasets and rollback protection. Data Governance Stage
Pipeline 8: An ETL job of AWS Glue was created to pass high-quality and low-quality records based on data validation rules and direct them into each folder (Passed/Failed) in a container with quality checks.
Pipeline 9: Watching The features of CloudWatch and Glue jobs monitoring were applied to observe ETL execution statuses, loading times, and logging results in order to be used in the future in audit work and optimize them.
![image](https://github.com/user-attachments/assets/3f64d1bc-a109-4314-8fcc-a961f464b95a)
![image](https://github.com/user-attachments/assets/306bf15d-51d3-4f2c-a313-c335251afedf)
![image](https://github.com/user-attachments/assets/e136221d-5b5b-4712-bb75-d94fb5897905)
![image](https://github.com/user-attachments/assets/8b682c31-c139-48a4-8887-78bdc62b09b3)
![image](https://github.com/user-attachments/assets/d7a00676-b2bb-4d30-9efa-ee189b8f6e10)
![image](https://github.com/user-attachments/assets/7ad0ab2f-3341-4ef6-82b9-5e459e9570de)
Although this is a curated version of the dataset, I saved it under the same raw dataset folder path in the S3 bucket to maintain cost-effectiveness and simplify access permissions. Proper labelling and folder structuring were maintained to ensure clarity between raw and transformed data.
![image](https://github.com/user-attachments/assets/129e8604-5866-4cfe-9b5e-8b8c2785bd57)
![image](https://github.com/user-attachments/assets/29d5d6fa-159c-4db2-a961-702ddd8e89dd)
![image](https://github.com/user-attachments/assets/500b370b-711f-4bb0-bf5a-437b23a43e6d)
![10](https://github.com/user-attachments/assets/c6999219-93a4-4dae-8c05-7a73a199a2bd)
![image](https://github.com/user-attachments/assets/75d56a0d-7af7-4629-9a92-030055594f95)
![image](https://github.com/user-attachments/assets/094a9c93-fcc3-4399-b25c-35ab21c2d2db)
![image](https://github.com/user-attachments/assets/cba6e410-7c44-4c2b-abb1-f733bb00cb62)
![image](https://github.com/user-attachments/assets/98100ec4-3b2f-4712-afd1-b8184285251b)
![image](https://github.com/user-attachments/assets/fb9c3cbd-ac5c-48a8-8ba9-73e0221cdcbc)
![image](https://github.com/user-attachments/assets/4f0dc7af-adf8-40d5-817b-75b014515112)


