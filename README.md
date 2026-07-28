# ABG Motors Market Entry Analysis using Machine Learning

A machine learning case study that helps **ABG Motors**, a leading Japanese automobile manufacturer, decide whether expanding into the Indian market is commercially viable — using a Logistic Regression model trained on Japanese customer data and applied to Indian customer data to estimate potential demand.

---

## 📑 Table of Contents

- [Project Overview](#-project-overview)
- [Business Problem](#-business-problem)
- [Objectives](#-objectives)
- [Dataset Information](#-dataset-information)
- [ML Workflow](#-ml-workflow)
- [Exploratory Data Analysis](#-exploratory-data-analysis)
- [Feature Engineering](#-feature-engineering)
- [Model](#-model)
- [Model Evaluation](#-model-evaluation)
- [Business Outcome](#-business-outcome)
- [Tableau Dashboard](#-tableau-dashboard)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [How to Run](#-how-to-run)
- [Key Business Insights](#-key-business-insights)
- [Future Improvements](#-future-improvements)
- [Author](#-author)

---

## 📌 Project Overview

This project analyzes customer purchasing behavior to help ABG Motors determine whether expanding into the Indian market would be commercially viable. A **Logistic Regression** classification model was developed using historical customer data from Japan and then applied to customer data from India to estimate the number of potential buyers.

The project follows a complete Machine Learning workflow — data preprocessing, exploratory data analysis, feature engineering, model building, evaluation, and business interpretation — supported by an interactive **Tableau dashboard** comparing customer characteristics across both markets.

---

## 💼 Business Problem

ABG Motors aims to expand its operations into India and wants to estimate whether the market has sufficient potential demand before making a significant investment.

The objective of this project is to:

- Analyze customer data from the Japanese market
- Build a predictive classification model to identify potential buyers
- Apply the trained model to the Indian dataset
- Estimate the number of customers likely to purchase a vehicle
- Support the market entry decision using data-driven insights

---

## 🎯 Objectives

- Perform Exploratory Data Analysis (EDA)
- Clean and preprocess the datasets
- Engineer meaningful features
- Train a Logistic Regression classification model
- Evaluate model performance using multiple metrics
- Predict potential buyers in the Indian market
- Create an interactive Tableau dashboard for business insights

---

## 🗂 Dataset Information

The project uses two datasets:

### Japanese Dataset
Used for EDA, model training, and model evaluation.

| Feature | Description |
|---|---|
| Customer ID | Unique customer identifier |
| Current Age | Customer's age |
| Gender | Customer's gender |
| Annual Income | Customer's yearly income |
| Age of Car | Age of current vehicle |
| Purchase Status | Target variable |

### Indian Dataset
Used for predicting potential buyers and market analysis.

| Feature | Description |
|---|---|
| Customer ID | Unique customer identifier |
| Current Age | Customer's age |
| Gender | Customer's gender |
| Annual Income | Customer's yearly income |
| Date of Maintenance | Converted to Age of Car |

---

## 🔄 ML Workflow

1. Business Understanding
2. Data Loading
3. Train-Test Split
4. Exploratory Data Analysis
5. Feature Engineering
6. Data Preprocessing
7. Logistic Regression Model
8. Model Evaluation
9. Prediction on Indian Dataset
10. Business Recommendation
11. Tableau Dashboard

---

## 🔍 Exploratory Data Analysis

- Dataset information review
- Missing value analysis
- Duplicate record check
- Descriptive statistics
- Histograms
- Gender distribution
- Scatter matrix
- Boxplots
- Correlation analysis & heatmap

---

## 🛠 Feature Engineering

To improve business interpretation, **Age of Car** was grouped into meaningful categories:

- Less than 200 days
- 200–360 days
- 360–500 days
- More than 500 days

Categorical variables were encoded, and numerical variables were standardized using **Scikit-learn Pipelines**.

---

## 🤖 Model

**Algorithm Used:** Logistic Regression

**Why Logistic Regression?**
- Suitable for binary classification problems
- Easy to interpret
- Computationally efficient
- Produces probability-based predictions
- Well-suited for customer purchase prediction

---

## 📊 Model Evaluation

The model was evaluated using:

- Accuracy Score
- Confusion Matrix
- Classification Report
- ROC Curve
- ROC-AUC Score

---

## 📈 Business Outcome

After training the model on Japanese customer data, predictions were generated for the Indian dataset.

> ### Predicted Potential Buyers: **67,309 customers**

The predicted number of potential buyers significantly exceeds the business target of **12,000 annual vehicle sales**, indicating strong market potential for ABG Motors in India.

---

## 📊 Tableau Dashboard

An interactive Tableau dashboard was developed to compare customer characteristics across both markets.

**Dashboard includes:**
- Customer distribution by gender
- Annual income distribution
- Vehicle age distribution
- Purchase behaviour (Japan)
- KPI cards — Total Customers, Average Annual Income, Average Customer Age, Average Vehicle Age

<!-- Add a screenshot once available: -->
<!-- ![Dashboard Preview](Images/Dashboard.png) -->

---

## 🧰 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Tableau Public
- Jupyter Notebook

---

## 📁 Project Structure

```
ABG-Motors-Market-Entry-Analysis/
│
├── Data/
│   ├── Japanese_Dataset.csv
│   ├── Indian_Dataset.csv
│
|── Images/
│   ├── Dashboard.png
|
├──  ABG_Motors.twb
│
├──  ABG_Motors Analysis.ipynb
│
├── CAPSTONE PROJECT.pdf
│
├── README.md
```

---

## ▶️ How to Run

1. Clone the repository
   ```bash
   git clone https://github.com/jannatchugh01/ABG-Motors-Market-Entry-Analysis.git
   cd ABG-Motors-Market-Entry-Analysis
   ```
2. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```
3. Launch the notebook
   ```bash
   jupyter notebook "Notebook/ABG Motors Analysis.ipynb"
   ```
4. Open `Tableau/ABG_Motors_Dashboard.twbx` in Tableau Public or Tableau Desktop to explore the dashboard.

---

## 💡 Key Business Insights

- Annual income and vehicle age are important indicators of purchasing behaviour
- Customer demographics in India show similarities to the Japanese market
- The Logistic Regression model successfully identified potential buyers in the Indian market
- Predicted demand exceeds the company's target, suggesting India represents a promising opportunity for expansion

---

## 🚀 Future Improvements

- Evaluate additional machine learning algorithms such as Random Forest, XGBoost, and Gradient Boosting
- Incorporate customer location and behavioural features
- Perform hyperparameter tuning to further improve prediction accuracy
- Develop a real-time deployment pipeline for market prediction

---

## 👩‍💻 Author

**Jannat Chugh**
B.Tech, Electronics and Communication Engineering (AI)
Indira Gandhi Delhi Technical University for Women (IGDTUW)

[GitHub](https://github.com/jannatchugh01) • [Portfolio](https://jannatchugh01.github.io/) • [LinkedIn](https://www.linkedin.com/in/jannat-11912b28a/)

---

## 📝 Conclusion

This project demonstrates the application of Machine Learning to support strategic business decisions. By leveraging customer data from the Japanese market, a predictive model was developed to estimate demand in the Indian market. The findings indicate strong market potential, providing ABG Motors with valuable insights for evaluating its expansion strategy.
