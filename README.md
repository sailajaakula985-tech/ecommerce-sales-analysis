 🛒 E-Commerce Sales Performance Analysis

A Python-based exploratory data analysis (EDA) project that digs into e-commerce sales data to uncover revenue trends, customer behavior, and actionable business insights.

---

📋 Project Overview

This project analyzes an e-commerce dataset to answer key business questions:

- How does revenue trend month-over-month?
- Which product categories drive the most sales?
- Do spending patterns differ by gender or device type?
- Is there a relationship between delivery time and customer ratings?
- How can customers be segmented by purchase behavior?

---

📁 Dataset

**File:** `E_Commerce.csv`

The dataset contains **18 columns** covering order details, customer demographics, browsing behavior, and post-purchase feedback.

| Column | Type | Description | Example |
|---|---|---|---|
| `Order_ID` | string | Unique identifier for each order | `ORD-00123` |
| `Customer_ID` | string | Unique identifier for each customer | `CUST-4521` |
| `Date` | date | Date the order was placed (DD/MM/YYYY) | `15/03/2024` |
| `Age` | integer | Age of the customer in years | `34` |
| `Gender` | categorical | Customer gender | `Male` / `Female` |
| `City` | string | City where the order was placed | `Mumbai` |
| `Product_Category` | categorical | Category of the purchased product | `Electronics`, `Clothing` |
| `Unit_Price` | float | Price of a single unit of the product (₹) | `499.00` |
| `Quantity` | integer | Number of units purchased in the order | `3` |
| `Discount_Amount` | float | Discount applied on the order (₹) | `50.00` |
| `Total_Amount` | float | Final revenue after discount (`Unit_Price × Quantity − Discount`) (₹) | `1447.00` |
| `Payment_Method` | categorical | Mode of payment used | `UPI`, `Credit Card`, `COD` |
| `Device_Type` | categorical | Device used to place the order | `Mobile`, `Desktop`, `Tablet` |
| `Session_Duration_Minutes` | float | Time (in minutes) the customer spent on the platform | `12.5` |
| `Pages_Viewed` | integer | Number of pages browsed during the session | `8` |
| `Is_Returning_Customer` | boolean | Whether the customer has ordered before | `True` / `False` |
| `Delivery_Time_Days` | integer | Number of days taken to deliver the order | `5` |
| `Customer_Rating` | integer | Post-delivery rating given by the customer (1–5 scale) | `4` |

---

🔍 Analysis Performed

1. Monthly Revenue Trends
Time-series resampling to visualize how total revenue evolves month by month.

 2. Product Category Performance
Grouped aggregation of revenue and quantity sold per category to identify top performers.

 3. Spending by Gender
Bar chart comparing average order spend across genders.

 4. Delivery Time vs. Customer Rating
Correlation analysis to assess whether faster delivery leads to higher ratings.

 5. Device Type Behavior
Comparison of session duration and pages viewed across device types (mobile, desktop, etc.).

 6. Day-of-Week Sales Patterns
Bar chart of total revenue by day to identify peak shopping days.

 7. RFM Customer Segmentation
Customers are scored and segmented based on:
- **Recency** – How recently they ordered
- **Frequency** – How often they order
- **Monetary** – How much they spend

Segments: `Champions` | `Loyal Customers` | `At Risk`

 8. Correlation Heatmap
Seaborn heatmap of all numerical features to surface hidden relationships.

---

 🛠️ Tech Stack

- **Python 3.x**
- **pandas** – Data manipulation and aggregation
- **matplotlib** – Plotting and visualization
- **seaborn** – Statistical visualizations
- **datetime** – Date handling for RFM analysis

---

 🚀 Getting Started

 1. Clone the repository
```bash
git clone https://github.com/sailajaakula985-tech/ecommerce-sales-analysis.git
cd ecommerce-sales-analysis
```

2. Install dependencies
```bash
pip install pandas matplotlib seaborn
```

3. Add the dataset
Place `E_Commerce.csv` in the project root directory (or update the file path in the notebook).

 4. Run the notebook
```bash
jupyter notebook E_Commerce.ipynb
```

---

 📊 Sample Outputs

- Monthly revenue line chart
- Category performance table (sorted by revenue)
- RFM segmentation bar chart
- Full correlation heatmap

---

💡 Key Insights 
📦 Overall Performance
Total Orders: 22,049 across 5,000 unique customers
Total Revenue: ₹26,694,597
Average Order Value: ₹1,210.69
Average Customer Rating: 3.90 / 5
Average Delivery Time: 6.5 days


📈 Revenue Trends
Revenue grew steadily from ₹15.98L in January 2023 to a peak of ₹19.71L in December 2023
A slight dip is observed in early 2024 (Jan–Mar), likely seasonal
Monday is the highest revenue day (₹40.24L total), while Thursday is the lowest (₹35.64L)


🛍️ Product Categories
Electronics is the dominant category, contributing ₹1.28Cr — nearly 48% of total revenue
Home & Garden (₹49.3L) and Sports (₹39.6L) follow as the next top earners
Books (₹4.33L) and Food (₹5.18L) are the lowest revenue categories


👤 Customer Demographics
Customers identifying as Other gender have the highest average spend (₹1,376.54), followed by Female (₹1,216.75) and Male (₹1,199.15)
Istanbul is the top city by revenue (₹69.8L), followed by Ankara (₹37.1L) and Izmir (₹32.2L)


💳 Payment & Device Behavior
Credit Card is the most preferred payment method (40% of orders), followed by Debit Card (25%)
Cash on Delivery is the least used (5%)
All device types (Mobile, Desktop, Tablet) show nearly identical session durations (~14.5 min) and pages viewed (~9), suggesting a consistent user experience across platforms


🚚 Delivery & Satisfaction
Correlation between delivery time and customer rating is nearly 0 (-0.009) — delivery speed alone does not significantly impact ratings

🔄 Customer Loyalty
81.8% of orders are from returning customers, indicating strong retention
RFM Segmentation breakdown:
🏆 Champions — 1,865 customers (37.3%)
💛 Loyal Customers — 2,469 customers (49.4%)
⚠️ At Risk — 666 customers (13.3%)

 
