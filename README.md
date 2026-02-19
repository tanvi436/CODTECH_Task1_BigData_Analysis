# CODTECH Internship Task 1 - Big Data Analysis using PySpark

## Project Overview
This project is completed as part of the CODTECH Internship Task 1.  
The objective of this task is to perform Big Data analysis using Apache Spark (PySpark) on a large dataset, apply data cleaning, perform transformations, and generate useful insights.

---

## Dataset Used
**Dataset Name:** NYC Yellow Taxi Trip Records  
**Source:** NYC TLC Official Dataset  
**File Used:** `yellow_tripdata_2023-01.parquet`

This dataset contains taxi trip details such as:
- Pickup and dropoff datetime
- Trip distance
- Fare amount
- Passenger count
- Payment type
- Total amount

---

## Tools and Technologies Used
- Python 3.11
- Apache Spark (PySpark)
- Jupyter Notebook
- Java JDK 17
- Hadoop winutils (for Windows)
- Pandas
- Matplotlib

---

## Steps Performed
### 1. Spark Session Setup
A Spark session was created using PySpark in Jupyter Notebook to process large-scale data.

### 2. Dataset Loading
The dataset was loaded in Parquet format using Spark DataFrame API.

### 3. Data Cleaning
The following cleaning operations were performed:
- Removed null values
- Filtered invalid passenger counts
- Filtered invalid trip distance values
- Filtered invalid fare amount values

### 4. Data Analysis
The dataset was analyzed to find:
- Passenger count distribution
- Average trip distance
- Average fare amount
- Most common payment types

### 5. Data Visualization
Basic visualization was done using Matplotlib for:
- Passenger count distribution
- Payment type distribution

### 6. Output Saving
The cleaned dataset was saved in:
- Parquet format
- CSV format

---

## Output Files Generated
- `cleaned_taxi_data.parquet` (cleaned dataset in parquet format)
- `cleaned_taxi_data_final.csv` (cleaned dataset in CSV format)
- `sample_cleaned_taxi_data.csv` (sample CSV file for GitHub)

---

## How to Run This Project
### Step 1: Install Dependencies
```bash
pip install pyspark pandas matplotlib
