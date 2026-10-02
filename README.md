# Load a CSV Dataset Using Pandas

## 📌 Project Overview

This project demonstrates how to load and inspect a CSV dataset using **Python and Pandas**.

The **Iris Dataset** is used to demonstrate how to:

- Import Pandas
- Load a CSV dataset
- Display the first five records
- Display the last five records
- Check the dataset shape
- Check column names
- Verify that the dataset loaded correctly

## 🎯 Objective

The objective of this task is to learn how to import real-world tabular data using Pandas for data analysis and machine learning workflows.

## 🛠️ Technologies Used

- Python 3
- Pandas
- Jupyter Notebook / JupyterLab

## 📊 Dataset

The Iris dataset contains measurements of iris flowers.

### Dataset Details

- **Rows:** 150
- **Columns:** 5
- **Features:** Sepal Length, Sepal Width, Petal Length, Petal Width
- **Target:** Species

### Columns

| Column | Description |
|---|---|
| `sepal_length` | Length of the sepal |
| `sepal_width` | Width of the sepal |
| `petal_length` | Length of the petal |
| `petal_width` | Width of the petal |
| `species` | Species of the iris flower |

### Species

The dataset contains three species:

- Setosa
- Versicolor
- Virginica

## 🔗 Dataset Source

The Iris dataset was loaded from:

https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv

## 💻 Implementation

```python
import pandas as pd

# Load the Iris CSV dataset
url = "https://raw.githubusercontent.com/mwaskom/seaborn-data/master/iris.csv"
df = pd.read_csv(url)

# Display first 5 records
print("First 5 records:")
display(df.head())

# Display last 5 records
print("\nLast 5 records:")
display(df.tail())

# Check dataset shape
print("\nDataset Shape:", df.shape)

# Display column names
print("\nColumn Names:")
print(df.columns.tolist())

# Display dataset information
print("\nDataset Information:")
df.info()
