# Smart-Hotel-Booking-Analytics-Platform-Using-Apache-Big-Data-Technologies
# Phase 1: Environment Setup

In this phase, the Hadoop ecosystem was successfully initialized.

Completed tasks:
- Started HDFS services (NameNode, DataNode, SecondaryNameNode).
- Started YARN services (ResourceManager and NodeManager).
- Verified all Hadoop services using the JPS command.
- Verified Apache Flume installation.
- Confirmed Java environment configuration.

This environment will be used for data ingestion and analytics in the following phases.
# <img width="741" height="371" alt="image" src="https://github.com/user-attachments/assets/f5851f5d-44da-423f-ad28-27e5769f109f" />
# <img width="697" height="581" alt="image" src="https://github.com/user-attachments/assets/90e6452a-4d8b-486d-973d-797fa6f38315" />
# Phase 2: Data Ingestion using Apache Flume

## Objective
Transfer the hotel booking dataset from the local file system to Hadoop HDFS using Apache Flume.

## Steps
1. Created a spool directory.
2. Copied the dataset into the spool directory.
3. Configured Apache Flume using a Spooling Directory Source.
4. Configured HDFS Sink.
5. Started the Flume Agent.
6. Successfully transferred the dataset into HDFS.

## Technologies
- Apache Flume 1.7.0
- Hadoop HDFS
- Java 8

## Output



Dataset stored in:

/hotel_project/input


<img width="1184" height="270" alt="image" src="https://github.com/user-attachments/assets/4a8d95db-adf0-4799-b292-c2552e35a2b2" />
<img width="1191" height="47" alt="image" src="https://github.com/user-attachments/assets/db022a8f-ff4d-413d-98df-12e1bb75b8a2" />
<img width="745" height="94" alt="image" src="https://github.com/user-attachments/assets/39b8e050-3f73-4bb4-b11c-f8e49741682f" />
<img width="712" height="426" alt="image" src="https://github.com/user-attachments/assets/c4e984ce-7324-4a85-b49e-a9f38dc8dc57" />


The dataset is now available inside Hadoop HDFS and ready for Spark ETL processing.


# Phase 3: Spark ETL & Data Cleaning

## Objective
Clean and transform the hotel booking dataset using Apache Spark before loading it into Hive.

## Technologies
- Apache Spark 3.0.1
- Hadoop HDFS
- Jupyter Notebook

## ETL Steps

1. Read the dataset from HDFS.
2. Explore the dataset.
3. Handle missing values.
4. Remove duplicate records.
5. Create new calculated columns:
   - total_nights
   - total_guests
   - total_stay_cost
6. Save the cleaned dataset back into HDFS.

## Output

The cleaned dataset was successfully saved in:

/hotel_project/cleaned_data_final

<img width="1135" height="612" alt="image" src="https://github.com/user-attachments/assets/7662f9c5-97aa-469f-8d30-aa29408539b4" />
<img width="1140" height="576" alt="image" src="https://github.com/user-attachments/assets/d54ca82a-6726-412f-bbe1-079ac8ad1498" />
<img width="1127" height="462" alt="image" src="https://github.com/user-attachments/assets/ad11d38c-ad40-4ee3-8807-69eb359d0aee" />
<img width="1135" height="569" alt="image" src="https://github.com/user-attachments/assets/0660cf01-506b-42e6-ab63-3773d3a09bca" />
<img width="1141" height="568" alt="image" src="https://github.com/user-attachments/assets/20c5b93a-01ff-46ee-a554-c34b7d797426" />
<img width="1101" height="377" alt="image" src="https://github.com/user-attachments/assets/023deb1a-3a78-4bcb-a00c-0ad1032bca6b" />
<img width="834" height="127" alt="image" src="https://github.com/user-attachments/assets/8c5982a7-9185-4ff1-b769-fbab5e5be14d" />




# Phase 4: Data Analysis Using Apache Hive

## Objective
Analyze the cleaned hotel booking dataset stored in HDFS using Apache Hive.

## Technologies
- Apache Hive
- Hadoop HDFS

## Steps

1. Create Hive database.
2. Create an external table linked to the cleaned dataset in HDFS.
3. Execute analytical SQL queries.

## Analysis Performed

- Total Bookings
- Booking Trend by Month
- Cancellation Rate
- Hotel Type Comparison
- Average Daily Rate (ADR)
- Booking Distribution by Country
- Customer Type Analysis
- Top Countries by Bookings

## Dataset Location

HDFS:
/hotel_project/cleaned_data_final

<img width="703" height="283" alt="image" src="https://github.com/user-attachments/assets/2d87c7eb-086b-464a-bbfc-2513324a3e7d" />
<img width="625" height="721" alt="image" src="https://github.com/user-attachments/assets/e2d74a13-7c6e-42f4-8bf2-20f63116f07b" />

<img width="926" height="721" alt="image" src="https://github.com/user-attachments/assets/42448bf8-a8ed-4e49-bb6e-01116af24260" />
<img width="1253" height="41" alt="image" src="https://github.com/user-attachments/assets/9c1cf9fe-6e5a-479c-b040-8e03474124c3" />
<img width="492" height="75" alt="image" src="https://github.com/user-attachments/assets/077f8d0e-4651-4c1e-91ba-0f2f7520fe47" />
<img width="990" height="99" alt="image" src="https://github.com/user-attachments/assets/afbbadbe-1a62-45a8-ae7d-8794ee1409e9" />
<img width="875" height="102" alt="image" src="https://github.com/user-attachments/assets/b60be0a1-d09e-43f2-a96d-586c65f04523" />
<img width="1149" height="129" alt="image" src="https://github.com/user-attachments/assets/b7322698-696b-4be5-a830-8c206a3ecc21" />
<img width="687" height="265" alt="image" src="https://github.com/user-attachments/assets/2a085736-ca6b-4ff4-9aa0-c090f073b4c0" />
<img width="957" height="141" alt="image" src="https://github.com/user-attachments/assets/c3b36c5b-a714-4a43-ab79-6f97cc60c6e1" />
<img width="462" height="64" alt="image" src="https://github.com/user-attachments/assets/1967c66c-c2ee-4d03-ad01-b120e186d701" />
<img width="1077" height="112" alt="image" src="https://github.com/user-attachments/assets/4bcca15f-ad08-419b-be28-1feb8a568532" />
<img width="542" height="89" alt="image" src="https://github.com/user-attachments/assets/e3698e24-0aaa-4b9f-abd7-bb35de6e9b05" />
<img width="571" height="95" alt="image" src="https://github.com/user-attachments/assets/96639f8b-500c-44bc-bbe4-3e1f4b23374e" />
<img width="476" height="71" alt="image" src="https://github.com/user-attachments/assets/b74422b7-0e04-4f45-a545-15c493a2f65b" />
<img width="638" height="143" alt="image" src="https://github.com/user-attachments/assets/86f894e6-4bff-4024-ab6f-df6d58c6d486" />
<img width="574" height="238" alt="image" src="https://github.com/user-attachments/assets/706b1c58-c3ea-4a0f-881c-fd45182be7eb" />
<img width="853" height="125" alt="image" src="https://github.com/user-attachments/assets/3946a032-474e-4479-aa36-f0c98bb5175b" />
<img width="676" height="144" alt="image" src="https://github.com/user-attachments/assets/43bfdc6c-a839-41e8-b03b-1327546246d5" />



