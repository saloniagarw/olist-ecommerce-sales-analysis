# 📦 Olist E-Commerce Sales & Customer Experience Analysis
An end-to-end Exploratory Data Analysis (EDA) project leveraging Python to extract actionable business insights from the Brazilian Olist e-commerce public dataset, focusing on revenue trends, customer purchasing behavior, and logistics performance.

---

## 🚀 Executive Summary & Key Findings
* **Total Revenue & Scale:** Analyzed over 99,000 orders spanning multiple years, uncovering a total item revenue of **~13.59M BRL** with peak seasonal spikes in late Q4 (notably November 2017).
* **Delivery Reliability:** **91.89%** of eligible delivered orders arrived on time, with an average purchase-to-delivery cycle of **12.56 days** (median: 10.22 days).
* **Customer Retention Challenge:** Identified a repeat-customer rate of **3.12%**, signaling a major growth opportunity for post-purchase lifecycle marketing and loyalty initiatives.
* **Freight Impact:** Freight costs averaged **16.57%** of total item revenue, highlighting areas for supply chain and packaging optimization.

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

## 📑 Project Notebook & Structure
The complete data pipeline, code execution, visual charts, and detailed business recommendations are documented in:
👉 [`Olist_Ecommerce_Analysis_with_Business_Insights.ipynb`](./Olist_Ecommerce_Analysis_with_Business_Insights.ipynb)

---

## 📊 Dataset Notice
This project utilizes the **Brazilian E-Commerce Public Dataset by Olist**, hosted publicly on Kaggle. *Note: Raw CSV dataset files are excluded from this repository due to file size constraints.* To run the notebook locally, download the dataset from Kaggle and update your local file paths accordingly in Section 1.

---

## 👤 Author
**Saloni Agarwal**
