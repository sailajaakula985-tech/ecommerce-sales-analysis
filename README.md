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
| `Order_ID` | Unique identifier for each order |
| `Customer_ID` | Unique identifier for each customer |
| `Date` | Date the order was placed |
| `Age` | Age of the customer |
| `Gender` | Gender of the customer |
| `City` | City where the customer is located |
| `Product_Category` | Category of the purchased product |
| `Unit_Price` | Price per unit of the product |
| `Quantity` | Number of units purchased |
| `Discount_Amount` | Discount applied to the order |
| `Total_Amount` | Final revenue after discount |
| `Payment_Method` | Method used to pay (e.g. card, UPI, COD) |
| `Device_Type` | Device used to place the order (mobile, desktop, tablet) |
| `Session_Duration_Minutes` | Time the customer spent on the platform (in minutes) |
| `Pages_Viewed` | Number of pages viewed during the session |
| `Is_Returning_Customer` | Whether the customer has ordered before (Yes/No) |
| `Delivery_Time_Days` | Number of days taken to deliver the order |
| `Customer_Rating` | Rating given by the customer after delivery (1–5) |

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
git clone https://github.com/your-username/ecommerce-sales-analysis.git
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

### 📈 Total Monthly Revenue
![Total Monthly Revenue](images/monthly_revenue.png)
> Revenue ranged from ~1.6M (Jan 2023) to a peak of ~1.97M (Dec 2023), followed by a sharp drop in early 2024.

---

### 🛍️ Product Category Performance
![Product Category Performance](images/category_performance.png)
> Electronics led with ₹12.8M in revenue; Books had the lowest at ₹433K.

---

### 👤 Average Spend by Gender
![Average Spend by Gender](images/avg_spend_gender.png)
> The "Other" gender segment had the highest average spend (~₹1,380); Male and Female were close at ~₹1,200.

---

### 📅 Day-of-Week Sales
![Day of Week Sales](images/day_of_week_sales.png)
> Monday drove the most revenue (~₹4.0M); Thursday was the lowest (~₹3.55M).

---

### 📱 Device Type Behavior
![Device Type Behavior](images/device_behavior.png)
> All devices showed nearly identical session durations (~14.5 min) and pages viewed (~9).

---

### 🔥 Correlation Heatmap
![Correlation Heatmap](images/correlation_heatmap.png)
> Strong correlation between `Unit_Price` and `Total_Amount` (0.85); `Discount_Amount` moderately correlated (0.44).

---

### 👥 Customer Segmentation Distribution
![Customer Segmentation](images/customer_segmentation.png)
> 2,469 Loyal Customers · 1,865 Champions · 666 At Risk

---

## 💡 Key Insights

- **Revenue peaked in December 2023** (~₹1.97M) and dropped sharply in early 2024 — likely a post-holiday effect worth investigating.
- **Electronics dominates revenue** (₹12.8M) despite not having the highest quantity sold — it has the highest unit price impact.
- **Delivery time does not affect customer ratings** (correlation: -0.009), suggesting satisfaction is driven by other factors like product quality or experience.
- **Device type has no meaningful impact** on session behavior — all three devices show nearly identical engagement metrics.
- **Monday drives the most revenue** (~₹4M); consider scheduling promotions or flash sales on Mondays to capitalize on this trend.
- **666 at-risk customers** identified via RFM — a targeted re-engagement campaign could recover a significant portion of lost revenue.
- **Unit price is the strongest driver of total order value** (correlation: 0.85), confirming that high-ticket items are the primary revenue engine.

---

## 📁 Project Structure

```
ecommerce-sales-analysis/
│
├── E_Commerce.ipynb       # Main analysis notebook
├── E_Commerce.csv         # Dataset (add manually)
├── images/                # Output charts and visualizations
│   ├── monthly_revenue.png
│   ├── category_performance.png
│   ├── avg_spend_gender.png
│   ├── delivery_vs_rating.png
│   ├── device_behavior.png
│   ├── day_of_week_sales.png
│   ├── correlation_heatmap.png
│   └── customer_segmentation.png
└── README.md              # Project documentation
```

---

## 🙋‍♀️ Author

**Sailaja**  
Feel free to connect or raise an issue if you have questions or suggestions!

---

