# **Retail Vibe Analytics — Local Notebook Edition**



Audience: Technical and business decision makers

Dataset: Olist Brazilian E-Commerce (Kaggle) — loaded from local CSV files into a Python notebook



---

## Getting Started: Dataset Setup



**Step 1: Download the dataset**

Go to [https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) and click **Download** (you'll need a free Kaggle account). This downloads a file called `archive.zip` (approximately 45 MB).



**Step 2: Unzip the data**

Unzip `archive.zip` into a folder on your laptop. You should see the following CSV files:

- `olist_customers_dataset.csv`
- `olist_orders_dataset.csv`
- `olist_order_items_dataset.csv`
- `olist_order_payments_dataset.csv`
- `olist_order_reviews_dataset.csv`
- `olist_products_dataset.csv`
- `olist_sellers_dataset.csv`
- `olist_geolocation_dataset.csv`
- `product_category_name_translation.csv`



**Step 3: Open a Python notebook**

Create a new Jupyter notebook (or open one in VS Code) in the same folder where you unzipped the CSV files. Make sure you have `pandas`, `matplotlib`, `seaborn`, and `plotly` installed:

```bash
pip install pandas matplotlib seaborn plotly scikit-learn statsmodels
```

You're ready to go. Start prompting the AI in your notebook.



---



###### Act 1 — Orient and Explore (3–5 min)



  **Prompt 1: Schema Discovery**



  *I have a set of CSV files from the Olist Brazilian E-Commerce dataset in the same folder as this notebook. Load them all into DataFrames and tell me about them.*



  **Purpose: Show that the AI can introspect the local CSV files, describe tables, row counts, and relationships with zero upfront context.**



  **Prompt 2: Star Schema + KPI Snapshot**



  *Create a star-style merged DataFrame that joins orders, customers, items, payments, and products. Then generate a KPI snapshot: total revenue, total orders, avg order value, avg delivery days, and review score.*



  **Purpose: Demonstrate data modeling on-the-fly and instant executive summary.**



---



##### Act 2 — Visual Dashboard (5–7 min)



  **Prompt 3: Multi-Chart Dashboard**



  *Create a dashboard-style cell with monthly revenue trend, a state-level heatmap of order volume, and a payment method mix donut chart.*



  **Purpose: Wow moment — a full dashboard from a single sentence. Great for business stakeholders.**



  **Prompt 4: Refine and Polish**



  *Make the revenue trend chart a dual-axis showing both revenue and order count. Add a 3-month rolling average line. Use a clean, professional color palette.*



  **Purpose: Show iterative refinement — "vibe coding" in action. Proves the tool is conversational, not one-shot.**



---



##### Act 3 — Business Deep-Dives (7–10 min)



  **Prompt 5: Customer Segmentation (RFM)**



  *Build an RFM segmentation (Recency, Frequency, Monetary) for all customers. Assign each customer to a segment like Champions, Loyal, At Risk, Lost, etc. Show segment counts and avg revenue per segment in a single visual.*



  **Purpose: Classic analytics use case that normally takes hours. Shows value for marketing/CRM teams.**



  **Prompt 6: Delivery Performance Analysis**



  *Analyze delivery performance: what percentage of orders arrived late vs. early? Which states have the worst on-time delivery rates? Show a bar chart of avg delivery delay (actual vs estimated) by state, sorted worst-to-best.*



  **Purpose: Operations/logistics angle — appeals to COO types. Uses date math and spatial grouping.**



  **Prompt 7: Product Category Insights**



  *What are the top 10 product categories by revenue? For each, show the average review score and average delivery time. Highlight any categories where high revenue coincides with low review scores — those are risk areas.*



  **Purpose: Cross-functional insight (product + CX + ops). Demonstrates the AI can surface non-obvious business risks.**



---



###### Act 4 — Advanced / Predictive (5–7 min)



  **Prompt 8: Review Sentiment and Drivers**



  *Analyze review scores: what factors most influence whether a customer leaves a 1-star vs 5-star review? Consider delivery time, product category, payment type, and order value. Show a correlation heatmap and summarize key drivers.*



  **Purpose: Shows the AI can do exploratory statistical analysis, not just reporting.**



  **Prompt 9: Cohort Retention Analysis**



  *Create a monthly cohort analysis: group customers by their first purchase month, then show what percentage made a repeat purchase in subsequent months. Display as a retention heatmap.*



  **Purpose: Sophisticated analysis that typically requires a data scientist. Big impact for growth/product teams.**



  **Prompt 10: Revenue Forecasting**



  *Using the monthly revenue trend, fit a simple forecast model and project revenue for the next 6 months. Show the historical data, forecast, and confidence interval on a single chart.*



  **Purpose: Predictive analytics from a plain-English prompt. Strong closer for exec audiences.**



---



###### Act 5 — Wrap-Up / Freestyle (2–3 min)



  **Prompt 11: Executive Summary**



  *Summarize everything we've found into a concise executive briefing: top 5 insights, top 3 risks, and top 3 recommended actions. Format it as a clean markdown report I could email to leadership. Include an impactful visual for each area.*



  **Purpose: Demonstrates the AI can synthesize an entire analysis session into an actionable deliverable.**



  **Prompt 12: Audience Q&A / Freestyle**



  *(Don't show this prompt — use it live based on audience questions)*



  *Ask the audience: "What would YOU like to explore in this data?"*



  **Purpose: Most impressive moment — live, unscripted analysis driven by the room. Shows this is not canned.**
