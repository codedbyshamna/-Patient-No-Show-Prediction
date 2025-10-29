# 🏥 Patient No-Show Prediction

## 📌 Overview
This project focuses on predicting whether a patient will **show up for a scheduled medical appointment** using data-driven insights and machine learning.  
By analyzing patient demographics, appointment details, and communication factors, the project identifies key patterns that influence **patient attendance**.

This project was developed as part of a **Mini Data Science Project**, implementing concepts of data cleaning, visualization, and prediction.

---

## 🎯 Objectives
- Understand the behavior and trends behind missed medical appointments.
- Explore and clean healthcare appointment data.
- Visualize the relationship between patient attributes and attendance.
- Build a predictive model to classify whether a patient will attend.
- Evaluate and interpret model performance.

---

## 📂 Dataset Description
**Dataset Name:** `patients_no_show.csv`

| Column Name | Description |
|--------------|-------------|
| `PatientId` | Unique ID of each patient |
| `AppointmentID` | Appointment reference number |
| `Gender` | Gender of the patient |
| `ScheduledDay` | Date and time when the appointment was scheduled |
| `AppointmentDay` | Date and time of the appointment |
| `Age` | Age of the patient |
| `Neighbourhood` | Location of the hospital |
| `Scholarship` | Whether the patient is on welfare (1 = Yes, 0 = No) |
| `Hypertension` | Whether the patient has hypertension |
| `Diabetes` | Whether the patient has diabetes |
| `Alcoholism` | Whether the patient has alcoholism |
| `Handcap` | Indicates any disability |
| `SMS_received` | Whether an SMS reminder was sent |
| `No-show` | Target variable (Yes = did not attend, No = attended) |

---

## 🧠 Workflow

### 1. **Data Exploration and Preprocessing**
- Handled missing values and corrected data types.
- Converted datetime features to extract useful insights (e.g., waiting days).
- Encoded categorical variables like gender and no-show.

### 2. **Exploratory Data Analysis (EDA)**
- Distribution of attendance by **gender**, **age**, and **neighbourhood**.
- Relationship between **waiting time** and likelihood of no-show.
- Impact of **SMS reminders** and **health conditions**.

### 3. **Feature Engineering**
- Created new variables such as waiting days and binary encodings.
- Normalized and scaled numerical features for model compatibility.

### 4. **Model Building**
- Implemented and compared classification models:
  - Logistic Regression  
  - Decision Tree  
  - Random Forest  
- Selected the best-performing model based on accuracy and recall.

### 5. **Evaluation Metrics**
- Accuracy Score  
- Confusion Matrix  
- Precision & Recall  
- F1 Score  

---

## 📊 Key Insights
- **Younger patients** were more likely to miss appointments.  
- **Receiving an SMS reminder** decreased the no-show rate.  
- A **longer gap** between scheduling and the appointment date increased the chance of no-shows.  
- Patients with **chronic conditions** (e.g., hypertension, diabetes) were more likely to attend.  

---

## 🛠️ Tools & Technologies
- **Python**
  - Libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
- **Google Colab / Jupyter Notebook**
- **GitHub** for version control and documentation
