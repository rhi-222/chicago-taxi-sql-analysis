# Analyzing Ride-Sharing Trends in Chicago: SQL & Data Collection Project

## Table of Contents
- [Overview](#overview)
- [Business Problem](#business-problem)
- [Dataset](#dataset)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Hypothesis Testing](#hypothesis-testing)
- [Key Insights & Business Impact](#key-insights--business-impact)
- [Next Steps & Improvements](#next-steps--improvements)
- [How to Use](#how-to-use)
- [Connect With Me](#connect-with-me)

---

## Overview
This project analyzes **ride-sharing data in Chicago** using **SQL queries and Python-based data analysis**. The objective is to identify trends in taxi usage, determine the impact of weather on ride frequency, and provide insights for **Zuber**, a new ride-sharing company entering the market.

## Business Problem
Zuber wants to understand:
- **Passenger preferences** (popular routes, frequent taxi companies)
- **Competitive landscape** (which taxi companies dominate the market)
- **Weather impact** (does bad weather affect ride duration and frequency?)

By leveraging **SQL** and **Python**, we extract insights that can **inform business decisions** and **optimize ride-sharing services**.

---

## Dataset
The project uses a **relational database** containing four key tables:

- **neighborhoods** – Chicago neighborhood names & IDs.
- **cabs** – Taxi company details and vehicle information.
- **trips** – Ride details (pickup/dropoff locations, duration, timestamps).
- **weather_records** – Hourly weather conditions (temperature, descriptions).

Additionally, **three extracted datasets** were analyzed in Python:
1. `project_sql_result_01.csv` – Taxi companies & ride counts (Nov 15-16, 2017).
2. `project_sql_result_04.csv` – Average trip counts per neighborhood.
3. `project_sql_result_07.csv` – Rides from Loop to O’Hare & weather impact.

All datasets are stored in the **`data/`** folder for easy access.

---

## Exploratory Data Analysis (EDA)
### **Key Findings**
- **Most Active Taxi Companies:**  
  - **Flash Cab** and **Taxi Affiliation Services** had the highest ride counts.
  - Companies with "Yellow" or "Blue" in their names had significant market share.

- **Popular Drop-off Locations:**  
  - The top 10 neighborhoods for drop-offs were identified.
  - Downtown and airport locations dominated ride activity.

- **Weather Impact on Ride Counts:**  
  - Rain and storms led to **fluctuations in ride demand**.
  - Certain taxi companies experienced **higher demand during bad weather**.

---

## Hypothesis Testing
### **Hypothesis:**  
_"The average duration of rides from the Loop to O’Hare International Airport changes on rainy Saturdays."_

- **Null Hypothesis (H₀):** Weather does not affect ride duration.
- **Alternative Hypothesis (H₁):** Ride duration is affected by weather.

**Method:**  
- Performed **statistical testing** (t-test) on ride durations during "Good" and "Bad" weather conditions.
- Used **Python's SciPy library** to calculate **p-values** and determine statistical significance.

**Results:**  
- The test **found no strong evidence** that rain significantly impacts ride duration.
- However, variability in travel times suggests other external factors (traffic, demand) may play a role.

---

## Key Insights & Business Impact
- **Taxi Market Concentration:** A few companies dominate the ride-sharing space.
- **Weather Considerations:** While rain doesn’t **drastically** affect ride duration, it **may impact ride availability**.
- **Neighborhood Hotspots:** Business districts and airports are **prime locations** for ride demand.

### **Business Recommendations**
- **Strategic Partnerships** – Partner with top taxi companies for competitive positioning.  
- **Dynamic Pricing Models** – Adjust pricing based on **weather conditions** and **peak demand hours**.  
- **Focus on High-Demand Areas** – Prioritize **airport routes** and **downtown locations** for expansion.  

---

## Next Steps & Improvements
- **Deeper Analysis of Ride Duration Trends:** Explore the impact of **traffic congestion** on ride duration.  
- **Expand Dataset Scope:** Incorporate **rideshare data from Lyft/Uber** for a broader comparison.  
- **Develop a Real-Time Ride Forecasting Model:** Predict demand spikes based on **weather & location trends**.  

---

## How to Use
### Clone the repository:
    git clone https://github.com/rhi-222/sql-data-collection.git

### Install dependencies:
    pip install pandas numpy matplotlib seaborn scipy
    
### Run the Jupyter Notebook:
- Open `DataCollection(SQL).ipynb` in Jupyter Notebook.
- Execute the notebook to analyze SQL query results, generate insights, and visualize trends.

## Connect With Me
📧 Email: rhiannon.filli@gmail.com

💼 LinkedIn: linkedin.com/in/rhiannonfilli
