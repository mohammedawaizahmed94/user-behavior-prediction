# 🛒 User Behavior Purchase Prediction using Random Forest

This project simulates a machine learning pipeline to predict whether a user will make a purchase (Revenue = 1) based on their browsing behavior. The dataset is synthetically generated and mimics typical e-commerce browsing data.

---

## 📌 Project Overview

This model performs the following steps:

1. Generates synthetic data for 1000 users.
2. Creates a binary target variable (Revenue) based on simulated purchase behavior.
3. Preprocesses the features using standard scaling.
4. Splits the dataset into training and test sets.
5. Trains a *Random Forest Classifier* to predict purchase likelihood.
6. Evaluates the model with accuracy and classification report.
7. Predicts purchase intent for a new user.

---

## 🧪 Sample Output

```plaintext
Accuracy: 0.94

Classification Report:
              precision    recall  f1-score   support

           0       0.94      0.96      0.95       157
           1       0.92      0.88      0.90        43

    accuracy                           0.94       200
   macro avg       0.93      0.92      0.93       200
weighted avg       0.94      0.94      0.94       200

New Customer Purchase Prediction: 1


---

🧠 Features Used

Administrative, Informational, ProductRelated: Count of visits to various page types.

Durations: Time spent on different page categories.

BounceRates, ExitRates: Website behavior metrics.

PageValues: Value of the page based on session activity.

SpecialDay: Closeness to a special day (like holiday).



---

🚀 How to Run

1. Clone the repository:

git clone https://github.com/yourusername/user-behavior-classifier.git
cd user-behavior-classifier


2. Install dependencies:

pip install -r requirements.txt


3. Run the script:

python user_behavior_model.py




---

📦 Dependencies

Listed in requirements.txt, including:

numpy

pandas

scikit-learn



---


💡 Future Improvements

Use a real e-commerce dataset (e.g., UCI Online Shoppers Intention Dataset).

Add model tuning and cross-validation.

Visualize feature importances and confusion matrix.

Deploy the model with a Flask or Streamlit web app.