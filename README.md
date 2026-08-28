# Superstore Sales Data Analysis

## Project Description

This project performs data analysis on a Superstore sales dataset using Python. The main purpose of the project is to understand sales data, customer information, product categories, discounts, profits, and delivery time.

The project uses **Pandas, NumPy, Matplotlib, and Seaborn** for data loading, data analysis, and visualization.

## Dataset

The dataset contains **10,194 records and 21 columns** before adding the delivery-days column.

The main columns include:

* Row ID
* Order ID
* Order Date
* Ship Date
* Ship Mode
* Customer ID
* Customer Name
* Segment
* Country/Region
* City
* State/Province
* Postal Code
* Region
* Product ID
* Category
* Sub-Category
* Product Name
* Sales
* Quantity
* Discount
* Profit

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Google Colab / Jupyter Notebook

## Project Steps

### 1. Import Libraries

The project imports Pandas, NumPy, Matplotlib, and Seaborn for data analysis and visualization.

### 2. Load the Dataset

The Superstore CSV dataset is loaded using Pandas.

```python
df = pd.read_csv("samplesuperstore.csv")
```

### 3. Explore the Dataset

The project uses functions such as:

* `df.head()`
* `df.info()`
* `df.shape`
* `df.describe()`

These functions are used to understand the structure, size, data types, and statistical information of the dataset.

### 4. Data Type Conversion

The `Order Date` and `Ship Date` columns are converted into datetime format.

```python
df['Order Date'] = pd.to_datetime(df['Order Date'], format='mixed')
df['Ship Date'] = pd.to_datetime(df['Ship Date'], format='mixed')
```

### 5. Calculate Delivery Days

A new column called `Delivery Days` is created to calculate the number of days between the order date and shipping date.

```python
df['Delivery Days'] = (df['Ship Date'] - df['Order Date']).dt.days
```

### 6. Check Missing Values

The project checks all columns for missing values using:

```python
df.isnull().sum()
```

The dataset contains no missing values in the analyzed columns.

### 7. Sales Analysis by Category

The total sales are calculated for each product category.

The dataset contains three main categories:

* Furniture
* Office Supplies
* Technology

Technology has the highest total sales among the three categories.

### 8. Data Visualization

A bar chart is created to visualize sales by category.

```python
category_sales.plot(kind='bar', figsize=(8,5))
plt.title("Sales by Category")
plt.ylabel("Total Sales")
plt.show()
```

## Key Findings

* The dataset contains 10,194 records.
* The dataset initially contains 21 columns.
* A new `Delivery Days` column is calculated during analysis.
* There are no missing values in the dataset.
* The dataset contains Furniture, Office Supplies, and Technology categories.
* Technology records the highest total sales among the three categories.

## How to Run

1. Open the notebook using **Google Colab** or **Jupyter Notebook**.
2. Upload the `samplesuperstore.csv` dataset.
3. Open `program1.ipynb`.
4. Run the cells from top to bottom.
5. View the analysis results and charts.

## Project Structure

```text
Superstore-Sales-Analysis/
│
├── program1.ipynb
├── samplesuperstore.csv
└── README.md
```

## Conclusion

This project demonstrates how Python can be used to perform basic data analysis and visualization on a sales dataset. It helps in understanding sales performance, product categories, customer information, profit, discounts, and delivery time.
