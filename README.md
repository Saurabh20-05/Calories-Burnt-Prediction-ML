# 🔥 Calories Burnt Prediction using XGBoost Regression

This project uses **XGBoost Regression** to predict the **number of calories burnt** by a person during physical activity based on physiological and workout-related parameters such as age, gender, height, weight, duration, heart rate, and body temperature.

The model is trained on real-world fitness datasets to accurately estimate calorie expenditure.

---

## 📘 Project Overview

This is a **Supervised Machine Learning** based **Regression** project.

By analyzing personal and exercise-related attributes, the model predicts the **continuous value of calories burnt** during exercise.

The goal is to build an **accurate, efficient, and reliable calorie prediction system** using the **XGBoost Regressor**.

---

## 🗂️ Dataset Information

### Dataset Names
- **Calories Dataset** → `calories.csv`
- **Exercise Dataset** → `exercise.csv`

### Description
- `exercise.csv` contains **user details and exercise parameters**
- `calories.csv` contains **calories burnt values**

Both datasets are merged using Pandas to form a single dataframe for training.

---

## 📌 Columns Description

- **User_ID** → Unique user identifier  
- **Gender** → Male / Female  
- **Age** → Age of the person  
- **Height** → Height (in cm)  
- **Weight** → Weight (in kg)  
- **Duration** → Exercise duration (in minutes)  
- **Heart_Rate** → Heart rate during exercise  
- **Body_Temp** → Body temperature  
- **Calories** → Calories burnt (Target Variable)

---

## 🎯 Target Variable

- **Calories**  
  → Continuous numerical value representing calories burnt

---

## 🧠 Technologies Used

- Python 3.x  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Scikit-learn  
- XGBoost  

---

## ⚙️ Project Workflow

1. Import required Python libraries  
2. Load `calories.csv` and `exercise.csv` using Pandas  
3. Merge both datasets into a single dataframe  
4. Perform exploratory data analysis:
   - `head()`, `shape`, `info()`, `describe()`
   - Check missing values  
5. Data visualization:
   - Count plot for Gender
   - Histogram plots for Age, Height, and Weight  
6. Encode categorical data:
   - Gender → Male: 0, Female: 1  
7. Perform correlation analysis using heatmap  
8. Split features and target:
   - **X** → All columns except `User_ID` and `Calories`
   - **Y** → Calories  
9. Split dataset into:
   - 80% Training data
   - 20% Testing data  
10. Train the model using **XGBoost Regressor**  
11. Evaluate the model using **Mean Absolute Error (MAE)**  
12. Build a predictive system for custom user input  

---

## 📊 Model Performance

### ✅ Evaluation Metric Used
- **Mean Absolute Error (MAE)**

### ✅ Result
- The model achieves **low MAE**, indicating accurate calorie prediction.
- Good generalization on unseen test data.

---

## 🧪 Predicting Custom Input

You can predict calories burnt by providing custom input in the following format:

input_data = (1, 27, 154.0, 58.0, 10.0, 81.0, 39.8)
**Gender, Age, Height, Weight, Duration, Heart_Rate, Body_Temp**

### 🔍 Output: Calories Burnt = <Predicted Value>

---

## 👨‍💻 Author

**Developed by Saurabh**

Feel free to connect, explore, or contribute to this project!

---

⭐ If you found this project helpful, don’t forget to **star the repository**!
