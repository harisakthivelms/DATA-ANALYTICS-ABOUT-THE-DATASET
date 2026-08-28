## DATA ANALYTICS ABOUT THE DATASET
# AIM

To perform data analytics on a given dataset using Python and Pandas, understand the characteristics of the dataset, identify different types of data, examine missing values, calculate descriptive statistics, and prepare the dataset for further analysis and machine learning.

# THEORY

Data Analytics is the process of examining, cleaning, transforming, and interpreting data to discover useful information and patterns. Python provides powerful libraries such as Pandas, NumPy, and Matplotlib for performing data analysis.

1. Dataset

A dataset is a structured collection of data arranged in rows and columns. Each row generally represents an observation or record, while each column represents a feature or variable.

2. Pandas

Pandas is a Python library widely used for data manipulation and analysis. Its main data structures are:

Series – One-dimensional labelled data.
DataFrame – Two-dimensional tabular data containing rows and columns.
3. Data Types

A dataset may contain different types of data:

Integer (int) – Whole numbers
Float (float) – Decimal values
Object/String (object) – Text or categorical information
Boolean (bool) – True/False values
Datetime – Date and time information

Identifying the data type of each column is important before performing analysis.

4. Dataset Inspection

Common Pandas functions used to understand a dataset include:

df.head()
df.tail()
df.shape
df.columns
df.info()
df.dtypes

These functions help identify the number of records, columns, data types, and overall structure of the dataset.

5. Descriptive Statistics

Statistical measures such as mean, median, standard deviation, minimum, maximum, and quartiles can be calculated to understand numerical data. Pandas' describe() function provides a summary of descriptive statistics and, by default, excludes missing values from these calculations.

df.describe()
6. Missing Values

Missing values are observations for which data is unavailable. Pandas provides functions such as:

df.isnull().sum()
df.isna().sum()

Missing values can be handled using methods such as:

df.dropna()
df.fillna(value)

Pandas also supports forward filling, backward filling, and interpolation for suitable datasets.

7. Data Cleaning

Before applying machine-learning algorithms, the dataset may need to be cleaned by:

Removing duplicate records
Handling missing values
Correcting incorrect data types
Removing irrelevant columns
Handling inconsistent values
Detecting outliers
Converting categorical data into suitable numerical representations
8. Data Preparation

After cleaning, the data can be prepared for further analysis or machine learning by selecting relevant features, transforming variables, and separating input features from target variables.

Basic Python Example
import pandas as pd

# Load dataset
df = pd.read_csv("dataset.csv")

# Display first five rows
print(df.head())

# Dataset size
print(df.shape)

# Column information
print(df.info())

# Data types
print(df.dtypes)

# Check missing values
print(df.isnull().sum())

# Descriptive statistics
print(df.describe())

# Remove duplicate records
df = df.drop_duplicates()

# Fill missing values
df = df.fillna(0)

print(df)

## RESULT

The given dataset was successfully loaded and analysed using Python and Pandas. The structure, dimensions, column names, data types, descriptive statistics, and missing values were identified. The dataset was also cleaned and prepared for further data analysis and machine-learning applications.
