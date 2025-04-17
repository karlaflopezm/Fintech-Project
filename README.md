# Fintech-Project

## 💰 “Predicting Personal Loan Risk Level by Analyzing Borrower Financial History, Credit Worthiness and Desired Loan Configurations”

## 📍 Industry: Finance / Fintech

### ❓ Problem
In today's fast paced lending markets, competition for market share is fierce. Technological developments like peer-to-peer lending, apps, DeFi, have lowered entry barriers for new lenders to enter the market. As banks / traditional lenders retrench (and traditional credit sources dry up) given increased regulatory pressure, opportunities emerge, but non-traditional players must act fast and offer competitive solutions in a timely manner to maintain market share and increase brand awareness. This means that non-traditional lenders able to vet, price, and approve loans quickly will have a competitive edge. As such, having a model capable of predicting loan quality / default risk is paramount to a non-traditional lending firm to stay relevant and manage risk exposure.


### 🎯 Process & Goal
Millions of people apply for personal loans every year. Banks and fintech platforms want to reduce risk and improve their approval accuracy. Consumers often get rejected without clear reasons. This can bridge that gap by building a predictive model that helps financial institutions assess loan eligibility and loan pricing more accurately and fairly using machine learning:

Process
- Use borrower financial data (credit score, income, debts, defaults, etc.) and loan needs (term, intended use of funds, etc.)
- Visualize trends and insights from the dataset
- Build a model to predict loan risk that can inform due diligence and loan pricing (risk level assignment)
- Bonus - make predictions on issued loans likely to default once issued for portfolio monitoring and risk management/planning

Goal
- Streamlining approval for low-risk loans
- Assigning pricing tiers (interest rates) fairly
- Managing high-risk loans more cautiously

---
🔍 **Objectives**

Clean and analyze real-world loan data (Lending Club)
Visualize key financial behavior and credit trends
Train and test a predictive classification model (e.g., Logistic Regression)
Optimize the model iteratively and track results
Evaluate performance with metrics like accuracy and precision

📊 **Dataset**

Lending Club Loan Dataset (Kaggle)
Sample size: ~1 million personal loans
Features: income, loan amount, DTI, employment, loan purpose, loan grade, and more

🧪 **Process Overview**

1. Data Cleaning and Preprocessing
Narrowed down the data set's 145 columns to 27 columns based on relevance of each category (handled non-accretive columns/information)
Removed missing and duplicate values
Handled outliers (e.g., income > $1M)
Converted categorical variables (e.g., loan purpose) to numerical where applicable
Bucketed data to smooth out variable distribution
Scaled numeric data (StandardScaler)

3. Exploratory Data Analysis (EDA)
Analyzed distributions of income, DTI, loan grades, interest rate levels, loan sizes
Visualized correlations between features and loan grade

3. Modeling
Model: Random Forest Classifier, Neural Networks, XGBoost

Training/Test split: 80/20

__Accuracy: ~75%, Precision: 0.81_UPDATE_

Target variable: Loan Grade (Grouped into "Low Risk" = A/B, "High Risk" = C to G)

4. Optimization
Tuned hyperparameters
Compared model metrics (accuracy, precision, recall) after each iteration
Made adjustments to identify optimal mix of hperparameters to achieve at least 75% accuracy

🛠️ **Tech Stack**

Tool/Library - Purpose
Python - Core scripting language
Pandas - Data cleaning, transformation
Matplotlib - Plotly	Visualization
Scikit-learn - ML modeling and evaluation
SQL	Data sourcing (bonus step)
Jupyter / Colab -	Analysis and development

🧠 **Key Features and Inputs**
🔢 Inputs
Income
Loan amount
Debt-to-income ratio
Employment length
Default history
Credit utilization
Loan purpose
Loan term

🧾 Outputs
Loan risk prediction (Low vs High Risk)
Confusion matrix, classification report

👥 **Team**
Asif Shahzad
José Traboulsi
Seyhr Waqas
Karla Lopez Marin

📁 **Repository Links** -----ADD-----
Google Colab Notebooks
Colab Drive Folder
GitHub Repository
Coming Soon (link to be added once pushed)

📄 **License**
Project 4 – Data Analytics Boot Camp – University of Toronto
For educational purposes only.

💡 **Next Steps (Optional Future Work)**
Using a larger data set and more advanced sampling/balancing techniques to better handle imbalanced classes and improve F1 scores
Build a web app using Streamlit or Flask for interactive use
Train a model on time-series data for portfolio risk monitoring
Integrate real-time credit bureau API (e.g., Equifax) for feature enrichment

Project4-Loan_Analysis/
│
├── 📁 data/                        # Raw and cleaned data files
│   ├── loan_data_raw.csv
│   └── loan_data_cleaned.csv
│
├── 📁 notebooks/                  # Jupyter Notebooks (EDA, model training, etc.)
│   ├── eda.ipynb
│   └── model_training.ipynb
│
├── 📁 scripts/                    # .py scripts for data cleaning, modeling, etc.
│   ├── clean_data.py
│   └── model.py
│
├── 📁 visuals/                    # Graphs, model performance charts, etc.
│   ├── feature_importance.png
│   └── confusion_matrix.png
│
├── 📁 docs/                       # Presentation slides, summary PDF, etc.
│
├── .gitignore                    # Ignore virtual env, .ipynb_checkpoints, datasets, etc.
├── README.md                     # Final project README
└── requirements.txt              # List of packages needed to run your code

