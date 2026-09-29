# 🚦 Urban Road Safety & Near-Miss Analysis

A data analysis project that investigates **road safety risks, near-miss situations, and traffic conditions** across different cities and road environments.

The goal of this project is to use **Python, Pandas, NumPy, and Matplotlib** to discover patterns between traffic, weather, vehicle type, road type, speed, pedestrian activity, visibility, and road incidents.

---

## 📌 Project Overview

Road safety can be affected by many factors, including:

- 🚗 Vehicle speed
- 🚦 Traffic level
- 🌧️ Weather conditions
- 🌫️ Visibility
- 🚶 Pedestrian activity
- 🛣️ Road type
- 🏍️ Vehicle type
- 🕐 Time of day

This project analyzes **12,000 road-safety observations** and attempts to identify combinations of conditions associated with higher `Near_Miss_Score` values and reported incidents.

---

## 🎯 Project Objectives

The main objectives are to:

1. Understand the structure of the dataset.
2. Clean and validate the data.
3. Analyze road incidents across different cities.
4. Investigate incidents by time of day.
5. Analyze the effect of weather conditions.
6. Study the relationship between traffic and road safety.
7. Compare different vehicle types.
8. Analyze different road types.
9. Investigate speed and near-miss scores.
10. Study pedestrian activity and visibility.
11. Find high-risk combinations of conditions.
12. Create meaningful visualizations.

---

## 📊 Dataset

The dataset contains **12,000 observations** and **14 columns**.

| Column               | Description                               |
| -------------------- | ----------------------------------------- |
| `Record_ID`          | Unique observation ID                     |
| `City`               | City where the observation occurred       |
| `Day_of_Week`        | Day of the week                           |
| `Hour`               | Hour of the observation                   |
| `Weather`            | Weather condition                         |
| `Traffic_Level`      | Traffic intensity                         |
| `Vehicle_Type`       | Type of vehicle                           |
| `Road_Type`          | Type of road                              |
| `Speed_Limit_kmh`    | Speed limit of the road                   |
| `Average_Speed_kmh`  | Average vehicle speed                     |
| `Pedestrian_Count`   | Number of pedestrians                     |
| `Visibility_Percent` | Visibility percentage                     |
| `Near_Miss_Score`    | Road safety risk score                    |
| `Incident`           | Whether an incident occurred (`0` or `1`) |

### Dataset Size

```text
Rows:       12,000
Columns:    14
```

---

## 🛠️ Technologies Used

### Python

The project is implemented in Python.

### Pandas

Used for:

- Data loading
- Data cleaning
- Grouping
- Aggregation
- Statistical analysis
- Data manipulation

### NumPy

Used for:

- Numerical calculations
- Statistical operations
- Working with numerical data

### Matplotlib

Used for:

- Bar charts
- Line plots
- Histograms
- Scatter plots
- Data visualization

---

## 📚 Project Modules

The project is divided into small modules.

### Module 1 — Data Loading

- Load the CSV dataset.
- Display the first and last rows.
- Check dataset dimensions.
- Check column names.

### Module 2 — Data Understanding

- Identify numerical columns.
- Identify categorical columns.
- Calculate average speed.
- Calculate average near-miss score.
- Find maximum pedestrian count.
- Find minimum visibility.
- Generate statistical summaries.

### Module 3 — Data Cleaning

- Check missing values.
- Check duplicate rows.
- Check data types.
- Check invalid values.
- Validate numerical ranges.

### Module 4 — Basic Statistical Analysis

Analyze:

- Mean
- Median
- Minimum
- Maximum
- Standard deviation
- Incident percentage

### Module 5 — City Analysis

Investigate:

- Number of observations per city
- Incident count by city
- Average near-miss score by city
- Incident rate by city

### Module 6 — Time Analysis

Analyze:

- Incidents by hour
- Near-miss score by hour
- Incidents by day of the week
- Daytime vs nighttime patterns

### Module 7 — Weather Analysis

Investigate:

- Incidents by weather
- Average near-miss score by weather
- Visibility by weather
- Weather-related risk patterns

### Module 8 — Traffic Analysis

Analyze:

- Traffic distribution
- Incidents by traffic level
- Average near-miss score by traffic level

### Module 9 — Vehicle Analysis

Investigate:

- Vehicle distribution
- Incidents by vehicle type
- Average near-miss score by vehicle type
- Incident rate by vehicle type

### Module 10 — Road Analysis

Analyze:

- Road type distribution
- Incidents by road type
- Average near-miss score by road type
- Pedestrian activity by road type

### Module 11 — Speed Analysis

Create a new feature:

```python
Speed_Difference = Average_Speed_kmh - Speed_Limit_kmh
```

Investigate:

- Vehicles exceeding the speed limit
- Average near-miss score for speeding observations
- Speed vs near-miss score
- Speed-related incident patterns

### Module 12 — Pedestrian Analysis

Analyze:

- Average pedestrian count
- Pedestrian count by road type
- Pedestrian count vs near-miss score
- Pedestrian activity and incidents

### Module 13 — Risk Analysis

Find:

- Highest near-miss scores
- Top 10 highest-risk observations
- Common conditions among high-risk observations

### Module 14 — Dangerous Combinations

This is one of the main parts of the project.

Analyze combinations such as:

```text
City + Weather
Road_Type + Weather
Traffic_Level + Weather
Road_Type + Traffic_Level
Vehicle_Type + Weather
```

Example:

```python
df.groupby(
    ["Road_Type", "Weather"]
)["Near_Miss_Score"].mean()
```

The objective is to identify combinations associated with higher average near-miss scores.

### Module 15 — Visualization

Create visualizations such as:

- Incidents by city
- Incidents by weather
- Incidents by traffic level
- Incidents by vehicle type
- Incidents by road type
- Incidents by hour
- Speed vs near-miss score
- Pedestrian count vs near-miss score

### Module 16 — Final Analysis

Summarize the major patterns discovered during the analysis.

---

## 📈 Example Questions

Some of the questions investigated in this project include:

- Which city has the highest number of incidents?
- Which city has the highest average near-miss score?
- Which hour has the most incidents?
- Which weather condition has the highest average risk?
- Does traffic level appear related to near-miss scores?
- Which vehicle type has the most incidents?
- Which road type has the highest average near-miss score?
- Does exceeding the speed limit correspond to higher near-miss scores?
- Does pedestrian activity relate to road safety?
- Which `Road_Type + Weather` combination has the highest average near-miss score?
- Which `Traffic_Level + Weather` combination has the highest average near-miss score?

---

## 📊 Visualizations

The project uses Matplotlib to create different types of charts.

### Bar Charts

Used for categorical comparisons such as:

```text
City → Incident Count
Weather → Incident Count
Vehicle Type → Incident Count
Road Type → Incident Count
```

### Line Plots

Used for time-based analysis:

```text
Hour → Incident Count
Hour → Average Near-Miss Score
```

### Scatter Plots

Used to investigate relationships:

```text
Average Speed → Near-Miss Score
Pedestrian Count → Near-Miss Score
```

### Histograms

Used to understand distributions such as:

```text
Near-Miss Score distribution
Average Speed distribution
```

---

## 🧠 Skills Practiced

This project helps practice:

- Python
- NumPy
- Pandas
- Matplotlib
- Data cleaning
- Data exploration
- GroupBy
- Aggregation
- Statistical analysis
- Feature creation
- Data visualization
- Exploratory Data Analysis (EDA)
- Interpreting data patterns

---

## 📁 Project Structure

```text
Urban-Road-Safety-Near-Miss-Analysis/
│
├── data/
│   └── urban_near_miss_dataset_12000.csv
│
├── notebooks/
│   ├── 01_data_loading.ipynb
│   ├── 02_data_understanding.ipynb
│   ├── 03_data_cleaning.ipynb
│   ├── 04_basic_analysis.ipynb
│   ├── 05_city_analysis.ipynb
│   ├── 06_time_analysis.ipynb
│   ├── 07_weather_analysis.ipynb
│   ├── 08_traffic_analysis.ipynb
│   ├── 09_vehicle_analysis.ipynb
│   ├── 10_road_analysis.ipynb
│   ├── 11_speed_analysis.ipynb
│   ├── 12_pedestrian_analysis.ipynb
│   ├── 13_risk_analysis.ipynb
│   ├── 14_dangerous_combinations.ipynb
│   └── 15_final_visualization.ipynb
│
├── README.md
└── requirements.txt
```

---

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/Engr-Jawad/Data-Science-Projects
```

### 2. Open the project

```bash
cd Urban-Road-Safety-Near-Miss-Analysis
```

### 3. Install the required libraries

```bash
pip install pandas numpy matplotlib jupyter
```

### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

Open the notebooks in the `notebooks` folder and work through the modules in order.

---

## ⚠️ Important Note

This dataset is intended for **educational and data-analysis practice**. The observations are synthetic and should not be interpreted as real-world traffic or accident statistics.

The analysis identifies patterns within this dataset; it does not establish that a particular factor causes road incidents.

---

## 👨‍💻 Author

**Jawad**

Aspiring Data Scientist

### Skills

```text
Python
Pandas
NumPy
Matplotlib
Data Analysis
Data Visualization
Exploratory Data Analysis
```

---

## ⭐ Project Goal

The main goal of this project is to develop practical data-analysis skills by taking a relatively large dataset and progressing from:

```text
Raw Data
    ↓
Data Understanding
    ↓
Data Cleaning
    ↓
Exploratory Data Analysis
    ↓
Grouping & Aggregation
    ↓
Risk Analysis
    ↓
Visualization
    ↓
Insights
```

This project is designed as a **learning and portfolio project** for developing practical Data Science skills.

