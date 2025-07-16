# 🛒 Online Retail Sales - Exploratory Data Analysis (EDA) Project

This project involves performing Exploratory Data Analysis on a real-world e-commerce dataset to uncover business insights, customer behavior patterns, product performance, and seasonal trends. The final results are presented through a well-structured **Jupyter Notebook** and an interactive **Power BI dashboard**.

---

## 📁 Dataset

- **Source:** [Kaggle - Online Retail Dataset](https://www.kaggle.com/datasets/lakshmi25npathi/online-retail-dataset)
- **Description:** Transactions of a UK-based online retail store from **December 2010 to December 2011**.
- **Size:** ~500,000 rows
- **Key Columns:**
  - `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`

---

## 🎯 Project Goals

- Clean and preprocess raw transaction data
- Perform univariate, bivariate, and multivariate analysis
- Identify top-selling products and seasonal trends
- Segment customers using RFM analysis
- Present insights through visualizations in Jupyter and Power BI

---

## 📌 Project Structure

### 1. **Data Cleaning**
- Removed missing `CustomerID` and `Description` values
- Dropped duplicate entries
- Removed canceled orders (`InvoiceNo` starting with 'C')
- Handled outliers in `Quantity` and `UnitPrice`
- Converted `InvoiceDate` to datetime
- Added `TotalPrice = Quantity * UnitPrice`

### 2. **Exploratory Data Analysis (EDA)**

#### 🔹 General Overview
- Unique products
- Total transactions
- Customer distribution by country

#### 🔹 Product Analysis
- Top 10 selling products by quantity
- Top 10 products by revenue
- Detection of products with negative or zero prices

#### 🔹 Customer Analysis
- Customers with the highest frequency and spend
- Purchase distribution
- Loyal customer identification

#### 🔹 Time Series & Seasonal Trends
- Monthly revenue trends
- Peak and slow seasons
- Weekday purchasing patterns

#### 🔹 Country Analysis
- Revenue and order comparison across countries

---

### 3. **Customer Segmentation (RFM Analysis)**

- **RFM Metrics:**
  - **Recency**: Days since last purchase
  - **Frequency**: Total number of purchases
  - **Monetary**: Total amount spent

- **Scoring & Segmenting:**
  - Each metric scored from 1–5 using quantiles
  - RFM segment created by combining scores
  - Final classification:
    - 🎖️ Champions
    - 💎 Loyal
    - 🙂 Potential
    - ⚠️ At Risk

---

## 📊 Power BI Dashboard

An interactive Power BI dashboard was created with the following pages:

### 1️⃣ **Sales Overview**
- KPIs: Total Revenue, Number of Invoices, Total Customers
- Monthly sales trend (line chart)

### 2️⃣ **Top Products**
- Top 10 products by quantity and revenue (bar charts)
- Product breakdown by revenue (pie chart/treemap)

### 3️⃣ **Customer Segments**
- RFM Table view
- Scatter plot of Frequency vs Monetary by segment
- Top 10 loyal customers by revenue

### 4️⃣ **Geographical Insights**
- Revenue by country (Map & Bar chart)

---

## 🧪 Tools Used

- **Python (Pandas, Matplotlib, Seaborn)**
- **Jupyter Notebook**
- **Power BI**
- **Excel (for data previewing)**

---

## 🚀 How to Run the Project

1. Clone the repository
2. Open the `Online_Retail_EDA.ipynb` in Jupyter
3. Run the cells to view code, visualizations, and insights
4. Open the Power BI `.pbix` file to interact with the dashboard
5. You can also open `cleaned_online_retail.csv` and `rfm_segments.csv` directly in Power BI
