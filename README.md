<center>
    
# Charging Stations for Electric Vehicles in The U.S. and Territories<br> 

</center>

An interactive Power BI analysis of EV charging infrastructure across the United States and U.S. territories, with a focus on Nissan EV charging compatibility.

## Overview

This project analyzes electric vehicle (EV) charging infrastructure across the United States and U.S. territories, with a focus on Nissan EV charging compatibility.

Using a dataset containing 80,000+ charging station records and 70+ attributes, I cleaned, transformed, and analyzed the data in Power BI to develop an interactive report examining the availability and distribution of EV charging infrastructure.

The final report covers 86,000+ charging stations across 54 U.S. states and territories, including an analysis of stations compatible with different Nissan EV categories.

<img width="871" height="486" alt="dashboard-overview" src="https://github.com/user-attachments/assets/90fe6924-c65e-4632-9e71-06139a943478" />

## Project Objectives

- Analyze the distribution of EV charging stations across the U.S. and territories.
- Identify the number and percentage of charging stations compatible with Nissan EVs.
- Examine charging compatibility across different Nissan vehicle categories.
- Present large-scale infrastructure data through interactive visualizations and KPIs.
- Create a dashboard that makes EV charging infrastructure trends easier to explore and understand.

## Dashboard

The Power BI report provides an overview of U.S. EV charging infrastructure and Nissan compatibility.

### Key Metrics

| Metric | Value |
|---|---:|
| Total EV Charging Stations | **86,805+** |
| Nissan-Compatible Stations | **21,211+** |
| States & Territories | **54** |
| Dataset Size | **80,000+ rows** |
| Dataset Attributes | **70+ columns** |

## Nissan Compatibility

The report categorizes charging stations based on Nissan compatibility, including:

| Nissan EV Category | Description |
|---|---|
| **Standard Level 2** | Charging stations supporting standard Level 2 charging. |
| **Nissan Next-Gen (2026+)** | Charging stations categorized as compatible with next-generation Nissan EVs. |
| **Nissan Current (Ariya)** | Charging stations categorized as compatible with the Nissan Ariya. |
| **Nissan Legacy (Leaf)** | Charging stations categorized as compatible with the Nissan Leaf. |
| **Other** | Charging stations that do not fall into the primary Nissan compatibility categories. |

<img width="867" height="488" alt="nissan-compatibility" src="https://github.com/user-attachments/assets/8347a5e5-5a7a-4904-a959-5772d8a0025f" />


The dashboard allows these categories to be compared to understand the availability of charging infrastructure for different Nissan EVs.

## Data Analysis

The project involved working with a large, multi-attribute dataset containing information about EV charging stations across the United States and territories.

**Key areas of analysis included:**

- Charging station availability
- Geographic distribution
- State and territory coverage
- Nissan charging compatibility
- Compatibility by Nissan EV category
- Overall infrastructure coverage

**DAX & Data Modeling**

DAX measures and calculations were used to create summary metrics and support dashboard analysis.

Key calculations included metrics for:

- Total EV Charging Stations
- Total Nissan-Compatible Stations
- Nissan Compatibility by Vehicle Category
- Percentage of Stations by Compatibility Type
- State and Territory Coverage
- Category-Level Station Counts

These calculations were used to power KPI cards, charts, and interactive report visuals.

Example DAX Measures

Total Stations =\
COUNT('US_EV_Charging_Stations'[Station Name])\
Nissan Compatible Stations =\
CALCULATE(\
&emsp;COUNT('US_EV_Charging_Stations'[Station Name]),\
&emsp;'US_EV_Charging_Stations'[Nissan Compatibility] <> "Other"\
)\
Nissan Compatibility % =\
DIVIDE(\
&emsp;[Nissan Compatible Stations],\
&emsp;[Total Stations],\
&emsp;0\
)

**Tools & Technologies**

- Power BI Desktop
- Power Query
- DAX
- Data Cleaning & Transformation
- Data Modeling
- Data Visualization

**Skills Demonstrated**

- Working with large datasets
- Data cleaning and transformation
- Data modeling
- DAX calculations
- Interactive dashboard development
- Geographic data analysis
- KPI development
- Data visualization
- Translating raw data into actionable insights

## Project Structure
EV-Nissan-Infrastructure/\
│\
├── README.md\
├── EV-Nissan-Infrastructure.pbix\
└── images/\
&emsp;├── dashboard-overview.png\
&emsp;└── nissan-compatibility.png
    
## Conclusion

This project demonstrates the use of Power BI to transform a large EV charging infrastructure dataset into an interactive analytical report. The analysis combines infrastructure coverage with Nissan-specific charging compatibility to provide a clearer view of EV charging availability across the U.S. and its territories.
