# EV Vehicle Population Analysis — Advanced Tableau Project Documentation

## Project Overview
This comprehensive Tableau workbook provides an in-depth analysis of the Electric Vehicle (EV) population dataset, emphasizing statistical patterns in vehicle distribution, manufacturer dynamics, and eligibility classifications. The methodology integrates rigorous data preprocessing, systematic validation of dataset integrity, and the derivation of advanced key performance indicators (KPIs), culminating in a series of sophisticated visual analytics.

---

## Methodological Framework

### 1. Data Preprocessing and Quality Assurance
- **Initial Dataset Assessment:**  
A meticulous examination identified missing values in critical fields such as `County`, `City`, `Postal Code`, `Legislative District`, `Vehicle Location`, `Electric Utility`, and `2020 Census Tract`.

- **Data Remediation Process:**  
All records containing null or incomplete entries in these fields were systematically excised to preserve analytical validity.  
- **Quantitative Summary:**  
  - Initial observations: **150,483 records**  
  - Post-cleaning dataset: **150,138 records**  

- **Geographical Clarification:**  
Initial assumptions positing nationwide data coverage were refuted; the dataset exclusively represents vehicle registrations within **Washington State (WA)**.  

- **Outlier Identification and Management:**  
Data from the year 2024 were incomplete and subsequently excluded to eliminate distortions in trend analyses.  
- **Finalized Dataset:**  
  - Curated and verified dataset: **149,496 observations**

---

### 2. Analytical Design and Visualization Architecture

#### a. KPI Derivation and Advanced Metric Construction:
- **Total EV Count:** Computed via custom-calculated fields with validation checks.  
- **Average Electric Range:** Derived through aggregation techniques to ensure representative sampling.  
- **Temporal Scope:** Analytical focus constrained to data from 2010 onwards due to insufficient representation in prior years.

#### b. Data Visualization Suite:
- **Proportionate Analysis of BEV and PHEV Vehicles:** Inclusive of both absolute totals and relative percentages using dynamic calculated fields.  

![BEV vs PHEV Distribution](./screenshots/bev_phev_distribution.png)

- **Visual Constructs Developed:**  
  - **Longitudinal trend of vehicle registrations by model year**  
    ![Registration Trends](./screenshots/registration_trends.png)
    
  - **Geospatial distribution by county**  
    ![County Distribution Map](./screenshots/geospatial_distribution.png)
    
  - **Parametric analysis of top vehicle manufacturers based on registration volume**  
    ![Top Manufacturers](./screenshots/top_manufacturers.png)
    
  - **Predictive modeling of EV adoption trends using Tableau's exponential smoothing forecast**  
    ![Forecast Model](./screenshots/forecast_model.png)

  - **Analysis of vehicles by CAFV eligibility**  
    ![CAFV Eligibility](./screenshots/Total%20Vehicles%20by%20CAFV%20Eligibility.PNG)
    
  - **Top vehicle models by registration count**  
    ![Top Vehicle Models](./screenshots/Top%20Vehicle%20Models.PNG)

- **Parametric Controls:**  
  An interactive **Top N Parameter** was integrated for stakeholder-driven analysis of manufacturers and models.  
---

## Principal Findings and Scholarly Insights:
- The dataset definitively represents EV registrations within **Washington State**, enabling focused regional policy analysis.  
- **Urban-centric clustering** of EV adoption is evident, reflecting infrastructure availability and demographic patterns.  
- **Market dynamics** reveal a concentration of vehicle registrations among select manufacturers and models, informing strategic market entry considerations.

---

## Artifacts and Deliverables:
- **EV_Vehicle_Population.twbx** — The primary Tableau workbook encapsulating the complete analytical process.

---

## Authorship and Correspondence
Authored by Sahil Thorat, MS in Data Science, Data Science and Analytics.  
For inquiries, please contact via [LinkedIn](https://www.linkedin.com/in/sahilthorat/).