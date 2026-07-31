# 🏥 Emergency Department Volume & Capacity Analysis

## 📌 Project Overview

Healthcare systems often struggle with managing Emergency Department (ED) demand due to increasing patient volume and limited resources.
This project analyzes patient volume, hospital capacity, and resource utilization to identify inefficiencies and improve decision-making.

## 🚨 Business Problem

Hospitals need to answer critical operational questions:

- Are emergency departments overloaded?
- Do hospitals have enough beds and treatment stations?
- Which regions face higher patient demand?
- Are there shortages in primary care or mental health services?
- How can resources be optimized to reduce waiting time?

Without proper analysis, this leads to:

- Overcrowding
- Delayed treatments
- Poor resource allocation

## 🎯 Objectives

- Analyze patient volume across hospitals
- Evaluate hospital capacity (beds & ED stations)
- Detect overcrowding and high-demand facilities
- Compare urban vs rural healthcare demand
- Identify shortages in primary care & mental health
- Study trends over time (2021–2023)
- Provide data-driven insights for optimization

## 📊 Dataset Information

- Source: https://catalog.data.gov/dataset/emergency-department-volume-and-capacity?from_hint=eyJzb3J0IjoicG9wdWxhcml0eSIsInEiOiIiLCJzcGF0aWFsX2ZpbHRlciI6IiJ9

- Location: United States (hospital-level emergency department data across multiple states)

- Year/Timeline: 2021 - 2023

- Domain: Healthcare Analytics / Hospital Management / Public Health

#### Dataset Size

- Number of Records (Rows): 12,000+

- Number of Attributes (Columns): 18

## 🧾 Data Dictionary (Renamed Attributes)

| Original Attribute       | Renamed Column     | Description                                          |
| ------------------------ | ------------------ | ---------------------------------------------------- |
| oshpd_id                 | hospital_id        | Unique ID for each hospital facility                 |
| FacilityName2            | hospital_name      | Name of the hospital                                 |
| CountyName               | county             | County where the hospital is located                 |
| system                   | hospital_system    | Hospital network/system affiliation                  |
| LICENSED_BED_SIZE        | bed_size           | Category of licensed bed capacity                    |
| HospitalOwnership        | ownership          | Type of hospital ownership                           |
| UrbanRuralDesi           | area_type          | Indicates whether hospital is in urban or rural area |
| TEACHINGDesignation      | teaching_status    | Teaching or non-teaching hospital                    |
| Category                 | condition          | Health condition category                            |
| Tot_ED_NmbVsts           | total_visits       | Total number of emergency visits                     |
| EDStations               | ed_stations        | Number of emergency department stations              |
| EDDXCount                | condition_visits   | Number of visits for specific condition              |
| LATITUDE                 | latitude           | Latitude of hospital location                        |
| LONGITUDE                | longitude          | Longitude of hospital location                       |
| PrimaryCareShortageArea  | primary_care_area  | Indicates if area has primary care shortage          |
| MentalHealthShortageArea | mental_health_area | Indicates if area has mental health shortage         |
| Visits_Per_Station       | visits_per_station | Average visits handled per station                   |
| Year                     | year               | Year of the data                                     |

Note: Column names were renamed for better readability and analysis.

## 🛠️ Tools & Technologies

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn

## ⚙️ Data Preprocessing

- Missing value analysis
- Duplicate checking
- Removal of unnecessary columns
- Feature engineering

## 📈 Statistical Analysis

#### Measures:

- Mean
- Median
- Mode
- Variance
- Standard Deviation
- Skewness
- Kurtosis

## 📉 Data Visualizations

### Univariate Analysis

- Hospital Bed Size Distribution
- Outlier Detection in Patient Visits
- Outlier Detection in Patient Visits

### Bivariate Analysis

- Total Visits vs Condition Visits
- Bed Size vs Total Visits
- Area Type vs Total Visits

### Multivariate Analysis

- Correlation Heatmap
- Scatter (with hue)

## 🔍 Key Findings

- Bigger hospitals handle more patients.
- Urban hospitals have higher visits compared to rural & frontier.
- Emergency cases form a major portion of total visits.
- Some hospital systems perform significantly better than others.
- Key variables (beds, visits, emergency) are strongly related.
- Few hospitals handle very high volume, most are moderate/low.
- Certain counties show higher healthcare demand.

## 📌 Types of Analysis

- Descriptive Analysis
- Diagnostic Analysis
- Predictive Analysis
- Prescriptive Analysis

## 🚀 Future Enhancements

- Forecast future patient visits using ML
- Monitor live hospital data
- Identify high-demand areas using maps
- Group patients by age, disease, region
- Improve bed & staff allocation
- Detect unusual spikes in visits
- Combine multiple hospital data sources

## ⭐ Conclusion
This project highlights the gap between patient demand and hospital capacity, identifying overcrowding and resource shortages. The insights help improve resource allocation, efficiency, and patient care through data-driven decisions.



