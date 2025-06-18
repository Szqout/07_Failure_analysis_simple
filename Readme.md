# Failure Data Analysis for Aircraft Hydraulic Pump

## ✈️ Project Overview

This mini-project demonstrates how to analyze failure data for a actuator in an modern factory. Using Python and basic statistical tools, the project calculates reliability metrics like **Mean Time Between Failures (MTBF)** and **failure rate**, and fits a **Weibull distribution** to better understand failure behavior.

---

## 🎯 Objective

- Analyze time-between-failure data for a critical component of machine assembly (actuator).
- Calculate key reliability metrics (MTBF, failure rate).
- Visualize failure distributions and fit a Weibull curve.
- Identify failure trends that could improve maintenance decisions.
- In this small project we ignore data cleaning, it will be added in 

---

## 📋 Project Assumptions

- The failure data is recorded as working hours between each failure (not calendar time).
- Failures are independent events.
- The company uses identical actuator under similar operational conditions.
- The dataset is fictional or anonymized but reflects realistic behavior.
- Detection of failures is assumed to be accurate and immediate (no delays).
- The company uses thousands of such actuators on its assembly machines ( with different size and purposes ).

---

## 🧪 Methodology

### 1. **Load Data**
- Data is read from a CSV file containing failure intervals (`Actuator_Failure_Simple`).

### 2. **Calculate Reliability Metrics**
- **MTBF** is calculated as the average of failure intervals.
- **Failure Rate (λ)** is computed as the inverse of MTBF.

### 3. **Visualize Failure Data**
- A histogram is plotted to understand the spread and shape of failure intervals.

### 4. **Fit Weibull Distribution**
- Weibull distribution is fitted to the failure data to assess reliability behavior:
  - **β (shape)** parameter: tells us if failures are random, early, or wear-out.
  - **η (scale)** parameter: represents the characteristic life.

### 5. **FMEA-style Summary (Optional)**
- An FMEA table is created to describe potential failure modes, their effects, and risk levels using RPN (Risk Priority Number).

---

## 📊 Sample Output

- MTBF: `e.g., 492.5 hours`
- Failure Rate: `e.g., 0.00203 failures/hour`
- Weibull β: `> 1 → wear-out failures detected`
- Histogram and fitted Weibull curve for failure data

---

## ✅ Conclusions

- 

---

## 📂 Files in This Repository

- `hydraulic_pump_failures.csv`: Sample dataset
- `analysis_Notebook.ipynb` : Jupyter Notebook as the analysis documentation and develop code results
- `04_scripts/analysis.py`: Python script for failure analysis and automates task
- `FMEA_Template_Actuator.xlsx`: Excel sheet with FMEA summary
- `README.md`: This documentation

---

## 📌 Future Improvements
- Data cleaning
- Integrate system for another types of actuator (size, purposes)
- Compare analysis with few different assembly machine ( various machine manufacturers )
- Integrate or extend real-time analysis of sensor data from other device (e.g., pressure, temperature) for predictive analytics. (create new one project?)
- Extend the project to a full fleet and track MTBUR (Mean Time Between Unscheduled Removals).
- Visualize time-based trends for different aircraft types.


---

## 📧 Contact

For questions or collaborations, feel free to reach out via GitHub or [szqzaczek@outlook.com].

