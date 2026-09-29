# Train-Schedule-Analysis# 🚆 Train Schedule Analysis and Interactive Route Enquiry System Using Python

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Project](https://img.shields.io/badge/Project-Data%20Analytics-purple)

## 📌 Project Overview

**Train Schedule Analysis and Interactive Route Enquiry System Using Python** is an internship project focused on analyzing train schedule data and developing an interactive route-based train enquiry system.

The project follows an end-to-end data analysis workflow, starting from basic dataset review and data processing and progressing to data quality checks, visualization, advanced analysis, and an interactive train enquiry system.

The final system allows users to enter a **source station** and **destination station** and find available direct trains along with their estimated journey duration.

---

## 🎯 Project Objectives

The main objectives of this project are:

* Understand and review the train schedule dataset
* Identify train routes and station information
* Calculate the number of stops for each train
* Standardize arrival and departure times
* Calculate journey duration
* Classify routes into Short, Medium, and Long
* Generate station-wise train frequency
* Perform data quality checks
* Analyze journey duration and station traffic
* Create visualizations
* Perform pivot table and cross-tabulation analysis
* Develop an interactive train route enquiry system

---

## 📊 Dataset

The dataset contains:

* **186,074 records**
* **12 columns**

### Important Columns

| Column           | Description            |
| ---------------- | ---------------------- |
| `SN`             | Serial number          |
| `Train_No`       | Train number           |
| `Station_Code`   | Station code           |
| `1A`             | First AC information   |
| `2A`             | Second AC information  |
| `3A`             | Third AC information   |
| `SL`             | Sleeper information    |
| `Station_Name`   | Name of station        |
| `Route_Number`   | Station route sequence |
| `Arrival_time`   | Arrival time           |
| `Departure_Time` | Departure time         |
| `Distance`       | Distance information   |

---

# 🛠️ Technologies Used

* **Python**
* **Pandas**
* **Matplotlib**
* **CSV**
* **Jupyter Notebook / VS Code**

---

# 📁 Project Structure

```text
Train_Schedule_Analysis/
│
├── Dataset/
│   └── Dataset1.csv
│
├── Step_1_Basic_Data_Review/
│   └── step1_analysis.py
│
├── Step_2_Data_Processing/
│   ├── step2_processing.py
│   ├── train_summary_step2.csv
│   └── station_frequency_step2.csv
│
├── Step_3_Data_Quality/
│   ├── step3_quality.py
│   └── verified_train_dataset.csv
│
├── Step_4_Analysis_Visualization/
│   ├── step4_analysis.py
│   ├── average_duration.png
│   └── top_10_stations.png
│
├── Step_5_Advanced_Analysis/
│   ├── step5_advanced.py
│   ├── station_train_distribution.csv
│   ├── station_route_crosstab.csv
│   ├── top_10_station_distribution.png
│   └── station_route_comparison.png
│
├── Step_6_Interactive_Train_Enquiry/
│   └── train_enquiry.py
│
├── PPT/
│   └── Train_Schedule_Analysis_Presentation.pptx
│
├── Screenshots/
│   └── project screenshots
│
└── README.md
```

---

# 🔄 Project Workflow

```text
Raw Train Dataset
       ↓
Level 1 — Basic Data Review
       ↓
Level 2 — Simple Data Processing
       ↓
Level 3 — Data Quality Checks
       ↓
Level 4 — Analysis & Visualization
       ↓
Level 5 — Advanced Analysis
       ↓
Level 6 — Interactive Train Enquiry
       ↓
Final Project Output
```

---

# 1️⃣ Level 1 — Basic Data Review

The first level focuses on understanding the dataset.

### Tasks Completed

* Reviewed dataset structure
* Checked total records and attributes
* Listed trains with starting and ending stations
* Calculated the number of stops for each train
* Identified trains with maximum and minimum stops

### Key Analysis

```text
Train
  ↓
Stations
  ↓
Route Order
  ↓
Number of Stops
```

---

# 2️⃣ Level 2 — Simple Data Processing

The second level focuses on processing train schedule information.

### Tasks Completed

### ⏰ Time Standardization

Arrival and departure times were converted into a usable time format.

### 🚆 Journey Duration

Journey duration was calculated using:

```text
Last Arrival − First Departure
```

For overnight journeys, the next-day assumption was handled by adding 24 hours when required.

### 🛣️ Route Classification

Routes were classified using:

```text
< 6 Hours       → Short
6–12 Hours      → Medium
> 12 Hours      → Long
```

### 🚉 Station Frequency

Station-wise train frequency was calculated to identify stations with higher train activity.

---

# 3️⃣ Level 3 — Data Quality Checks

Before performing further analysis, data quality checks were performed.

### Checks Included

* Missing arrival/departure schedule values
* Duplicate records
* Correct station route order

After cleaning and verification, the processed dataset was saved as:

```text
verified_train_dataset.csv
```

---

# 4️⃣ Level 4 — Basic Analysis & Visualization

The fourth level focuses on exploratory analysis and visualization.

### Analysis Performed

* Average journey duration by route type
* High-traffic stations
* Station-wise train frequency
* Journey duration comparison

### Visualizations

#### Average Journey Duration

A bar chart was created to compare average journey duration across route categories.

#### Top High-Traffic Stations

A horizontal bar chart was created to identify stations with higher train frequency.

---

# 5️⃣ Level 5 — Advanced Analysis & Visualization

Advanced analysis was performed using pivot tables and cross-tabulations.

### Pivot Table

A station-wise pivot table was created to analyze the number of unique trains associated with each station.

### Cross-Tabulation

A station × route cross-tabulation was created to understand train distribution across routes.

```text
Station
   ×
Route Number
   ↓
Train Distribution
```

### Visualizations

* Top 10 station train distribution
* Station vs route comparison
* Stacked comparative chart

### Advanced Insights

The analysis identifies:

* Stations with high train distribution
* Station-route combinations with higher frequency
* Total unique stations
* Total route numbers

---

# 6️⃣ Level 6 — Interactive Train Enquiry System 🚆

The final stage of the project is an interactive route-based train enquiry system.

### How It Works

The user enters:

```text
Source Station
Destination Station
```

The Python program then:

```text
User Input
    ↓
Search Dataset
    ↓
Find Source Station
    ↓
Find Destination Station
    ↓
Check Route Order
    ↓
Find Direct Trains
    ↓
Calculate Journey Duration
    ↓
Display Results
```

### Example Input

```text
Enter Source Station: New Delhi
Enter Destination Station: Bhopal
```

### Output

```text
AVAILABLE DIRECT TRAINS

Train_No
Source
Destination
Departure_Time
Arrival_Time
Journey_Duration_Hours
```

The system also handles the case where no direct train is found.

```text
❌ No direct trains found.
```

---

# ▶️ How to Run the Project

## Step 1 — Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

## Step 2 — Open the Project

```bash
cd Train_Schedule_Analysis
```

## Step 3 — Install Required Libraries

```bash
pip install pandas matplotlib
```

## Step 4 — Run the Analysis

Run the Python files from their respective folders.

For example:

```bash
cd Step_6_Interactive_Train_Enquiry
python train_enquiry.py
```

## Step 5 — Enter Route

```text
Enter Source Station:
Enter Destination Station:
```

The system will display matching direct trains.

---

# 📈 Project Outputs

The project generates:

* Train-wise route information
* Number of stops per train
* Journey duration
* Route classification
* Station frequency
* Verified dataset
* Average journey duration chart
* High-traffic station chart
* Station train distribution
* Station-route cross-tabulation
* Advanced comparison charts
* Interactive train enquiry results

---

# 💡 Key Learnings

Through this project, I developed practical experience in:

* Data loading and exploration
* Data cleaning
* Data validation
* Data transformation
* GroupBy operations
* Pivot tables
* Cross-tabulation
* Exploratory Data Analysis
* Data visualization
* Python functions
* User input handling
* Route-based data searching
* Basic application development

---

# 🚀 Future Scope

The project can be further improved by adding:

* GUI-based train enquiry system
* Web-based application
* Database integration
* Date-wise train availability
* Advanced route search
* Multi-stop route planning
* Train filtering by departure time
* Distance-based analysis
* Interactive dashboards

---

# 📸 Project Screenshots

Add your project screenshots inside the `Screenshots` folder and display them here.

Example:

```markdown
![Journey Duration Analysis](Screenshots/average_duration.png)
```

```markdown
![Top Stations](Screenshots/top_10_stations.png)
```

```markdown
![Interactive Train Enquiry](Screenshots/train_enquiry_output.png)
```

---

# 🎓 Internship Project

**Project:** Train Schedule Analysis and Interactive Route Enquiry System Using Python

**Role:** Data Analyst Intern / Data Analytics Learner

**Tools:** Python, Pandas, Matplotlib

**Project Type:** Data Analysis + Interactive Application

---

# 👨‍💻 Author

**Vikash Rao**

Aspiring Data Analyst

Skills:

```text
Python | SQL | Excel | Power BI | Data Analysis
```

---

## ⭐ Conclusion

This project demonstrates an end-to-end Python-based data analysis workflow, starting from raw train schedule data and progressing through data processing, quality checks, visualization, advanced analysis, and an interactive train route enquiry system.

The project combines **data analysis and basic application development** to transform train schedule data into useful analytical and enquiry-based outputs.
