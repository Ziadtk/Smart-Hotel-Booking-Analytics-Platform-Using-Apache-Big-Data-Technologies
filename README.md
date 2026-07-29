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


