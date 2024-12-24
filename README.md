# Medical Data Visualizer  

## Project Overview  
This project involves visualizing and analyzing medical examination data using Python libraries such as Matplotlib, Seaborn, and Pandas. The dataset contains detailed medical information collected during routine check-ups, which include body measurements, blood test results, and lifestyle factors.  

The goal is to explore relationships between these variables and cardiovascular disease, presenting the findings through informative visualizations.  

## Dataset Description  
The dataset (`medical_examination.csv`) contains rows representing patients and columns describing various medical attributes:  

| Feature                       | Description                          | Type            | Value Type                  |  
|-------------------------------|--------------------------------------|-----------------|----------------------------|  
| **Age**                       | Patient age (in days)               | Objective       | `int` (days)               |  
| **Height**                    | Height (in cm)                      | Objective       | `int`                      |  
| **Weight**                    | Weight (in kg)                      | Objective       | `float`                    |  
| **Gender**                    | Gender (categorical)                | Objective       | `int` (code)               |  
| **Systolic Blood Pressure**   | Systolic pressure (ap_hi)           | Examination     | `int`                      |  
| **Diastolic Blood Pressure**  | Diastolic pressure (ap_lo)          | Examination     | `int`                      |  
| **Cholesterol**               | Cholesterol levels                  | Examination     | `1: normal`, `2: above normal`, `3: well above normal` |  
| **Glucose**                   | Glucose levels                      | Examination     | `1: normal`, `2: above normal`, `3: well above normal` |  
| **Smoking**                   | Smoking status                      | Subjective      | `0: non-smoker`, `1: smoker` |  
| **Alcohol Intake**            | Alcohol consumption                 | Subjective      | `0: no`, `1: yes`           |  
| **Physical Activity**         | Physical activity                   | Subjective      | `0: inactive`, `1: active`  |  
| **Cardiovascular Disease**    | Presence of heart disease           | Target          | `0: no`, `1: yes`           |  

---

## Features and Instructions  

1. **Data Import and Preprocessing:**  
   - Import data from `medical_examination.csv`.  
   - Add an "Overweight" column by calculating BMI and marking values >25 as overweight.  
   - Normalize data for cholesterol and glucose (0 for normal, 1 for abnormal).  

2. **Categorical Plot Creation:**  
   - Generate a categorical plot to display counts of good and bad outcomes for cholesterol, glucose, smoking, alcohol intake, physical activity, and overweight status.  
   - Use `pd.melt` to restructure the data and `sns.catplot()` for visualization.  

3. **Heatmap Visualization:**  
   - Clean data by filtering invalid values (e.g., diastolic pressure greater than systolic).  
   - Create a heatmap showing correlations between features using a masked upper triangle for clarity.  

---

## Development  

Write your code in the `medical_data_visualizer.py` file. Use `main.py` to test your implementation.  

---

## Testing  

Unit tests are provided in `test_module.py` and are accessible via `main.py` for validation.  

---

