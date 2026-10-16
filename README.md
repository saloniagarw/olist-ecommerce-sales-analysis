# 📦 Olist E-Commerce Sales & Customer Experience Analysis
An end-to-end Exploratory Data Analysis (EDA) project leveraging Python to extract actionable business insights from the Brazilian Olist e-commerce public dataset, focusing on revenue trends, customer purchasing behavior, and logistics performance.

---

<p align="center">
  <a href="#executive-summary">Overview</a> •
  <a href="#key-findings">Key Findings</a> •
  <a href="#visual-insights">Visualizations</a> •
  <a href="#key-analysis-areas">Methodology</a> •
  <a href="#project-notebook--structure">Notebook</a>
</p>

---

## 🚀 Executive Summary & Key Findings
* **Total Revenue & Scale:** Analyzed over 99,000 orders spanning multiple years, uncovering a total item revenue of **~13.59M BRL** with peak seasonal spikes in late Q4 (notably November 2017).
* **Delivery Reliability:** **91.89%** of eligible delivered orders arrived on time, with an average purchase-to-delivery cycle of **12.56 days** (median: 10.22 days).
* **Customer Retention Challenge:** Identified a repeat-customer rate of **3.12%**, signaling a major growth opportunity for post-purchase lifecycle marketing and loyalty initiatives.
* **Freight Impact:** Freight costs averaged **16.57%** of total item revenue, highlighting areas for supply chain and packaging optimization.

---

## 📌 Key Business Metrics

<table>
  <tr>
    <td align="center" width="50%">
      <h3>BRL 13.59M</h3>
      <b>Total Item Revenue</b>
    </td>
    <td align="center" width="50%">
      <h3>91.89%</h3>
      <b>On-Time Delivery Rate</b>
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <h3>12.56 Days</h3>
      <b>Average Delivery Time</b>
    </td>
    <td align="center" width="50%">
      <h3>3.12%</h3>
      <b>Repeat Customer Rate</b>
    </td>
  </tr>
</table>

---

## 🎯 Project Objectives
- **Sales & Revenue Dynamics:** Track Month-over-Month (MoM) growth and identify seasonal revenue drivers.
- **Geographic Concentration:** Evaluate order distribution, volume, and cancellation rates across Brazilian states (e.g., high concentration in SP, RJ, MG).
- **Logistics & Delivery Performance:** Contrast estimated vs. actual delivery timelines to uncover bottlenecks.
- **Financial Metrics:** Analyze Average Order Value (AOV), item pricing distributions, and freight-to-price ratios.
- **Customer Segmentation:** Distinguish between one-time buyers and repeat purchasers to evaluate retention.

---

## 🛠️ Tools & Technologies
* **Programming Language:** Python 
* **Data Manipulation & Calculation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook

---

## 📂 Key Analysis Areas
1. **Data Preprocessing & Cleaning:** Handled missing timestamps (`NaT` preservation for unapproved/canceled orders), validated data types, and merged relational schemas (`customers`, `orders`, `order_items`).
2. **Order Status Distribution:** Categorized fulfillment states (delivered, shipped, canceled, unavailable, etc.).
3. **Logistics Performance Analysis:** Calculated delivery durations and classified orders into *On-Time* vs. *Late* benchmarks.
4. **Pricing & Shipping Cost Evaluation:** Evaluated item pricing structures alongside freight expenditures.
5. **Customer Behavior & Retention:** Measured unique customer frequencies to evaluate the true repeat purchase rate.

---
## 📊 Visual Insights

<table>
  <tr>
    <td align="center" width="50%">
      <b>Monthly Orders & Revenue Trend</b><br><br>
      <img src="./Monthly%20Orders%20and%20revenue%20Trend.png" alt="Monthly Orders and Revenue Trend" width="100%">
    </td>
    <td align="center" width="50%">
      <b>Top 10 States by Orders</b><br><br>
      <img src="./Top%2010%20states%20by%20number%20of%20Orders.png" alt="Top 10 States by Orders" width="100%">
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <b>Shipping Cost vs Product Price</b><br><br>
      <img src="./shipping_cost_vs_product_price.png" alt="Shipping Cost vs Product Price" width="100%">
    </td>
    <td align="center" width="50%">
      <b>Correlation Heatmap</b><br><br>
      <img src="./correlation_heatmap.png" alt="Correlation Heatmap" width="100%">
    </td>
  </tr>
</table>

---


## 💡 Business Insights

<details>
  <summary><b>📦 Sales & Regional Performance</b></summary>

  - Analyze monthly order and revenue trends.
  - Compare order distribution across customer states.
  - Identify high-volume regions for further investigation.

</details>

<details>
  <summary><b>🚚 Delivery & Logistics</b></summary>

  - Evaluate on-time versus late deliveries.
  - Study delivery duration and shipping costs.
  - Identify logistics areas that may need improvement.

</details>

<details>
  <summary><b>💰 Pricing & Customer Behavior</b></summary>

  - Examine product prices against freight charges.
  - Explore correlations among price, freight, and delivery time.
  - Analyze repeat purchasing behavior.

</details>

---

## 📑 Project Notebook & Structure
The complete data pipeline, code execution, visual charts, and detailed business recommendations are documented in:
👉 [`Olist_Ecommerce_Analysis_with_Business_Insights.ipynb`](./Olist_Ecommerce_Analysis_with_Business_Insights.ipynb)

---

## 📊 Dataset Notice
This project utilizes the **Brazilian E-Commerce Public Dataset by Olist**, hosted publicly on Kaggle. *Note: Raw CSV dataset files are excluded from this repository due to file size constraints.* To run the notebook locally, download the dataset from Kaggle and update your local file paths accordingly in Section 1.

---

## 👤 Author
**Saloni Agarwal**
