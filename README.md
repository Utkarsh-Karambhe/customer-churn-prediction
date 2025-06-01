# Customer Churn Prediction App 📉

This is a simple machine learning web application built with **Streamlit** that predicts whether a customer is likely to churn or not based on their demographic and service details.

## 🔍 Project Overview

Customer churn is a major issue for subscription-based businesses. This project analyzes churn patterns and predicts whether a customer is likely to leave the service using machine learning techniques.

### Key Features:
- 🔍 Exploratory Data Analysis (EDA)
- 🧹 Data Preprocessing
- 📊 Feature Engineering
- 🤖 Logistic Regression Model
- 📈 Accuracy Evaluation
- 🌐 Interactive Web App using **Streamlit**

---

## 🧠 Machine Learning Model

- **Algorithm Used**: Logistic Regression
- **Input Features**:
  - Age
  - Gender (0 = Male, 1 = Female)
  - Tenure (Number of months the customer has stayed)
  - Monthly Charges
- **Target Variable**: Churn (0 = No, 1 = Yes)

The data was scaled using **StandardScaler**, and the final model and scaler were saved as:
- `model.pkl`
- `scaler.pkl`

---

## 📦 Files in the Repository

- `notebook.ipynb` – Jupyter Notebook with full EDA, preprocessing, model training & evaluation
- `app.py` – Streamlit app source code
- `model.pkl` – Trained logistic regression model
- `scaler.pkl` – Scaler used for input normalization
- `customer_churn_data.csv` – Dataset used for model training
- `requirements.txt` – Python dependencies

---

## 🚀 Streamlit Web App

### How to Run:

```bash
pip install -r requirements.txt
streamlit run app.py
```

### App Features:
- Input fields for Age, Gender, Tenure, and Monthly Charges
- "Predict" button to show whether a customer will churn or not
- 🎈 Balloons on prediction just for fun!

---

## 📊 Data Insights

- **Dataset**: `customer_churn_data.csv`
- Missing values handled (e.g., InternetService was filled with empty string)
- Gender and Churn encoded to 0 and 1
- Correlation analysis and groupby visualizations

### Key Findings:
Churn customers generally had:
- Lower tenure
- Higher monthly charges

### Sample Visualizations:
- Pie chart for churn distribution
- Bar plots for contract type vs average monthly charge
- Histograms for tenure and monthly charges

---

## ✅ Results

- Logistic Regression achieved high interpretability
- Preprocessed features showed clear impact on churn
- Model successfully identifies at-risk customers

---

## 🛠 Technologies Used

- **Python**
- **Pandas, NumPy, Matplotlib**
- **Scikit-learn**
- **Streamlit**
- **Jupyter Notebook**

---

## 🚀 Getting Started

### Prerequisites
Make sure you have Python 3.7+ installed on your system.

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/customer-churn-prediction.git
cd customer-churn-prediction
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Run the Streamlit app:
```bash
streamlit run app.py
```

4. Open your browser and go to `http://localhost:8501`

---

## 📋 Requirements

Create a `requirements.txt` file with the following dependencies:

```
streamlit
pandas
numpy
matplotlib
seaborn
scikit-learn
pickle-mixin
```

---

## 📁 Project Structure

```
customer-churn-prediction/
│
├── app.py                      # Streamlit web application
├── notebook.ipynb              # Jupyter notebook with analysis
├── model.pkl                   # Trained model
├── scaler.pkl                  # Feature scaler
├── customer_churn_data.csv     # Dataset
├── requirements.txt            # Python dependencies
└── README.md                   # Project documentation
```

---

## 🎯 Future Enhancements

- [ ] Add more sophisticated ML models (Random Forest, XGBoost)
- [ ] Implement feature importance visualization
- [ ] Add model performance metrics dashboard
- [ ] Include data upload functionality
- [ ] Deploy to cloud platforms (Heroku, Streamlit Cloud)

---

## 👨‍💻 Author

**Utkarsh Karambhe**
- 📧 Email: utkarshkarambhe@gmail.com
- 🌐 [GitHub](https://github.com/utkarshkarambhe)
- 💼 [LinkedIn](https://linkedin.com/in/utkarshkarambhe)

---

## 📌 License

This project is open-source and free to use for educational purposes.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/yourusername/customer-churn-prediction/issues).

---

## ⭐ Show your support

Give a ⭐️ if this project helped you!

---

### ✅ Steps to Upload Your Project to GitHub

1. **Go to GitHub** and create a new repository (e.g., `customer-churn-prediction`)

2. **On your system:**
```bash
cd path_to_your_project_folder
git init
git remote add origin https://github.com/yourusername/customer-churn-prediction.git
git add .
git commit -m "Initial commit - added churn prediction app"
git branch -M main
git push -u origin main
```

3. **Update the repository URL** in this README with your actual GitHub username

4. **Add a proper requirements.txt** file with all dependencies

5. **Consider adding screenshots** of your app in action to make the README more visually appealing
