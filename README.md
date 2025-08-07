# Food Delivery ETL Pipeline Project

This project demonstrates a scalable, end-to-end ETL (Extract, Transform, Load) pipeline for a food delivery platform—similar to Zomato or Swiggy—combining traditional relational database design with modern big data tools.

### Core Features

- **Relational Database Design:**  
  Includes a normalized PostgreSQL schema tailored for food delivery operations, covering customers, orders, restaurants, menu management, carts, payment invoices, delivery partners, and more.

- **Real-Time Data Ingestion with Kafka:**  
  Utilizes Apache Kafka to stream real-time events such as order transactions, customer activity, delivery updates, and payment details.

- **Schema Management:**  
  Maintains strong data integrity and compatibility across microservices by integrating a Schema Registry for Kafka topics.

- **Object Storage with MinIO (S3-Compatible):**  
  Raw and semi-structured event data is landed in MinIO for batch analytics and persistence—enabling cost-effective, durable, and scalable data storage outside the database.

- **Data Transformation with PySpark:**  
  Apache Spark processes and transforms event streams and object data. ETL jobs cleanse, enrich, and join datasets for downstream analytics and business reporting.

- **Data Warehousing:**  
  The processed and analytics-ready data is loaded back into PostgreSQL for use by BI tools, dashboards, and operational analytics.

- **Management & Monitoring:**  
  Kafka Control Centre, ZooKeeper, and related utilities are used for system administration, health monitoring, and topic management.

### Tech Stack

- PostgreSQL (Relational Database)
- Apache Kafka (Event Streaming)
- Kafka Schema Registry
- ZooKeeper (Kafka Coordination)
- MinIO (S3-Compatible Object Storage)
- Apache Spark (PySpark)
- Kafka Control Centre

### Problem Solved

This pipeline design bridges the gap between transactional operations (OLTP) and high-volume analytical processing (OLAP), supporting both real-time streaming and scalable batch workflows for food delivery businesses.
