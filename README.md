# Energix Energy_Market_Resilience_Metrics KPI & Performance Analysis

- Energix Enterprise is a prominent player in the Energy and Utilities sector, specializing in electricity generation and distribution across various regions. With a diversified energy portfolio encompassing both fossil fuels and renewable sources, the company has been a vital contributor to the energy landscape for over two decades.
- This project analyzes historical energy data, market trends, infrastructure, and regulatory changes for Energix Enterprise. It calculates key performance indicators (KPIs) and visualizes the results to provide insights into operational efficiency, market competitiveness, and compliance risks.

---

## Purpose of the Analysis

The goal is to provide a data-driven understanding of the company's performance by focusing on four key areas:
1.  **Supply & Demand:** Investigating the gap between energy production and market demand.
2.  **Renewable Energy:** Comparing the adoption of renewable energy across different regions.
3.  **Regulatory Impact:** Assessing the financial and operational effects of new regulations.
4.  **Infrastructure Limitations:** Exploring the relationship between technology status and production efficiency.

---

## Data Sources
* `historical_energy_data.csv`
* `infrastructure_data.csv`
* `market_data.csv`
* `regulatory_data.csv`

---

## Steps Used

1.  **Import of .csv File:** Importing .csv file in Notebook
2.  **Exploratory Data Analysis:** Performing EDA to correct Date/Time format and imputation.
3.  **Merging all Cleaned Datasets:** Merging all the 4 datasets to make one dataset for analysis and calculations.
4.  **KPIs selection** Finding and selecting important KPIs suitable for solving the business problems.
5.  **KPI Integration to Dataset** Integrating KPI as columns into the dataset with corresponding rows
6.  **Visualisation** Analysis through data visualisation.
7.  **File import** Importing merged KPI dataset
---

## Key Performance Indicators (KPIs) Used

The following KPIs were calculated from the merged datasets:
* **Production Efficiency**
* **Cost per kWh**
* **Demand Gap**
* **Compliance Cost Ratio**
* **Tech Limitation Score**

---

## Visualizations and Key Conclusions

### Demand Gap Over Time
![Demand Gap Over Time](visualisation/demand_gap_plot.png)  
**Analysis:** 
- The company consistently experiences periods of both energy surplus and energy deficit. This indicates that Energix Enterprise is not effectively matching its energy production with market demand.

**Conclusion:**
- The company experiences significant volatility in its supply and demand, indicating a need for better forecasting and production planning.

### Cost per kWh vs. Regulation Impact
![Cost per kWh vs. Regulation Impact](visualisation/cost_per_kwh_vs_regulation.png)  
**Analysis:** 
- The median for "Regulation Impact" appears to be slightly higher than the median for "No Regulation Impact.
- The box and whiskers for the "Regulation Impact" group are noticeably longer and more spread out.

**Conclusion:** 
- While the difference in typical cost might be small, regulatory changes introduce a significant amount of financial instability and risk into the company's cost structure.

### Compliance cost vs. Regulation Impact
![Compliance cost vs. Regulation Impact](https://github.com/Sivaan66/Energy_Market_Resilience_Metrics--Analyzing_Vulnerabilities.Python-/blob/0a81867684486b2e0f1c6ce38acefa677fa734be/Visualisation/compliance_cost_plot.png)  
**Analysis:** The compliance cost of the company changes dramatically over regulations. It reaches the spike at the time of regulatory impacts.  

**Conclusion:** 
- Indicates that  company needs a more proactive strategy to manage compliance and its associated costs, rather than reacting to each new regulation as it occurs.

### Tech limitation vs compliance cost
![Tech limitation vs compliance cost](visualisations/tech_limitation_vs_compliance_cost.png)   
**Analysis:** 
- When the Tech Limitation Score is low (at 1 on the x-axis), the compliance costs are also generally low and not widely scattered. 
- As the Tech Limitation Score increases, the costs become much more unpredictable. At a score of 2, the compliance costs show a wide range of values.
- At a score of 3 (high tech limitation), the compliance costs are consistently very high.

**Conclusion:**
- The plot strongly suggests a positive correlation between technology limitations and compliance costs.
- **This provides clear evidence that modernizing your infrastructure is not just about efficiency but is also a critical factor in controlling regulatory expenses.**

---

## How to Run the Code

1.  Make sure you have **Python**, **pandas**, and **matplotlib** installed.
2.  Place all `.csv` files and the Python script in the same folder.
3.  Run the script from your terminal: `python your_script_name.py`.
4.  The script will generate new CSV and image files in a `visualizations` folder.
