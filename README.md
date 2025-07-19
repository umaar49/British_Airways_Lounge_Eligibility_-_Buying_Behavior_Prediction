# ✈️ Lounge Eligibility & Buying Behavior Prediction – British Airways

This project predicts whether a customer will complete a booking based on their flight behavior and preferences. Using a real airline dataset, I performed data cleaning, exploratory data analysis, feature engineering, and trained a Random Forest Classifier. The project was developed during a virtual internship with British Airways on the Forage platform.

---

## 📁 Project Files

| `Lounge_Eligibility_Prediction.ipynb` | Full Jupyter notebook with data cleaning, EDA, feature engineering, model training, and evaluation |
| `Lounge Eligibility & Buying Behavior Prediction.pdf` | Project report summarizing key steps and findings |
| `customer_booking.csv` | Dataset provided by British Airways (used for prediction) |
| `README.md` | This documentation file |

---

## 📊 Dataset Overview
- 📌 Dataset Source:
      [(https://www.kaggle.com/datasets/deepakb4/british-airways-customer-bookings)]
      (I do not own this dataset — used for educational purposes only)
- Size: 50,000 records
- Features:
  - Passenger and booking info (`num_passengers`, `purchase_lead`, `length_of_stay`)
  - Preferences (`wants_extra_baggage`, `wants_in_flight_meals`, `wants_preferred_seat`)
  - Travel details (`route`, `booking_origin`, `flight_hour`, `flight_day`)
  - Target variable: `booking_complete` (0 = not booked, 1 = booked)

---

## 🔧 Data Cleaning & Feature Engineering

- Converted `flight_day` to numerical format (Mon=1 to Sun=7)
- Extracted `Origin_Country` and `Destination_Country` from `route`
- Created `Day Timing` feature based on `flight_hour` (AM/PM)
- Encoded categorical features using one-hot encoding
- Grouped less frequent categories into an `other` class

---

## 📊 Exploratory Data Analysis (EDA)

- Analyzed the distribution of booking completion
- Visualized relations between categorical features and target
- Boxplots for numeric features vs. booking status
- Heatmap to understand correlation between features

---

## 🧠 Machine Learning

- Model | Random Forest Classifier |
- Pipeline | Scikit-learn pipeline with StandardScaler and model |
- Split | Train-test (80/20) |
- Tuning | GridSearchCV used to find best hyperparameters |

### ✅ Model Evaluation:
- Accuracy: ~85%
- Precision for class 1: ~45%
- Classification Report and Confusion Matrix
- Feature Importance: `purchase_lead`, `length_of_stay`, `num_passengers`, and `booking_origin`

---

## 🛠️ Tools & Libraries Used

- Python (Pandas, NumPy)
- Matplotlib & Seaborn (for visualization)
- Scikit-learn (ML model, pipeline, and evaluation)
- Jupyter Notebook

---

## 📌 Key Learning Outcomes

- Real-world data preprocessing and feature extraction
- Analyzing travel behavior patterns
- Building classification models using Scikit-learn pipelines
- Understanding feature importance for business decisions
- Model tuning using GridSearchCV

---

## 📫 About Me

**Muhammad Umar Saleem**
Electrical Engineering Graduate (June 2025)  
Aspiring Data Scientist | Machine Learning & IoT Enthusiast  
[LinkedIn](www.linkedin.com/in/umarsaleem49))


