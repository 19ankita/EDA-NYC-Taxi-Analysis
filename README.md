# 🚕 NYC Taxi Operations Analysis (2023)

A comprehensive Exploratory Data Analysis (EDA) project on NYC Yellow Taxi trip records aimed at optimizing taxi operations through demand forecasting, routing analysis, pricing insights, surcharge behavior analysis, and spatial zone intelligence. The project identifies operational inefficiencies, high-demand zones, traffic bottlenecks, and revenue-driving patterns using temporal, spatial, and fare-related analytics. 

---

## 📌 Project Objectives

* Analyze taxi demand patterns across hours, days, months, and quarters
* Identify high-demand pickup and dropoff zones
* Detect slow and congested routes using average route speeds
* Analyze fare-per-mile patterns across vendors and trip distances
* Study tipping behavior and surcharge application trends
* Optimize taxi fleet positioning and dispatch strategies
* Recommend data-driven pricing and operational improvements

---

## 📂 Dataset

* **Dataset:** NYC Yellow Taxi Trip Records (2023)
* **Source:** NYC Taxi & Limousine Commission (TLC)
* **Format:** Monthly parquet trip files
* **Sampling Strategy:** Hourly-date stratified sampling
* **Final Working Dataset:** ~276,000 rows and 22 columns after 0.7% sampling 

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* GeoPandas
* Streamlit
* Jupyter Notebook

---

## 🧹 Data Cleaning & Preprocessing

Key preprocessing steps included:

* Resetting dataframe index after filtering operations
* Combining airport fee columns into a single feature
* Handling missing values in:

  * `passenger_count`
  * `RatecodeID`
  * `congestion_surcharge`
* Removing invalid payment types
* Fixing negative surcharge values
* Removing unrealistic trip distances and fare anomalies
* Removing passenger counts greater than 6
* Filtering zero/negative fares and trip distances 

---

## 📊 Key Analyses Performed

### ⏰ Temporal Demand Analysis

* Hourly taxi demand trends
* Weekday vs weekend traffic analysis
* Monthly and quarterly revenue trends
* Nighttime vs daytime demand comparison

### 🗺️ Spatial Zone Analysis

* High-demand pickup/dropoff zones
* Pickup/dropoff imbalance ratios
* Nighttime hotspot zones
* Taxi zone heatmaps using GeoPandas

### 🚦 Route Efficiency Analysis

* Average route speed calculations
* Slow-route detection
* Congestion bottleneck identification

### 💰 Fare & Pricing Analysis

* Fare vs distance relationships
* Fare-per-mile comparisons across vendors
* Distance-tier pricing analysis
* Revenue trend analysis

### 💳 Customer Behavior Analysis

* Tip percentage trends
* Payment type distribution
* Passenger count trends
* Surcharge frequency analysis

---

## 📈 Major Insights

### 🚖 Demand Trends

* Highest taxi demand occurs around **11 PM**
* Peak operational hours:

  * 3 PM – 7 PM
  * 11 PM
* Lowest activity observed between **3 AM – 5 AM** 

### 🗺️ High-Demand Zones

Major pickup zones included:

* JFK Airport
* LaGuardia Airport
* Midtown Center
* Times Square/Theatre District
* Upper East Side zones 

### 🚦 Operational Bottlenecks

* Several routes exhibited extremely low average speeds during peak traffic hours
* Congestion heavily affected route efficiency in Manhattan-heavy corridors 

### 💰 Pricing Insights

* Short-distance trips had the highest fare-per-mile values
* Vendor 2 showed more volatile fare patterns during nighttime hours
* Long-distance trips had more stable fare-per-mile behavior 

### 💳 Surcharge Insights

* Surcharges peaked during evening and nighttime hours
* Airports and congested urban zones had the highest surcharge frequencies 

---

## 📌 Recommendations

### 🚕 Fleet & Dispatch Optimization

* Allocate more drivers during peak hours (15:00–19:00 and 23:00)
* Reduce idle fleet allocation during low-demand early-morning hours
* Use route-speed monitoring to avoid congestion-heavy corridors 

### 🗺️ Strategic Cab Positioning

* Prioritize airport and Manhattan zones
* Increase nighttime taxi availability near nightlife and transportation hubs
* Reposition taxis from dropoff-heavy to pickup-heavy zones 

### 💰 Pricing Strategy Improvements

* Carefully review short-trip pricing policies
* Apply dynamic pricing during high-demand periods
* Promote digital payments for better revenue and tip capture 

---




```text
NYC-Taxi-Operations-EDA/
│
├── app.py
├── notebooks/
├── data/
├── images/
├── report/
├── requirements.txt
└── README.md
```

---



`Report_NYC_Taxi_Operations_Ankita_Sarkar.pdf` 
