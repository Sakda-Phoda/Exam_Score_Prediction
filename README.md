# 🎓 Student Academic Performance Analysis & Predictive Modeling

---

## 📌 Project Overview
This project aims to analyze and identify the key factors influencing student academic success. By leveraging **Machine Learning Pipelines**, we developed a predictive model to estimate final scores and used feature importance analysis to reveal which behaviors (such as study habits and attendance) drive performance compared to demographic backgrounds.

---

## 📊 Summary of Key Findings

**1. Primary Drivers of Success: Personal Effort** *To identify the most influential factors in academic achievement.*
- **Study Hours** is the #1 predictor of success (Coefficient: 8.89). There is a strong positive correlation between time invested in self-study and final outcomes.
- **Attendance Rate** (Coefficient: 3.12) serves as a critical supporting factor, confirming that consistent classroom presence is essential for maintaining high grades.

**2. The Impact of Academic History** *To understand how past performance dictates future results.*
- Students with a history of **passing** (Passed_Yes) maintain a significant advantage (Weight: 5.57).
- Conversely, a history of **failing** (Passed_No) is the strongest negative indicator (-5.57), highlighting a "cycle of struggle" that requires early intervention.

**3. Behavioral vs. Demographic Factors** *To see if background matters as much as student behavior.*
- Interestingly, factors like **Gender, Internet Access, and Parent Education** have near-zero impact on the final score in this dataset.
- **Conclusion:** Student success is driven more by **controllable behaviors** (studying, attending) than by socioeconomic or demographic backgrounds.

**4. Model Reliability & Performance** *To ensure the accuracy of our insights.*
- The model achieved an **R² Score of 0.80** (explaining 80% of data variance).
- **5-Fold Cross-Validation** confirmed a stable **MAE of 5.54**, meaning our predictions are accurate within approximately ±6 points on average.

---

## 🛠 Tech Stack & Methodology

- **Language:** Python (Pandas, NumPy)
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn
- **Data Pipeline:** 
    - `OrdinalEncoder`: For ranked parent education data.
    - `PowerTransformer (Yeo-Johnson)`: To handle data skewness.
    - `StandardScaler`: For feature scaling.
    - `LinearRegression`: Used for interpretable predictive modeling.

---

## 📚 Data Source
**Student Academic Performance Dataset** (500 Students)  
Available on Kaggle: [Dataset Link](https://www.kaggle.com/datasets/mubashirsidiki/student-academic-performance-500-students)
