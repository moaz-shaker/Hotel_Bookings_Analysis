![Python](https://img.shields.io/badge/Using-Python-lightblue?logo=python)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)


# 🏨 Hotel Booking Analysis — ITI Project

This project focuses on analyzing hotel booking data and building machine learning models to predict booking cancellations. The project was completed as part of an internal team effort at the Information Technology Institute (ITI).

---

## 👨‍💻 Project Members

1. Ahmed Gomaa Nazief  
2. Karim Ayman Mohammed  
3. Mohamed Hassan El Qappaney  
4. Mohamed Saeed Fathey  

---

## 📊 Dataset

- Source: [Kaggle - Hotel Booking Demand](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand/data)
- Rows: ~119,000 hotel booking records
- Features include: hotel type, lead time, cancellation status, booking channels, customer demographics, and reservation status.
- Target variable: `is_canceled` (1 = canceled, 0 = not canceled)

---

## 🧼 Data Cleaning & Preprocessing

- Removed missing values and outliers (e.g., bookings with 0 guests)
- Dropped irrelevant columns (`Unnamed: 0`)
- Converted categorical features to numerical via **Label Encoding**
- Engineered new time-based features from `reservation_status_date` (e.g., year, month, day)

---

## 📈 Exploratory Data Analysis (EDA)

- Found seasonal trends: peaks in bookings and cancellations during summer and end-of-year
- City hotels showed a **30%** cancellation rate, while resort hotels had **24%**
- Portugal (PRT) accounted for **40.9%** of cancellations
- High correlation between:
  - `reservation_status` and `is_canceled`
  - `lead_time` and `is_canceled`
  - `deposit_type` and cancellations

---

## 🤖 Machine Learning Models

We tested four classification models:

- Support Vector Machine (SVM)  
- XGBoost  
- K-Nearest Neighbors (KNN)  
- Logistic Regression  

### 🛠 Techniques Used:
- **SMOTE**: to balance the dataset (handling class imbalance)
- **Scaling**: applied `StandardScaler` and `RobustScaler` for normalization
- **Evaluation**: Accuracy, Precision, Recall, F1-Score, Confusion Matrix

### 📊 Performance Summary:
- **KNN**: ~99% accuracy  
- **SVM**: ~98.8% accuracy  
- Demonstrated strong ability to predict cancellations

---

## 📂 Files Included

- `Hotel_Bookings_Code.ipynb`: Full notebook with EDA and ML
- `Final_report.pdf`: Final version of the project report
- `hotel_bookings_Dataset.csv`: The Original Dataset
- `Cleaning_Dataset.csv`: Cleaned and formatted version
- `README.md`: This documentation file

---

## 🚀 How to Run

1. Clone this repository or download the files
2. Open `Hotel_Bookings_Code.ipynb` in Jupyter Notebook or Google Colab
3. Run all cells to follow the full analysis and modeling process

### 📦 Required Libraries

```bash
pip install pandas numpy seaborn matplotlib scikit-learn xgboost imbalanced-learn
```
---

## 🔗 Connect with Me

- [LinkedIn](https://www.linkedin.com/in/mohammed-saeed-4148b423b/)
- [GitHub](https://github.com/Mohamedsaeed12-5)

