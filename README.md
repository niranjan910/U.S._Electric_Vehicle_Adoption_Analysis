# U.S. Electric Vehicle (EV) Adoption Analysis

- **Author:** Niranjan  
- **Date:** 22 June 2025

---

## Project Workflow & Steps

This section outlines the complete process and technical steps taken during the project to showcase the end-to-end workflow:

### 1. Data Acquisition

- Obtained the real-world dataset **`EvolutionInsight_US_EV_Trends.csv`** containing U.S. electric vehicle adoption data.
- Dataset was stored locally in a structured project folder.

### 2. Database Setup & Connection

- Created a new MySQL database named **`U_S_Electric_Vehicle_Adoption_Analysis`** to store and manage data.
- Used MySQL Workbench to create and verify the database and tables.

### 3. Data Loading via Python

- Used **Python** with libraries such as `pandas`, `sqlalchemy`, and `pymysql` for database interaction.
- Loaded the CSV data into a pandas DataFrame.
- Cleaned column names by removing spaces and special characters for consistency.
- Established a MySQL connection in Python using SQLAlchemy's `create_engine`.
- Uploaded the cleaned DataFrame into MySQL as a table named **`ev_trends_data`**.
- Verified the data upload using SQL queries in MySQL Workbench.

### 4. Data Exploration & Validation in MySQL

- Performed basic SQL queries to explore data structure and content, such as:
  - Checking total row count.
  - Inspecting column data types and names.
  - Previewing data samples.
  - Calculating summary statistics for numeric columns using aggregate functions with proper handling of column names containing spaces.
  - Counting distinct values for categorical variables.
  - Identifying missing values in key columns with conditional aggregation.

### 5. Jupyter Notebook for Analysis

- Created a dedicated Jupyter Notebook for hands-on data analysis.
- Loaded data directly from both the CSV file and MySQL database into pandas DataFrames.
- Utilized pandas for detailed data profiling, including `.describe()`, `.info()`, and categorical value counts.
- Maintained reproducible documentation within the notebook, including code and markdown explanations.

### 6. Insights & Reporting

- Used SQL and pandas analysis results to identify EV adoption hotspots, incentive effectiveness, vehicle trends, and demographic insights.
- Summarized findings and strategic recommendations for infrastructure planning and policy adjustments.
- Compiled the entire analysis into well-documented Python notebooks, supporting visualization and future scalability.

---

## Project Background

This capstone project leverages Python and SQL to analyze real-world U.S. electric vehicle adoption data. The goal is to provide data-driven insights to state transportation agencies and energy utilities. These insights support infrastructure planning, incentive evaluation, and strategic policymaking to accelerate EV adoption and reduce environmental impact.

Key focus areas include:

- **Identifying EV adoption hotspots** for targeted infrastructure deployment  
- **Assessing Clean Alternative Fuel Vehicle (CAFV) incentive effectiveness**  
- **Analyzing EV range and price trends** to understand consumer behavior and reduce range anxiety  

The full ETL pipeline, data cleaning, analysis, and visualizations are implemented using Python notebooks.

---

## Data Structure & Initial Checks

Primary dataset fields include:

- **County, City, State:** Geographic identifiers  
- **Year, Make, Model:** Vehicle manufacturing details  
- **EV_Type:** Battery Electric Vehicle (BEV) or Plug-in Hybrid (PHEV)  
- **CAFV_Eligibility:** Eligibility for clean fuel incentives  
- **EV_Range:** Electric range in miles  
- **MSRP:** Manufacturer suggested retail price  
- **Vehicle_Age:** Calculated vehicle age  
- **Price_Bracket:** Categorized as Budget, Mid-Range, Premium, Luxury  
- **EV_Category:** Classified by EV range (Short, Moderate, Long, Ultra)  

Initial data profiling confirmed data integrity, missing value handling, and removal of future model years.

---

## Executive Summary

### Overview of Findings

The analysis reveals clear EV adoption patterns and incentive effectiveness challenges:

- **EV hotspots** are concentrated in cities like Seattle, Everett, and Kent, signaling prime zones for charging infrastructure expansion.  
- **CAFV incentives** largely benefit premium and luxury EV buyers, with budget-friendly models often excluded, suggesting a policy gap.  
- **Battery Electric Vehicles (BEVs)** dominate overall EV registrations, especially in higher price segments.  
- **Improved range capabilities** are evident, with most vehicles falling into moderate to long-range categories, easing consumer range anxiety concerns.  
- Brand-wise, Tesla leads mid-to-high-end segments, while Kia, Chrysler, and Subaru focus on budget-conscious buyers.

---

## Insights Deep Dive

### EV Adoption Hotspots

- Heatmaps and geographic analysis pinpoint high EV densities in urban centers like Seattle, providing a clear map for resource prioritization.

### CAFV Incentive Alignment

- Budget EV models often miss CAFV eligibility, which may hinder adoption in lower-income demographics. Premium EV buyers disproportionately benefit from incentives.

### EV Type and Price Trends

- BEVs dominate, especially among premium and luxury classes; PHEVs mostly occupy mid-range brackets.  
- Price brackets align with EV categories, reflecting consumer segmentation by vehicle range and affordability.

### Vehicle Age and Range Analysis

- Majority of vehicles are between 2 to 8 years old, indicating a growing, relatively new EV market.  
- Long-range EVs are increasingly common, reducing “range anxiety” and fostering consumer confidence.

---

## Recommendations

Based on the insights, the following strategic actions are advised:

- **Expand charging infrastructure** in identified high-density EV adoption regions such as Seattle and Everett.  
- **Reform CAFV incentives** to include affordable EVs, improving accessibility for budget-conscious consumers.  
- **Encourage manufacturers** targeting budget-friendly long-range EVs through supportive policies and grants.  
- **Leverage state-level adoption patterns** to tailor regional EV growth strategies effectively.

---

## Assumptions and Caveats

- The dataset excludes future vehicle model years to ensure analysis relevance.  
- Geolocation data was generated by city and state combinations, which may introduce minor spatial inaccuracies.  
- Incentive impact is inferred from eligibility data; actual adoption drivers may vary.  
- Data cleaning removed duplicate records and handled missing values to preserve quality.

---

## 📬 Contact

For questions or collaboration opportunities:  

- **Email:** [niranjan991100@gmail.com](mailto:niranjan991100@gmail.com)  
- **LinkedIn:** [https://www.linkedin.com/in/niranjan-k-a83517229/](https://www.linkedin.com/in/niranjan-k-a83517229/)
