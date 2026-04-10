# crime-analysis-india
Power BI dashboard analyzing 40,160 crime records across 29 Indian cities (2020–2024) — demographics, victim profiling, police efficiency &amp; geo-spatial insights.

# 🔍 Crime Analysis - India | Power BI Dashboard

A comprehensive **Power BI crime analytics project** built on a dataset of **40,160 crime records** spanning **29 major Indian cities** from **January 2020 to July 2024**. The dashboard provides deep insights into crime demographics, victim profiling, police efficiency, time-based patterns, and geo-spatial crime distribution.

---

## 📁 Repository Structure

```
crime-analysis-india/
│
├── Crime_Analysis_Final.pbix       # Power BI report file
├── data/
│   └── crime_dataset_india.csv     # Raw dataset (40,160 records)
├── screenshots/                    # Dashboard page screenshots
└── README.md
```

---

## 📊 Dataset Overview

**File:** `crime_dataset_india.csv`  
**Records:** 40,160 rows × 17 columns  
**Time Period:** January 2020 – July 2024  

### 🗂️ Columns / Fields

| Column | Type | Description |
|--------|------|-------------|
| `Report Number` | Integer | Unique identifier for each crime report (1–40160) |
| `Date Reported` | String | Date the crime was officially reported |
| `Date of Occurrence` | String | Actual date the crime took place |
| `Time of Occurrence` | String | Time the crime occurred (HH:MM:SS) |
| `City` | String | One of 29 major Indian cities |
| `Crime Code` | Integer | Numeric crime classification code (100–599) |
| `Crime Description` | String | Type of crime (21 categories) |
| `Victim Age` | Integer | Age of the victim (10–79 years) |
| `Victim Gender` | String | M (Male), F (Female), X (Non-binary/Other) |
| `Weapon Used` | String | Weapon involved (5790 nulls = unarmed/unknown) |
| `Crime Domain` | String | Broad domain: Violent Crime, Other Crime, Fire Accident, Traffic Fatality |
| `Police Deployed` | Integer | Number of officers deployed (1–19) |
| `Case Closed` | String | Yes / No |
| `Date and Time of Case Closed` | String | Timestamp of case closure (null if open) |
| `Case Status` | String | Open / Closed |
| `Crime Occurred` | String | Time-of-day: Morning, Afternoon, Evening, Night |
| `Age Group` | String | Child, Teenager, Adult, Senior Citizen |

### 📈 Key Data Statistics

| Metric | Value |
|--------|-------|
| Total Records | 40,160 |
| Cities Covered | 29 |
| Crime Types | 21 |
| Date Range | Jan 2020 – Jul 2024 |
| Open Cases | 20,098 (50%) |
| Closed Cases | 20,062 (50%) |
| Missing: Weapon Used | 5,790 rows |
| Missing: Case Closed Date | 20,098 rows (open cases) |

---

### 🏙️ City-wise Crime Distribution (Top 10)

| City | Records |
|------|---------|
| Delhi | 5,400 |
| Mumbai | 4,415 |
| Bangalore | 3,588 |
| Hyderabad | 2,881 |
| Kolkata | 2,518 |
| Chennai | 2,493 |
| Pune | 2,212 |
| Ahmedabad | 1,817 |
| Jaipur | 1,479 |
| Lucknow | 1,456 |

### 🔫 Weapons Used

| Weapon | Count |
|--------|-------|
| Knife | 5,835 |
| Explosives | 5,751 |
| Blunt Object | 5,737 |
| Poison | 5,728 |
| Other | 5,676 |
| Firearm | 5,643 |
| Unarmed / Unknown | 5,790 |

### 🧑‍🤝‍🧑 Victim Demographics

- **Gender:** Female – 22,423 (55.8%) | Male – 13,405 (33.4%) | Other – 4,332 (10.8%)
- **Age Range:** 10 – 79 years | **Average Age:** ~44.5 years
- **Age Groups:** Adult (17,922) | Senior Citizen (16,544) | Teenager (3,983) | Child (1,711)

### 🕐 Time of Occurrence

| Period | Count |
|--------|-------|
| Evening | 13,365 (33.3%) |
| Morning | 10,061 (25.0%) |
| Night | 10,055 (25.0%) |
| Afternoon | 6,679 (16.6%) |

### 🗂️ Crime Domain Breakdown

| Domain | Count |
|--------|-------|
| Other Crime | 22,948 (57.1%) |
| Violent Crime | 11,472 (28.5%) |
| Fire Accident | 3,825 (9.5%) |
| Traffic Fatality | 1,915 (4.8%) |

---

## 📋 Power BI Report Pages

The `.pbix` file contains **9 report pages**, built using Power BI Desktop (Version 2.142.580.0) and published from the Cloud in April 2025.

---

### 1. 🏠 INTRO
Landing/navigation page.
- Project title: **"Crime Analysis – India"**
- Navigation buttons to: Dataset, Dashboard, Data Preparation pages
- Decorative shapes and layout elements

<img width="995" height="563" alt="image" src="https://github.com/user-attachments/assets/010462cd-3ada-4875-8555-b5b5c0b0963f" />


---

### 2. 📋 Dataset
A documentation page describing the raw data source.
- Static textbox descriptions of the dataset
- Navigation panel for moving between report pages

<img width="997" height="562" alt="image" src="https://github.com/user-attachments/assets/6aaa909f-b647-4869-b30a-f1500f9bcd9b" />

---

### 3. 👥 Crime Demographics
**Interactive slicers:** Year, Month, City, Crime Domain, Gender, Crime Occurred

| Visual | Type | Description |
|--------|------|-------------|
| Total Crimes | Card | KPI – total number of crimes |
| Quarterly Crimes Occurred | Line Chart | Crime trend across quarters |
| Types of Weapons Used | Donut Chart | Weapon distribution |
| Count of Case by Crime | Treemap | Crime-type frequency map |
| Case Status | Column Chart | Open vs. Closed breakdown |
| Age Grp-wise Crimes | Donut Chart | Child / Teen / Adult / Senior breakdown |
| 2 KPI Cards | Cards | Additional metrics |

<img width="997" height="566" alt="image" src="https://github.com/user-attachments/assets/98b4c3d3-eabd-45b6-9af5-8f1c5ccc374a" />


---

### 4. 🩺 Victim Analysis
**Interactive slicers:** Crime Domain, Crime Occurred, Month, Gender, Year, City

| Visual | Type | Description |
|--------|------|-------------|
| Age Grp-wise Victims | Donut Chart | Victim age group distribution |
| Gender-wise Victims | Pie Chart | M / F / X gender split |
| Top Victim Age Segments | Clustered Bar Chart | Most affected age ranges |
| Total Crime by City | Pivot Table | Matrix of crime counts per city |


<img width="995" height="561" alt="image" src="https://github.com/user-attachments/assets/c9c25a89-38be-482f-a1c2-02e566f26d99" />

---

### 5. 👮 Police Efficiency
**Interactive slicers:** Crime Domain, Crime Occurred, Month, Gender, Year, City

| Visual | Type | Description |
|--------|------|-------------|
| Police Deployed by City (Top 10) | Clustered Bar Chart | Resource allocation by city |
| Police Deployed per Cases | Clustered Column Chart | Efficiency ratio |
| Case Status vs Police Deployed | Column Chart | Correlation between deployment and resolution |
| Monthly Police Deployed vs Total Reports | Stacked Area Chart | Trend over time |
| Pivot Table | Matrix | Detailed cross-tab breakdown |

<img width="998" height="558" alt="image" src="https://github.com/user-attachments/assets/e7b14ac7-0735-4766-a4d1-1b97eb3e4fc8" />


---

### 6. ⏰ Time Analysis – 1 (Occurrence-based)
**Interactive slicers:** Crime Domain, Crime Occurred, Month, Gender, Year, City

| Visual | Type | Description |
|--------|------|-------------|
| Crimes Occurred by Day of the Week | Clustered Column Chart | Weekly pattern of incidents |
| Hourly Crimes | Clustered Column Chart | Hour-by-hour crime distribution |
| Monthly Crimes | Area Chart | Monthly crime volume trend |
| Age Grp-Wise Crimes Per Day | Bar Chart | How different age groups are affected per weekday |

<img width="997" height="562" alt="image" src="https://github.com/user-attachments/assets/6acc5133-651b-4cd6-baaa-241be8377781" />


---

### 7. ⏱️ Time Analysis – 2 (Reporting-based)
**Interactive slicers:** Crime Domain, Crime Occurred, Month, Gender, Year, City

| Visual | Type | Description |
|--------|------|-------------|
| Hourly Police Deployed | Clustered Column Chart | When are police most active |
| Monthly Crimes Reported | Area Chart | Reporting trend over months |
| Age Grp-Wise Crimes Reported Per Day | Column Chart | Age-segmented reporting patterns |
| Avg Crimes Reported by Day | Clustered Bar Chart | Average daily reporting volume |

<img width="995" height="560" alt="image" src="https://github.com/user-attachments/assets/32c1df50-0c19-47a1-8771-2f2947dceb73" />


---

### 8. 🗺️ Geo Crime Analysis
**Interactive slicers:** Crime Domain, Crime Occurred, Month, Gender, Year, City, + a map-specific slicer

| Visual | Type | Description |
|--------|------|-------------|
| Count of Crime by City | Shape Map | India map with choropleth crime density |
| Top 10 Cities With Most Crime | Bar Chart | City ranking by crime volume |
| Pivot Table | Matrix | City × Crime type detail |

*Note: Uses a custom India TopoJSON file (`india8201911891396916.json`) for the shape map.*

<img width="995" height="557" alt="image" src="https://github.com/user-attachments/assets/171bf4c8-d4a9-4b12-83eb-41ff944e32be" />


---

### 9. 💡 INSIGHTS
Key findings and conclusions page.
- Textbox with written insights summarizing the analysis
- Navigation panel

<img width="995" height="561" alt="image" src="https://github.com/user-attachments/assets/53428862-fd26-4170-b2b0-0fbe7447e05e" />


---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** v2.142.580.0 | Report building & visualization |
| **Power Query** | Data cleaning and transformation |
| **DAX** | Calculated measures and KPIs |
| **Python / Pandas** | Exploratory data analysis |
| **TopoJSON (India map)** | Geo-spatial shape map |

---

## 🚀 How to Use

### Prerequisites
- [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) (free) installed on Windows

### Steps
1. **Clone this repository:**
   ```bash
   git clone https://github.com/YOUR_USERNAME/crime-analysis-india.git
   cd crime-analysis-india
   ```

2. **Open the report:**
   - Launch **Power BI Desktop**
   - Go to `File → Open report → Browse`
   - Select `Crime_Analysis_Final.pbix`

3. **Refresh data (if needed):**
   - Go to `Home → Transform data → Data source settings`
   - Update the file path to point to `data/crime_dataset_india.csv` on your machine
   - Click `Close & Apply`

4. **Explore the dashboard** using the navigation panel on each page.

---

## 📌 Key Insights

- 🏙️ **Delhi, Mumbai, and Bangalore** account for the highest crime volumes
- 🌆 **Evening hours** are the most crime-prone time period (33% of all crimes)
- 👩 **Female victims** are the majority (55.8%) in recorded crimes
- 👴 **Adults and Senior Citizens** are the most affected age groups (combined ~85%)
- ⚖️ **Case closure rate** is approximately 50%, indicating room for improvement in resolution
- 🔪 **Knives** are the most commonly used weapon type
- 🚨 **Burglary** is the most frequent crime type (~1,980 cases)

---

## 📄 License

This project is for educational and analytical purposes only. The dataset is synthetic/simulated for learning purposes.

---

## 🙋‍♂️ Author

**[Aleena Hanjgikar]**  
📧 [aleenahanjgikar@gmail.com]  
🔗 [LinkedIn]( www.linkedin.com/in/aleena-hanjgikar-89a723251)

---

> ⭐ If you found this project helpful, please give it a star!
