<img width="880" height="559" alt="WhatsApp Image 2026-08-28 at 2 23 22 PM" src="https://github.com/user-attachments/assets/c692e523-2e0d-4bd9-8f0d-b9cf601ec0d9" />
<img width="873" height="492" alt="WhatsApp Image 2026-08-28 at 2 23 22 PM (1)" src="https://github.com/user-attachments/assets/79d2a4a8-1b61-4376-a3aa-ecc08d9ebe7e" />
# 📊 Superstore Sales Data Analysis

> **A Python-based data analysis and visualization project using the Superstore dataset**

---

## 📌 About the Project

This project analyzes a **Superstore sales dataset** using Python.
The main goal is to understand the sales performance of different product categories and explore important business information such as **Sales, Quantity, Discount, Profit, and Delivery Days**.

The project uses **Pandas, NumPy, Matplotlib, and Seaborn** to perform data analysis and create visualizations.

---

## 🎯 Objectives

The main objectives of this project are:

* To understand and explore the sales dataset.
* To clean and prepare the data for analysis.
* To convert date columns into the correct format.
* To calculate delivery time.
* To check for missing values.
* To analyze sales based on product categories.
* To visualize sales results using charts.

---

## 🛠️ Technologies Used

| Technology      | Purpose                   |
| --------------- | ------------------------- |
| 🐍 Python       | Programming Language      |
| 🐼 Pandas       | Data Analysis             |
| 🔢 NumPy        | Numerical Operations      |
| 📈 Matplotlib   | Data Visualization        |
| 🎨 Seaborn      | Statistical Visualization |
| ☁️ Google Colab | Development Environment   |

---

## 📂 Dataset

The dataset contains **Superstore sales information** with details about:

* Orders
* Customers
* Products
* Categories
* Sales
* Quantity
* Discounts
* Profit
* Shipping
* Delivery time

The dataset contains **10,194 records** and **21 original columns**. A new column called **Delivery Days** is calculated during the analysis.

---

## 🔍 Data Analysis Process

### 1️⃣ Import Libraries

The required Python libraries are imported for data analysis and visualization.

### 2️⃣ Load Dataset

The Superstore CSV file is loaded using Pandas.

### 3️⃣ Explore Data

The following functions are used to understand the dataset:

```python
df.head()
df.info()
df.shape
df.describe()
```

### 4️⃣ Convert Date Columns

The `Order Date` and `Ship Date` columns are converted into datetime format.

### 5️⃣ Calculate Delivery Days

A new column, **Delivery Days**, is created by calculating the difference between the ship date and order date.

### 6️⃣ Check Missing Values

The dataset is checked for missing values using:

```python
df.isnull().sum()
```

The analysis shows **no missing values** in the dataset.

### 7️⃣ Analyze Sales by Category

Sales are grouped according to the three main product categories:

* 🪑 Furniture
* 📎 Office Supplies
* 💻 Technology

The total sales are calculated for each category.

### 8️⃣ Create Visualization

A bar chart is created to compare the total sales of different categories.

---

## 📊 Key Results

| Category           |  Total Sales |
| ------------------ | -----------: |
| 🪑 Furniture       | 754,747.7613 |
| 📎 Office Supplies | 731,893.3140 |
| 💻 Technology      | 839,893.2790 |

### ⭐ Main Finding

**Technology** has the highest total sales among the three categories, followed by **Furniture** and **Office Supplies**.

---

## 📈 Visualization

The project creates a **Sales by Category** bar chart to make it easier to compare the performance of each category.

---

## 🚀 How to Run the Project

### Step 1

Download or open the project notebook.

### Step 2

Make sure the following files are available in the same working environment:

```text
program1.ipynb
samplesuperstore.csv
```

### Step 3

Open `program1.ipynb` using **Google Colab** or **Jupyter Notebook**.

### Step 4

Run the notebook cells from top to bottom.

### Step 5

View the analysis results and generated charts.

---

## 📁 Project Structure

```text
Superstore-Sales-Analysis/
│
├── 📓 program1.ipynb
├── 📄 samplesuperstore.csv
└── 📖 README.md
```

---

## 💡 Conclusion

This project demonstrates how **Python can be used to analyze real-world sales data**.

The analysis helps understand:

* Sales performance
* Product categories
* Customer and order information
* Discounts and profit
* Delivery time
* Category-wise sales

Overall, the project provides a simple and clear approach to **exploratory data analysis and visualization using Python**.

---

## 👩‍💻 Project

**Superstore Sales Data Analysis**
**Developed using Python & Data Analysis Libraries**
