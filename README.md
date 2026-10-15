# 🛍️ Olist E-Commerce Sales & Customer Experience Analysis

### Turning E-Commerce Data into Business Insights with Python

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-013243?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Visualization-4c72b0)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)

> An exploratory data analysis project investigating e-commerce sales trends, customer purchasing behavior, shipping costs, and delivery performance to generate actionable business insights.

## 📌 Table of Contents

- [Overview](#-overview)
- [Business Objectives](#-business-objectives)
- [Key Features and Methodology](#-key-features-and-methodology)
- [Project Structure](#-project-structure)
- [Key Findings and Visualizations](#-key-findings-and-visualizations)
- [Business Recommendations](#-business-recommendations)
- [Technology Stack](#-technology-stack)
- [Getting Started](#-getting-started)
- [Future Improvements](#-future-improvements)
- [Dataset and Acknowledgments](#-dataset-and-acknowledgments)
- [Author](#-author)

## 📖 Overview

The **Olist E-Commerce Sales & Customer Experience Analysis** project explores Brazilian e-commerce order data to understand sales performance, customer purchasing patterns, shipping costs, and delivery reliability.

Using Python and its data analysis ecosystem, customer, order, and order-item datasets are examined and combined to support meaningful business analysis.

The project goes beyond generating charts by connecting analytical findings to practical recommendations that could help e-commerce businesses improve operational efficiency, understand customer behavior, and make informed decisions.

## 🎯 Business Objectives

- Analyze monthly order volume and revenue trends.
- Identify high-performing customer regions.
- Evaluate order status and cancellation patterns.
- Measure delivery timelines and on-time delivery performance.
- Calculate Average Order Value (AOV).
- Understand repeat purchasing behavior.
- Examine shipping costs relative to product prices.
- Translate findings into actionable business recommendations.

## 🔍 Key Features and Methodology

### 1. Data Exploration and Cleaning
- Inspected dataset structure, data types, duplicate records, and missing values.
- Converted timestamp columns into datetime formats.
- Evaluated missing timestamps in the context of order status.
- Preserved missing values where filling them could introduce misleading information.

### 2. Data Integration
- Combined customer, order, and order-item datasets using relational keys.
- Checked identifiers, missing item records, and duplicate order-item combinations.
- Distinguished order-level metrics from item-level metrics to avoid inflated order counts.

### 3. Sales and Revenue Analysis
- Analyzed monthly order volume and item-price revenue.
- Calculated month-over-month revenue growth.
- Compared sales performance across customer states.
- Examined order-value distributions and Average Order Value.

### 4. Customer Behavior Analysis
- Used unique customer identifiers to analyze purchasing behavior.
- Calculated the observed repeat-customer rate.
- Compared one-time and repeat purchasing behavior.

### 5. Logistics and Delivery Analysis
- Calculated purchase-to-delivery time.
- Compared actual delivery dates against estimated delivery dates.
- Evaluated on-time and late delivery proportions.
- Examined freight charges relative to item prices.

### 6. Visualization and Business Interpretation
- Line charts for monthly trends.
- Bar charts for regional and order-status comparisons.
- Histograms for order-value and delivery-time distributions.
- Scatter plots for shipping-cost relationships.
- Correlation heatmap for numerical relationships.
- Business insights and actionable recommendations alongside analyses.

## 🗂️ Project Structure

```text
olist-ecommerce-sales-analysis/
│
├── README.md
├── requirements.txt
├── notebooks/
│   └── Olist_Ecommerce_Analysis_with_Business_Insights.ipynb
├── images/
│   ├── monthly-sales-trend.png
│   ├── delivery-performance.png
│   ├── customer-retention.png
│   └── correlation-heatmap.png
└── data/
    └── README.md
```

*This is the intended structure. Add the folders and files as you create them, or update the structure to match your actual repository.*

## 📊 Key Findings and Visualizations

The following metrics summarize the current analysis and should be interpreted using the definitions implemented in the notebook.

| Metric | Result | Interpretation |
|---|---:|---|
| Average Order Value | **137.75 BRL** | Average sum of item prices per order, excluding freight |
| On-Time Delivery Rate | **91.89%** | Share of eligible delivered orders arriving by the estimated date |
| Average Purchase-to-Delivery Time | **12.56 days** | Average elapsed time from purchase to customer delivery |
| Repeat-Customer Rate | **3.12%** | Share of observed unique customers with more than one order |

### 📈 Monthly Sales and Revenue Trends

![Monthly sales and revenue trend](images/monthly-sales-trend.png)

**Business question:** How do order volume and item-price revenue change over time?

**What to investigate:** Revenue peaks, seasonal patterns, and months where revenue changes differently from order volume.

### 🚚 Delivery Performance

![Delivery performance](images/delivery-performance.png)

**Business question:** How reliably are delivered orders meeting their estimated delivery dates?

**What to investigate:** Late deliveries, regional differences, and opportunities to improve delivery estimates.

### 👥 Customer Retention

![Customer retention](images/customer-retention.png)

**Business question:** How many unique customers place repeat orders during the observed period?

**What to investigate:** Potential opportunities for post-purchase engagement, loyalty initiatives, and customer win-back campaigns.

### 🔥 Correlation Analysis

![Correlation heatmap](images/correlation-heatmap.png)

**Business question:** Which numerical variables show relationships worth investigating further?

**Interpretation:** Correlation indicates association, not causation. Delivery time should ideally be analyzed at the order level rather than on duplicated item-level rows.

*Note: The image paths above are placeholders. Save your actual charts with these filenames in the `images/` folder, or update the paths to match your files.*

## 💡 Business Recommendations

### Improve Delivery Reliability
Investigate late deliveries by customer state and seller to identify recurring operational issues. Use delivery-time patterns to refine estimated delivery dates and customer communication.

### Encourage Repeat Purchasing
Evaluate post-purchase communication, relevant product recommendations, and loyalty initiatives. Measure changes in repeat purchasing over time before concluding that an initiative is effective.

### Optimize Shipping Costs
Identify orders where freight is high relative to item price. Explore packaging improvements, carrier negotiations, or carefully tested shipping offers while monitoring profitability.

### Make Revenue Analysis More Actionable
Investigate high-performing months and compare revenue with order volume and AOV. Use recurring patterns to inform campaign timing and inventory planning.

### Evaluate Promotions Responsibly
Use AOV as a baseline for testing bundles and cross-selling. Assess margins and overall financial impact rather than treating increased order value alone as proof of success.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data manipulation, cleaning, and aggregation |
| NumPy | Numerical calculations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Jupyter Notebook | Interactive analysis and documentation |

## 🚀 Getting Started

### Prerequisites

Install Python 3 and Git. Familiarity with Python and Jupyter Notebook is helpful.

### 1. Clone the Repository

```bash
git clone https://github.com/saloniagarw/olist-ecommerce-sales-analysis.git
cd olist-ecommerce-sales-analysis
```

### 2. Create and Activate a Virtual Environment

```bash
python -m venv .venv
```

On Windows:

```bash
.venv\Scripts\activate
```

On macOS or Linux:

```bash
source .venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Download the Dataset

Download the Brazilian E-Commerce Public Dataset by Olist from Kaggle:

https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

Place the required CSV files in the `data/` directory and ensure their filenames and paths match those referenced in the notebook. Update the notebook paths if necessary.

### 5. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the notebook in the `notebooks/` directory and execute the cells in order.

**Important:** Confirm that the notebook's CSV file paths work on your machine before running the full analysis.

## 🗺️ Future Improvements

- Build an interactive dashboard using Power BI, Tableau, or Streamlit.
- Add seller-level and product-category performance analysis.
- Investigate factors associated with late deliveries and cancellations.
- Extend customer analysis with cohort retention and repeat-purchase timing.
- Add automated data-quality checks and reusable analysis functions.
- Incorporate available payment and cost data to develop more complete profitability measures.

## 📂 Dataset and Acknowledgments

This project uses the Brazilian E-Commerce Public Dataset by Olist, available on Kaggle:

**Dataset:** https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

Please refer to the dataset page for its description and applicable terms.

## 👨‍💻 Author

**Parv Agarwal**

- GitHub: https://github.com/saloniagarw
- LinkedIn: https://www.linkedin.com/in/parv-agarwal-09b042215/

---

⭐ If you find this project useful, consider starring the repository.

*This project was created for learning, exploratory analysis, and portfolio demonstration. The recommendations are hypotheses for further investigation, not evidence of causal business impact.*
