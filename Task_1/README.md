# Titanic Data Cleaning and Preprocessing

## Problem Statement

Raw datasets often contain missing values, duplicate records, inconsistent data types, and unclear column names. These issues can affect the accuracy and usability of the data. The purpose of this project is to clean and prepare the Titanic dataset for further analysis.

## Dataset Details

* **Dataset:** Titanic Test Dataset
* **Source:** Kaggle
* **File Used:** `test.csv`
* **Number of Records:** 418
* **Dataset Type:** Tabular data

The dataset contains information about passengers, including passenger class, name, gender, age, ticket details, fare, and port of embarkation.

## Objective

The main objectives of this project are:

* To identify and handle missing values.
* To check for duplicate records.
* To maintain suitable data types.
* To rename columns using clear and consistent names.
* To export the cleaned dataset as a CSV file.

## Data Cleaning Approach

### 1. Handling Missing Values

* Missing values in the `Age` column were replaced using the median age.
* Missing values in the `Fare` column were replaced using the median fare.
* The `Cabin` column was removed because it contained a large number of missing values.
* The cleaned dataset contains no missing values.

### 2. Checking Duplicate Records

The dataset was checked for duplicate rows. No duplicate records were found.

### 3. Data Type Conversion

Suitable data types were maintained for the columns. The `PassengerId` and `Pclass` columns were converted to integer-based data types.

### 4. Column Renaming

The column names were standardized to make them easier to understand and use during further analysis.

Examples:

* `PassengerId` → `passenger_id`
* `Pclass` → `passenger_class`
* `SibSp` → `siblings_spouses`
* `Parch` → `parents_children`

## Results

The Titanic dataset was successfully cleaned and preprocessed. Missing values were handled, duplicate records were checked, data types were maintained, and column names were standardized. The final cleaned dataset was saved as `cleaned_titanic.csv`.

## Technologies Used

* Python
* Pandas
* NumPy
* Jupyter Notebook

## Project Files

* `test.csv` – Original Titanic dataset
* `cleaned_titanic.csv` – Cleaned dataset
* `Task_1_Titanic_Data_Cleaning.ipynb` – Jupyter Notebook containing the complete cleaning process

## Conclusion

This project demonstrates the basic steps of data cleaning and preprocessing using Python and Pandas. The cleaned dataset is now ready for further analysis or visualization.
