# Titanic-Dataset-cleaning-
Data Cleaning &amp; Preprocessing

# Titanic Dataset Cleaning

This project focuses on cleaning and preprocessing the Titanic dataset. The Jupyter Notebook `Titanic-Dataset cleaning .ipynb` contains the code and steps performed to handle missing values, encode categorical features, and scale numerical data.

## Project Description

The goal of this project is to prepare the Titanic dataset for further analysis or machine learning tasks. The following steps were performed:

1.  **Import Libraries**:  Imported necessary libraries such as `pandas`, `numpy`, `seaborn`, `matplotlib.pyplot`, `LabelEncoder`, and `StandardScaler`.
2.  **Load Dataset**: Loaded the Titanic dataset from a CSV file (`Titanic-Dataset.csv`).
3.  **Explore Data**:  Checked the dataset's information using `df.info()` and identified missing values using `df.isnull().sum()`.
4.  **Handle Missing Values**:
    * Filled missing `Age` values with the median age.
    * Filled missing `Embarked` values with the mode (most frequent value).
    * Dropped the `Cabin` column due to a large number of missing values.
5.  **Encode Categorical Features**:
    * Encoded the `Sex` column using `LabelEncoder` (male/female to 0/1).
    * Converted the `Embarked` column into dummy variables using `pd.get_dummies()`.
6.  **Scale Numerical Features**:
    * Scaled the `Age` and `Fare` columns using `StandardScaler`.
7.  **Outlier Detection and Removal**:
    * Visualized the distribution of `Fare` using a boxplot.
    * Removed outliers in the `Fare` column by filtering values less than 3 (after scaling).
8.  **Display Processed Data**: Printed the first few rows of the cleaned dataset using `df.head()`.

## Files

* `Titanic-Dataset cleaning .ipynb`: Jupyter Notebook containing the data cleaning and preprocessing code.
* `Titanic-Dataset.csv`: The original Titanic dataset (not included in the cleaning process but assumed to be in the same directory).

## Libraries Used

* `pandas`
* `numpy`
* `seaborn`
* `matplotlib.pyplot`
* `sklearn.preprocessing` (LabelEncoder, StandardScaler)

## Usage

To reproduce the data cleaning process:

1.  Ensure you have the required libraries installed. You can install them using pip:
    ```bash
    pip install pandas numpy seaborn matplotlib scikit-learn
    ```
2.  Place the `Titanic-Dataset.csv` file in the same directory as the Jupyter Notebook.
3.  Open and run the `Titanic-Dataset cleaning .ipynb` notebook.

## Output

The notebook outputs the cleaned and preprocessed dataset, which is ready for further analysis or model training.

---
