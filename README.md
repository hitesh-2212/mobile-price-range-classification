# 📱 Mobile Price Range Classification

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/fa229947-40b4-4427-bab8-dacd7b51243d" />

## 📌 Project Overview
This project aims to classify mobile phones into different **price ranges** (Low, Medium, High, Premium) based on their technical specifications. Instead of predicting the exact price, the model identifies the appropriate price category to support data-driven pricing decisions in a competitive smartphone market.

---

## 🎯 Problem Statement
A new mobile manufacturing company wants to estimate the price range of its devices using features such as RAM, battery power, screen resolution, and storage. Incorrect pricing can lead to revenue loss or reduced market competitiveness. This project solves the problem using **machine learning classification techniques**.

---

## 🗂️ Dataset Description
- Cleaned dataset (no missing values or duplicates)
- Numeric and binary features
- Target variable: `price_range` (0 = Low, 3 = Premium)

---

## 🔍 Exploratory Data Analysis (EDA)
Key insights from EDA:
- 📌 **RAM is the strongest predictor** of price range
- 🔋 Battery power and 📺 screen resolution have moderate influence
- 📷 Camera and 📡 connectivity features have limited impact
- Dataset is perfectly balanced across all price categories

---

## 🤖 Models Used
| Model | Purpose | Validation Accuracy |
|-----|--------|--------------------|
| Logistic Regression | Baseline & Final Model | **96.5%** |
| Decision Tree | Non-linear baseline | 83% |
| Tuned Decision Tree | Reduced overfitting | 85% |
| Random Forest | Ensemble model | 87.75% |

---

## ✅ Final Model Selection
**Logistic Regression** was finalized because:
- Highest validation accuracy
- Strong interpretability
- Stable and generalizable performance
- Business-friendly explanations

---

## ⚙️ Feature Scaling
- Used `StandardScaler`
- Fitted only on training data
- Applied consistently to validation and test data
- Prevented data leakage

---

## 📊 Feature Importance Summary
**Top features influencing price range:**
1. RAM ⭐⭐⭐⭐⭐
2. Battery Power ⭐⭐⭐⭐
3. Screen Resolution (px_width, px_height) ⭐⭐⭐
4. Internal Memory ⭐⭐

---

## 📈 Results
- Strong classification performance
- Minimal confusion between non-adjacent price ranges
- Clear linear separability in data

---

## 🏁 Conclusion
This project shows that **simpler models can outperform complex ones** when feature relationships are strong and linear. Logistic Regression proved to be the most effective solution for mobile price range classification.

---

## 🛠️ Tools & Libraries
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

---

## 👤 Author
**Hitesh Kumar**  
_Data Analyst / Machine Learning Enthusiast_
