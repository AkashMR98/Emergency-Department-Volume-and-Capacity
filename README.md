# 🏥 Emergency Department Volume & Capacity Analysis

## 📌 Project Overview

Healthcare systems often struggle with managing Emergency Department (ED) demand due to increasing patient volume and limited resources.
This project analyzes patient volume, hospital capacity, and resource utilization to identify inefficiencies and improve decision-making.

--------------------------------------------------------------------------

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

--------------------------------------------------------------------------

## 🎯 Objectives

- Analyze patient volume across hospitals
- Evaluate hospital capacity (beds & ED stations)
- Detect overcrowding and high-demand facilities
- Compare urban vs rural healthcare demand
- Identify shortages in primary care & mental health
- Study trends over time (2021–2023)
- Provide data-driven insights for optimization

--------------------------------------------------------------------------

## 📊 Dataset Information

- Source: https://catalog.data.gov/dataset/emergency-department-volume-and-capacity?from_hint=eyJzb3J0IjoicG9wdWxhcml0eSIsInEiOiIiLCJzcGF0aWFsX2ZpbHRlciI6IiJ9

- Location: United States (hospital-level emergency department data across multiple states)

- Year/Timeline: 2021 - 2023

- Domain: Healthcare Analytics / Hospital Management / Public Health

#### Dataset Size

- Number of Records (Rows): 12,000+

- Number of Attributes (Columns): 18

--------------------------------------------------------------------------

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

--------------------------------------------------------------------------

## 🛠️ Tools & Technologies

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn

--------------------------------------------------------------------------

## ⚙️ Data Preprocessing

- Missing value analysis
- Duplicate checking
- Removal of unnecessary columns
- Feature engineering

--------------------------------------------------------------------------

## 📊 Exploratory Data Analysis

### 📈 Statistical Analysis

#### Measures:

- Mean
- Median
- Mode
- Variance
- Standard Deviation
- Skewness
- Kurtosis

--------------------------------------------------------------------------

### 📉 Data Visualizations

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
### Chart Type:
Scatter Plot

--------------------------------------------------------------------------

### Columns Used:
Total Visits, Visits per Station, Area Type

### Relationship:
Total Visits ↔ Visits per Station (with Area Type classification)

### Insights:
- Urban areas show higher total visits and better station utilization.
- Rural areas fall in the medium range of visits and usage.
- Frontier areas have the lowest visits and utilization levels.
- A slight positive relationship exists between total visits and visits per station.
- This indicates that as hospital visits increase, station usage also increases moderately.

 <img width="580" height="437" alt="scatter totalvisitarea" src="https://github.com/user-attachments/assets/d5244fd5-0aee-46b5-b168-546ee616a7d6" />
 
--------------------------------------------------------------------------

### Chart Type:
Heatmap

### Columns Used:
Total Visits, ED Stations, Condition Visits, Visits per Station

### Relationship:
Correlation between multiple numerical variables

### Insights:
- Total Visits and ED Stations have a strong positive correlation (~0.83).
- Condition Visits and Visits per Station also show strong correlation (~0.80).
- ED Stations and Visits per Station have very low correlation.
- This shows that increasing stations does not always improve efficiency.
- Key hospital metrics are interrelated but not equally impactful.

  <img width="620" height="537" alt="heatmap chart" src="https://github.com/user-attachments/assets/03c92c0d-ad61-4e5a-aa13-896aec7ba23e" />

--------------------------------------------------------------------------

### Chart Type:
Bar Chart

### Columns Used:
Area Type, Total Visits

### Relationship:
Area Type ↔ Total Hospital Visits

### Insights:
- Urban areas record the highest number of hospital visits.
- Rural areas show moderate patient volume.
- Frontier areas have the lowest hospital visits.
- This indicates a clear demand gap based on location.
- Healthcare demand is concentrated more in urban regions.

<img width="588" height="435" alt="barplot chart" src="https://github.com/user-attachments/assets/893630ef-2e03-4507-8873-5fde283cca21" />

--------------------------------------------------------------------------

## 🔍 Key Findings

- Bigger hospitals handle more patients.
- Urban hospitals have higher visits compared to rural & frontier.
- Emergency cases form a major portion of total visits.
- Some hospital systems perform significantly better than others.
- Key variables (beds, visits, emergency) are strongly related.
- Few hospitals handle very high volume, most are moderate/low.
- Certain counties show higher healthcare demand.

--------------------------------------------------------------------------

## 📌 Types of Analysis

- Descriptive Analysis
- Diagnostic Analysis
- Predictive Analysis
- Prescriptive Analysis

--------------------------------------------------------------------------

## 🚀 Future Enhancements

- Forecast future patient visits using ML
- Monitor live hospital data
- Identify high-demand areas using maps
- Group patients by age, disease, region
- Improve bed & staff allocation
- Detect unusual spikes in visits
- Combine multiple hospital data sources

--------------------------------------------------------------------------

## ⭐ Conclusion
This project highlights the gap between patient demand and hospital capacity, identifying overcrowding and resource shortages. The insights help improve resource allocation, efficiency, and patient care through data-driven decisions.



