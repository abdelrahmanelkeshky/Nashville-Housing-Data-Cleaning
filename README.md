# 🏡 Nashville Housing Data Cleaning

## 📌 Overview

***This project focuses on cleaning and preprocessing real estate data from the Nashville Housing Dataset using SQL. The key objectives include standardizing date formats, handling missing values, splitting address fields, correcting categorical values, removing duplicates, and optimizing the dataset for further analysis.***

## 🗂️ Cleaning Steps & SQL Techniques

### 1. 📅 Standardizing Date Format

- **Convert SaleDate to Date format for consistency.**

- **Create a new column SaleDateConverted and populate it with formatted dates.**

### 2. 🏠 Handling Missing Property Addresses

- **Identify NULL values in PropertyAddress.**

- **Use self-joins to populate missing addresses based on matching ParcelID.**

### 3. 📌 Splitting Address into Components

- **Extract Street Address and City from PropertyAddress.**

- **Extract Street Address, City, and State from OwnerAddress using PARSENAME.**

### 4. ✅ Standardizing Categorical Values

- **Convert SoldAsVacant values:** *Replace Y with "Yes" and N with "No" for better readability.*

### 5. 🗑️ Removing Duplicates

- **Use CTE and ROW_NUMBER() to identify duplicate records based on key attributes (ParcelID, PropertyAddress, SalePrice, etc.).**

- **Select and remove redundant entries.**

### 6. 🔻 Dropping Unnecessary Columns

- **Remove fields that are no longer needed, such as OwnerAddress, TaxDistrict, PropertyAddress, and SaleDate.**

## 🛠️ Technologies Used:

**1. SQL Server / Any SQL Database**

**2. Data Cleaning Techniques: Joins, CTEs, Aggregations, String Functions**

**3. Data Standardization & Optimization**

## 🎯 How to Use

- Load the Nashville Housing Dataset into a SQL database.

- Execute the provided SQL scripts step by step.

- Validate results using SELECT * FROM NashvilleHousing.

- Use the cleaned dataset for analysis and visualization.

## 🔮 Future Enhancements

- Stored Procedures for automated cleaning processes.

- Triggers for real-time data validation.

- Integration with BI tools like Power BI or Tableau.

***✍️ Author: Abdelrahman Elkeshky***
