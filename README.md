# OptiStock: Inventory Policy & EOQ Logistics Optimization
**Author:** Miguel A. Martinez | Business Intelligence Analyst  
**Interactive Deliverable:** [Live Tableau Dashboard Simulator](https://public.tableau.com/views/OptiStockEOQSimulator/OptiStockEOQSimulator?:language=es-ES&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

---

## Business Context & Objective
In retail supply chain management, balancing inventory holding costs against transactional ordering costs is a critical driver of profitability. This business case evaluates the historical demand of a high-turnover Walmart product from the M5 Forecasting Dataset to establish an optimal inventory replenishment policy. 

The primary objective is to transition from deterministic stock tracking into a dynamic, data-driven framework by calculating the **Economic Order Quantity (EOQ)** under volume discount tiers and setting a probabilistic **Reorder Point (ROP)** to mitigate stockout risks.

## Data-to-Decision Pipeline
The project follows a structured business intelligence lifecycle:
1. **Data Analytics & Engineering (Kaggle Backend):** Time-series sales data and pricing structures were processed using Python (Pandas/NumPy) to aggregate annual demand and determine daily demand volatility.
2. **Semantic Layer Export:** The continuous cost curves and business variables were structured into a single source of truth (`tableau_dashboard_master.csv`).
3. **Executive Visualization (Tableau Frontend):** Built an interactive management simulator that empowers stakeholders to stress-test financial scenarios (holding costs, lead times, and discount rates) without interacting with raw data.

## Strategic Insights & Business Impact
* **Cost Optimization:** The mathematical model identified that shifting from small-batch ordering to an optimal batch size of **300 units** captures a 12% supplier discount, minimizing the Total Inventory Cost (TIC) to **$3,100.03 USD** annually.
* **Risk Mitigation:** Incorporating a 95% service level factor established a safety stock requirement, setting the automated **Reorder Point at 23 physical units** to prevent costly operational stockouts.

## Repository Structure
* `bi-logistics-eoq-optimization-walmart.ipynb`: Data extraction, statistical demand analytics, and financial modeling.
* `tableau_dashboard_master.csv`: Cleaned dataset powering the BI solution.
* `README.md`: Executive summary and project documentation.

---
*Note: This project is an academic and professional case study modeled with simulated financial parameters for educational and portfolio purposes.*
