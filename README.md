# data-analysis
Analyzing e-commerce sales performance and customer value tiers using Pandas, RFM modeling, and Power BI dashboards.


An end-to-end data analytics project analyzing e-commerce retail transactions to uncover revenue trends, top-selling product categories, and high-value customer segments using Python and Power BI.

---

Project Overview
In the competitive retail landscape, understanding customer behavior and revenue drivers is critical for business growth. This project tackles an e-commerce dataset to answer key strategic questions:
* What are the primary seasonal revenue trends and peak sales periods?
* Which products generate the highest gross revenue?
* How can we segment customers using **RFM (Recency, Frequency, Monetary)** analysis to identify VIPs versus at-risk accounts?

---

Tech Stack & Tools
* Data Cleaning & Feature Engineering: Python (Pandas)
* Customer Segmentation: RFM Modeling (Recency, Frequency, Monetary scoring)
* Data Visualization & Reporting: Power BI 
* Version Control: Git & GitHub

---

Project Workflow & Methodology

1. Data Cleaning & Validation:
   * Filtered out order cancellations and returns (rows marked with invoice prefix 'C' and negative quantities).
   * Removed invalid transactional entries (zero or negative unit prices).
   * Cleaned and handled missing customer identification keys.

2. Feature Engineering:
   * Generated a `TotalSales` metric ($\text{Quantity} \times \text{UnitPrice}$).
   * Extracted temporal components (`YearMonth`, `DayOfWeek`, `Hour`) to analyze shopping habits.
   * Engineered **RFM Metrics** for each customer to evaluate purchasing recency, frequency, and monetary value.
   * Assigned quartile scores ($1$ to $4$) to segment customers into actionable tiers (*VIP / Champions*, *Loyal Customers*, *At-Risk*, and *Low-Value*).

3. Dashboard & Visualizations:
   * **Executive KPIs:** Total Revenue, Total Orders, and Active Customer Count.
   * **Monthly Revenue Trend:** Line chart tracking revenue growth and holiday purchasing spikes.
   * **Top Products Bar Chart:** Highlighting the highest-earning inventory items.
   * **Customer Segment Breakdown:** Visualizing the distribution of customer tiers.

---

## Key Insights & Findings
* Seasonality Spikes: Revenue surges significantly during the fourth quarter (specifically October through December), driven by holiday shopping behavior.
* Product Concentration: A small percentage of top-tier giftware items account for the majority of gross revenue.
* Customer Value Distribution: RFM segmentation reveals that a core segment of "Champions" drive repeat transactions, while targeted retention strategies are needed for "At-Risk" segments.

---

Dashboard Preview
<img width="830" height="467" alt="image" src="https://github.com/user-attachments/assets/13fc97e9-683a-463f-94a4-a5e5ab9e275f" />

<img width="620" height="397" alt="image" src="https://github.com/user-attachments/assets/549c1fb7-0017-496b-95ad-59083e403d7c" />

<img width="697" height="384" alt="image" src="https://github.com/user-attachments/assets/eec5dee8-18ca-4a67-a8e7-e1796b7cfc08" />

Code link: https://colab.research.google.com/drive/1lsHOf3uMsmixffjRquTy4XAI0ao2RZHv?usp=sharing
