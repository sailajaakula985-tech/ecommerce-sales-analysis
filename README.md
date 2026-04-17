# 🛒 E-Commerce Sales Performance Analysis

A Python-based exploratory data analysis (EDA) project that uncovers revenue trends, customer behavior patterns, and actionable segments from e-commerce transaction data.

---

## 📌 Project Overview

This project analyzes an e-commerce dataset to answer key business questions:

- How does revenue trend over time (monthly)?
- Which product categories drive the most sales?
- How do customers behave across different devices?
- Is there a relationship between delivery time and customer satisfaction?
- Who are the most valuable customers, and who is at risk of churning?

---

## 📂 Dataset

**File:** `E_Commerce.csv`

**Key columns used:**

| Column | Description |
|---|---|
| `Date` | Order date |
| `Order_ID` | Unique order identifier |
| `Customer_ID` | Unique customer identifier |
| `Product_Category` | Category of the purchased product |
| `Total_Amount` | Revenue from the order |
| `Quantity` | Units purchased |
| `Gender` | Customer gender |
| `Delivery_Time_Days` | Days taken to deliver |
| `Customer_Rating` | Rating given by the customer |
| `Device_Type` | Device used to place the order |
| `Session_Duration_Minutes` | Time spent on the platform |
| `Pages_Viewed` | Number of pages viewed per session |

---

## 🔍 Analysis Performed

### 1. Monthly Revenue Trend
Resampled order data by month to visualize how total revenue changes over time.

### 2. Product Category Performance
Grouped by `Product_Category` to compare total revenue and units sold — identifying best and worst performing categories.

### 3. Average Spend by Gender
Bar chart showing how average order value differs between male and female customers.

### 4. Delivery Time vs. Customer Rating
Correlation analysis to determine if longer delivery times negatively impact ratings.

### 5. Device Type Behavior
Compared average session duration and pages viewed across device types (mobile, tablet, desktop).

### 6. Day-of-Week Sales Patterns
Identified which days of the week generate the highest revenue.

### 7. Correlation Heatmap
Visualized correlations between all numeric features to uncover hidden relationships.

### 8. RFM Customer Segmentation
Segmented customers into three groups based on **Recency**, **Frequency**, and **Monetary** value:

| Segment | Description |
|---|---|
| 🏆 Champions | High RFM score — most valuable customers |
| 💛 Loyal Customers | Mid-range RFM — engaged but not top spenders |
| ⚠️ At Risk | Low RFM score — inactive or low-value customers |

---

## 🛠️ Tech Stack

- **Python 3.x**
- **pandas** — data manipulation
- **matplotlib** — data visualization
- **seaborn** — statistical plots
- **datetime** — RFM recency calculation

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/sailajaakula985-tech/ecommerce-sales-analysis.git
cd ecommerce-sales-analysis
```

### 2. Install dependencies
```bash
pip install pandas matplotlib seaborn
```

### 3. Add the dataset
Place `E_Commerce.csv` in the project root directory (or update the file path in the notebook).

### 4. Run the notebook
```bash
jupyter notebook E_Commerce.ipynb
```

---

## 📊 Sample Outputs

- 📈 Monthly revenue line chart
- 📊 Category performance bar chart
- 🔥 Correlation heatmap
- 👥 Customer segment distribution (magma palette)

---

## 💡 Key Insights

- Revenue trends reveal peak and off-peak months for targeted promotions.
- RFM segmentation allows marketing teams to prioritize high-value customers and re-engage at-risk ones.
- Device-type analysis helps optimize the UX for the most-used platform.
- Delivery time correlation with ratings can guide logistics improvements.

---

## 📁 Project Structure

```
ecommerce-sales-analysis/
│
├── E_Commerce.ipynb       # Main analysis notebook
├── E_Commerce.csv         # Dataset (add manually)
└── README.md              # Project documentation
```

---

## 🙋‍♀️ Author

**Sailaja**  
Feel free to connect or raise an issue if you have questions or suggestions!




