# Retention and Sales Analysis


The goal is to analyze sales and payment data using SQL, perform customer behavior and retention analysis, and visualize retention insights using Power BI.

---

## 🗂️ Datasets

- `customer_orders.csv` — Order data including order date, status, and amount
- `payments.csv` — Payment data including method, status, and amount

---

## 🧮 SQL Query Tasks

### ✅ Task 1: Order and Sales Analysis

- Count of orders by status
- Monthly revenue trends (completed payments only)
- Order fulfillment rate (delivered orders vs total)
- Average Order Value (AOV)

### ✅ Task 2: Customer Analysis

- Total orders per customer
- Repeat customer count and repeat rate
- Monthly trend of unique customers

### ✅ Task 3: Payment Status Analysis

- Breakdown of payment statuses
- Payment method vs status distribution
- Payment failure rate

### ✅ Task 4: Order Details Report

- Combined report using a `LEFT JOIN` on `customer_orders` and `payments`
- Fields include customer info, order status, payment amount, and status

> All SQL queries can be found in the Summary.doc

---

## 📈 Visualization Task — Customer Retention Analysis (Task 5)

Built in **Power BI** using cohort-based analysis.

- Customers are grouped by their **first purchase month (cohort)**
- Tracked monthly over time to show **retention behavior**
- Matrix format:
  - **Rows** = First Order Month (Cohort)
  - **Columns** = Months Since First Purchase
  - **Values** = % of customers who made repeat purchases
- Includes **heatmap-style conditional formatting** to show retention decay

> 📁 Power BI file: `CustomerRetentionAnalysis.pbix`  
> 📸 Exported image: `retention_matrix.png`

---

## 📝 Summary of Key Insights

- **Fulfillment Rate**: ~33.7% of orders have been delivered
- **Repeat Customer Rate**: ~60% of customers placed more than one order
- **Payment Failures**: Roughly 33.3% of all payments failed
- **Retention**: Most cohorts see sharp drop-off after the first 1–2 months, indicating a potential need for re-engagement strategies

---

## ✅ Recommendations

- Improve payment success rates — investigate top failing payment methods
- Increase fulfillment by optimizing shipment logistics
- Launch email/SMS follow-ups for cohorts showing early drop-off
- Offer incentives for second and third purchases to increase retention



