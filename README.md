# CODTECH Internship Task 1 - Big Data Analysis using PySpark

## 📌 Project Title
Big Data Analysis using PySpark (NYC Yellow Taxi Dataset)

---

## 📖 Project Description
This project is completed as part of the **CODTECH Internship - Task 1**.  
The main objective of this task is to perform **Big Data Analysis** using **Apache Spark (PySpark)** on a large real-world dataset.  

In this project, the dataset is loaded using Spark, cleaned by removing invalid and null values, transformed for better analysis, and finally exported into Parquet and CSV formats.

---

## 📂 Dataset Information
### Dataset Name:
NYC Yellow Taxi Trip Records

### Dataset Source:
NYC TLC (Taxi and Limousine Commission) Open Data

### Dataset File Used:
`yellow_tripdata_2023-01.parquet`

### Dataset Format:
Parquet (.parquet)

### Dataset Contains Columns Like:
- VendorID
- tpep_pickup_datetime
- tpep_dropoff_datetime
- passenger_count
- trip_distance
- fare_amount
- payment_type
- total_amount

---

## ⚙️ Technologies and Tools Used
- Python 3.11
- Apache Spark (PySpark)
- Java JDK 17
- Hadoop winutils (Windows setup)
- Jupyter Notebook
- Pandas
- Matplotlib

---

## ✅ Steps Performed in the Project

### 1️⃣ Spark Setup
A SparkSession was created in Jupyter Notebook to run Spark jobs locally.

### 2️⃣ Dataset Loading
The Parquet dataset was loaded into a Spark DataFrame using:
- `spark.read.parquet()`

### 3️⃣ Data Cleaning
The dataset was cleaned using Spark transformations:
- Removed null values using `dropna()`
- Filtered invalid passenger count values (passenger_count > 0)
- Removed invalid trip distances (trip_distance > 0)
- Removed invalid fare amounts (fare_amount > 0)

### 4️⃣ Data Analysis
The cleaned dataset was analyzed to find:
- Passenger count distribution
- Average trip distance
- Average fare amount
- Payment type distribution
- Total trips count

### 5️⃣ Data Visualization
Visualization was performed using Matplotlib:
- Bar chart for passenger count distribution
- Bar chart for payment type distribution

### 6️⃣ Output Storage
The cleaned dataset was saved in:
- Parquet format (big data optimized)
- CSV format (for Excel/Power BI)

---

## 📊 Output Files Generated
Since GitHub does not allow large file uploads, a sample file is uploaded.

### Generated Output Files:
- `cleaned_taxi_data.parquet` (Saved Parquet format output)
- `cleaned_taxi_data_final.csv` (Final full cleaned CSV output - stored locally)
- `sample_cleaned_taxi_data.csv` (Sample output uploaded to GitHub)

---

## 📌 Project Structure
```bash
CODTECH_Task1_BigData_Analysis/
│── CODTECH_Task1_BigData_Analysis.ipynb
│── README.md
│── sample_cleaned_taxi_data.csv
│── requirements.txt
│── report.md (optional)
