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
     
     ![image alt](https://github.com/MRUDULA007/-Medical-Appointments-EDA/blob/ffd81aedfae68dfbb007b551f5756c88bc0e49dd/Distribution%20of%20Patient%20Age.png)
     
     ![image alt](https://github.com/MRUDULA007/-Medical-Appointments-EDA/blob/ffd81aedfae68dfbb007b551f5756c88bc0e49dd/Distribution%20of%20Gender.png)

   - Overview of medical conditions (hypertension, diabetes).
     
     ![image alt](https://github.com/MRUDULA007/-Medical-Appointments-EDA/blob/ffd81aedfae68dfbb007b551f5756c88bc0e49dd/Overview%20of%20medical%20conditions%20(Hypertension%2C%20Diabetes).png)
     
   - Impact of receiving SMS reminders.
     
     ![image alt](https://github.com/MRUDULA007/-Medical-Appointments-EDA/blob/ffd81aedfae68dfbb007b551f5756c88bc0e49dd/Impact%20of%20receiving%20SMS%20reminders.png)

3. **Bivariate Analysis**
   - Correlation of predictors with **No-show**.
  
     ![image alt](https://github.com/MRUDULA007/-Medical-Appointments-EDA/blob/683288a2048cc8fb6fda058b5424dfe48b35905c/Correlation%20of%20predictors%20with%20No-show..png)
     
   - Comparison of attendance across age groups, gender.
     
![image alt](https://github.com/MRUDULA007/-Medical-Appointments-EDA/blob/43782af8b9b97d1e937f6466799c10603d767e81/Comparison%20of%20attendance%20across%20%20gender..png)

![image alt](https://github.com/MRUDULA007/-Medical-Appointments-EDA/blob/43782af8b9b97d1e937f6466799c10603d767e81/Comparison%20of%20attendance%20across%20age%20groups.png)

   - Effect of scholarship status and medical conditions on attendance.
   - 
![image alt](https://github.com/MRUDULA007/-Medical-Appointments-EDA/blob/43782af8b9b97d1e937f6466799c10603d767e81/Effect%20of%20Scholarship%2C%20Hypertension%2C%20Diabetes.png)

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
