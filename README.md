# E-Commerce Sales & Customer Behavior Analysis

A complete end-to-end data analysis project that explores e-commerce sales data to uncover revenue trends, customer behavior, profitability drivers, and actionable business insights.

---

## 📌 Project Overview

This project analyzes transactional data from an e-commerce company to answer important business questions such as:

- Which region generates the highest profit?
- Which product categories drive the most revenue?
- How do discounts affect profitability?
- What are the seasonal sales trends?
- Which customer segments are most valuable?

The dataset contained missing values, duplicates, invalid records, and inconsistent formatting. After performing extensive data cleaning and exploratory data analysis (EDA), meaningful insights and business recommendations were derived.

---

## 🎯 Objectives

- Clean and validate raw e-commerce data
- Handle missing values and duplicates
- Detect and treat outliers
- Perform exploratory data analysis (EDA)
- Analyze customer purchasing behavior
- Identify key business drivers
- Generate actionable recommendations

---

## 🛠️ Tools and Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📂 Dataset Description

The dataset includes the following fields:

- Order ID
- Customer ID
- Order Date
- Ship Date
- Region
- State
- Product Category
- Sub Category
- Sales
- Profit
- Discount
- Quantity
- Shipping Cost
- Payment Mode
- Customer Segment

---

## 🧹 Data Cleaning Process

### 1. Basic Inspection
- Checked dataset shape, columns, and data types
- Identified missing values and duplicates

### 2. Handling Missing Values
- `Customer_Segment` → Filled with mode
- `Profit` → Filled with median
- `Shipping_Cost` → Filled with median

### 3. Removing Duplicates
- Removed 500 duplicate rows

### 4. Data Type Corrections
- Converted Sales and Profit to numeric
- Converted date columns to datetime format

### 5. Logical Validation
- Removed records where Ship Date < Order Date
- Removed negative sales values
- Removed discounts greater than 80%

### 6. Outlier Treatment
- Used IQR method
- Capped extreme values in Profit and Shipping Cost

### 7. Standardization
- Removed extra spaces
- Standardized capitalization in categorical columns

---

## 📊 Exploratory Data Analysis (EDA)

### Univariate Analysis
- Sales distribution
- Profit distribution
- Discount analysis
- Quantity distribution
- Shipping Cost distribution

### Categorical Analysis
- Sales by Region
- Sales by Customer Segment
- Sales by Product Category
- Top 10 Products by Sales
- Top 10 States by Sales

### Bivariate Analysis
- Sales vs Profit
- Discount vs Profit
- Shipping Cost vs Profit
- Category vs Profit
- Region vs Profit

### Time-Based Analysis
- Monthly Sales Trend
- Quarterly Revenue Growth
- Seasonal Patterns
- Best and Worst Performing Months

### Customer Analysis
- Pareto Analysis (Top 20% Customers)
- Repeat Customer Behavior
- Average Order Value by Segment

### Correlation Analysis
- Correlation Heatmap
- Strongest Variable Relationships

---

## 📈 Key Findings

### Regional Performance
- **North Region** generated the highest sales and profit.

### Customer Segments
- **Consumer Segment** generated the highest total revenue.
- **Corporate Segment** had the highest average order value.

### Product Categories
- **Electronics** was the top-performing category by sales.
- **Electronics and Furniture** generated strong profits.

### Discount Impact
- Higher discounts were associated with lower profitability.

### Seasonal Trends
- Sales fluctuated significantly across months.
- **December 2022** was the best-performing month.
- **February 2022** was the worst-performing month.

### Customer Contribution
- Top 20% of customers contributed approximately **29%** of total revenue.

### Correlation Insights
- Sales and Profit showed a strong positive correlation (**0.87**).

---

## 💡 Business Insights

### Most Profitable Region
- North Region

### Category to Promote
- Electronics

### Discount Strategy
- Excessive discounting reduces profit margins

### Most Valuable Customers
- Consumer Segment (highest revenue)
- Corporate Segment (highest order value)

### Shipping Cost Impact
- Minimal direct impact on profitability

---

## 🚀 Actionable Recommendations

1. Optimize discount strategy to protect profit margins
2. Increase marketing in low-performing regions
3. Promote high-profit categories like Electronics and Furniture
4. Prepare inventory for peak seasonal months
5. Focus on increasing sales volume to improve profitability

---

## 📊 Visualizations Created

More than 15 visualizations were created, including:

- Histograms
- Boxplots
- Bar Charts
- Scatter Plots
- Line Charts
- Correlation Heatmaps

---

## 📁 Project Structure

```text
E-Commerce-Sales-Analysis/
│── data/
│   └── ecommerce_dirty_dataset.csv
│
│── notebooks/
│   └── E-Commerce-Sales-Analysis.ipynb
│
│── images/
│   └── charts and visualizations
│
│── documentation/
│   └── Project_Documentation.pdf
│
│── README.md
