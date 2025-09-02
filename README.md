# Medical Appointments EDA 📊

This project performs **Exploratory Data Analysis (EDA)** on a dataset of medical appointments to understand the factors influencing whether patients show up for their scheduled appointments.

---

## 📌 Project Overview
The goal of this analysis is to:
- Clean and preprocess the medical appointments dataset.
- Explore demographic, social, and medical variables affecting patient behavior.
- Identify trends and correlations with the target variable **No-show** (whether a patient missed their appointment).

---

## 🛠️ Steps Performed
1. **Data Cleaning & Preparation**
   - Standardized date and time formats.
   - Extracted weekdays from `ScheduledDay` and `AppointmentDay`.
   - Renamed columns for clarity.
   - Handled missing and inconsistent values.

2. **Univariate Analysis**
   - Distribution of patient demographics (age, gender).
   - Overview of medical conditions (hypertension, diabetes).
   - Impact of receiving SMS reminders.

3. **Bivariate Analysis**
   - Correlation of predictors with **No-show**.
   - Comparison of attendance across age groups, gender.
   - Effect of scholarship status and medical conditions on attendance.

---

## 🔍 Key Findings
1. **Gender**: Female patients have taken more appointments than male patients.  
2. **Age**: Show-up rate is almost equal across most age groups, except infants (Age 0–1) with ~80% attendance.   
3. **Scholarship**:  
   - ~99,666 patients without scholarship → ~80% show rate.  
   - ~21,801 patients with scholarship → ~75% show rate.  
4. **Hypertension**:  
   - Without hypertension → 78% show rate.  
   - With hypertension → 85% show rate.  
5. **Diabetes**:  
   - Without diabetes → 80% show rate.  
   - With diabetes → 83% show rate.  
6. **SMS Reminders**:  
   - Patients without SMS → 84% show rate.  
   - Patients with SMS → lower show rate (~72%).  

---

## 📈 Conclusion
- Demographics (age, gender) play a minor role in predicting attendance.  
- Medical conditions (hypertension, diabetes) slightly improve attendance rates.  
- Surprisingly, SMS reminders **reduced** attendance likelihood, suggesting possible data quality issues or external factors.  
- Socioeconomic factor (scholarship) is linked to slightly lower attendance.  

---

## 🧰 Tools & Libraries Used
- Python (Pandas, NumPy)
- Matplotlib & Seaborn (visualization)
- Jupyter Notebook
