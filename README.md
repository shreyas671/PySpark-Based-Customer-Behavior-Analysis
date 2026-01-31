PySpark-Based Customer Behavior Analysis
This project focuses on building an end-to-end big data analytics pipeline using Hadoop for large-scale data ingestion and PySpark for distributed data processing. Utilizing a dataset of over 110 million user interaction events from a multi-category eCommerce store, the goal is to understand behavioral patterns, predict purchase likelihood, and segment customers for personalized marketing.

Technical Stack

Big Data Frameworks: Hadoop (HDFS), Apache Spark

Languages: Python (PySpark)

ML Library: PySpark MLLib

Data Source: eCommerce Behavior Data from a Multi-Category Store (Kaggle)

Phase I: Foundation & Ingestion

The first phase established the infrastructure and initial data processing.

Key Steps:
  1. Environment Setup: Deployed a Hadoop cluster for large-scale storage and configured PySpark with OpenJDK-11.
  2. Data Ingestion: Large-scale ingestion of multi-month CSV datasets into HDFS.
  3. Exploratory Data Analysis (EDA): Analyzed user interaction types (view, cart, purchase) and behavioral trends across categories.
  4. Preprocessing: Cleaning, merging multi-month datasets, and handling initial schema transformations.

Phase II: Advanced Analytics & Machine Learning

Phase II extends the pipeline by implementing predictive and descriptive models using PySpark MLLib.

  A. Data Cleaning & Feature Engineering
    
  1. Missing Value Imputation: Handled missing categorical data with mode values and numerical data with mean values.
  2. Time-Series Features: Extracted hour and day_of_week from event timestamps to identify peak shopping windows.
  3. Encoding: Applied StringIndexer and OneHotEncoder for categorical variables like category_code and brand.
  4. Frequency Features: Integrated frequency counts for brands and categories to enhance model context.

  B. Machine Learning Models
  
  1. Classification: Built models to predict purchase likelihood based on user interaction history.
  2. Regression: Implemented revenue estimation models to forecast spending trends.
  3. Clustering: Segmented customers (e.g., "Frequent Buyers," "Window Shoppers," "Cart Abandoners") using behavioral metrics like session duration and conversion frequency.
  4. Association Rule Mining: Utilized the FP-Growth algorithm to identify cross-category product affinities and build recommendation systems.



