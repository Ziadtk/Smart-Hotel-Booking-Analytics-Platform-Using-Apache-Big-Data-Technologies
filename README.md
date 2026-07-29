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
<img width="745" height="94" alt="image" src="https://github.com/user-attachments/assets/39b8e050-3f73-4bb4-b11c-f8e49741682f" />
<img width="712" height="426" alt="image" src="https://github.com/user-attachments/assets/c4e984ce-7324-4a85-b49e-a9f38dc8dc57" />
<img width="1191" height="47" alt="image" src="https://github.com/user-attachments/assets/db022a8f-ff4d-413d-98df-12e1bb75b8a2" />

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




