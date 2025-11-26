📊 Customer Conversion Prediction Model

Machine Learning • Python • Scikit-learn

This project focuses on predicting whether a customer will subscribe to a term deposit using machine learning models. It demonstrates a complete ML workflow including data exploration, preprocessing, model training, evaluation, and feature importance analysis.

🚀 Project Overview

The objective of this project is to build a prediction system using classical machine learning techniques.
This includes:

Loading and understanding the dataset

Performing exploratory data analysis (EDA)

Cleaning and preprocessing data

Encoding categorical features

Building classification models

Evaluating model performance

Identifying key drivers behind customer conversion

The final output helps understand which customer attributes influence conversion and supports better marketing decisions.

📂 Dataset Details

The dataset contains 11,162 rows and 17 columns representing customer demographics, financial history, campaign interactions, and the final conversion status.

Target Variable:
deposit → mapped as:

1 → customer subscribed

0 → customer did not subscribe

Feature Types Include:

Numerical: age, balance, day, duration, etc.

Categorical: job, marital, education, housing, etc.

No missing values were found in the dataset.

🛠️ Technologies Used

Python 3

Pandas, NumPy

Matplotlib, Seaborn

Scikit-learn

Jupyter Notebook / VS Code

🔎 Exploratory Data Analysis (EDA)

Key steps in EDA included:

Statistical summary of all columns

Identifying duplicated rows

Visualizing distribution of the target variable

Checking numeric correlations

Understanding campaign behavior (duration, calls made, etc.)

Example:

sns.countplot(x=df["deposit"])

🔧 Data Preprocessing

Binary conversion of target variable
deposit → {yes: 1, no: 0}

Handling duplicates

Label Encoding for categorical features

Train/Test split (80/20)

Ensuring clean and model-ready data

🤖 Machine Learning Models

Two models were implemented:

✔ Logistic Regression

Simple baseline model used to predict probability of customer conversion.

✔ Random Forest Classifier

Final model due to superior accuracy and ability to capture nonlinear patterns.

Both models were evaluated using:

Accuracy

Precision

Recall

F1-score

Classification report

Random Forest showed the best performance overall.

📈 Feature Importance Analysis

A feature importance plot (Random Forest) highlights the top predictors:

duration

pdays

previous

balance

campaign

These insights help in understanding behavioral and financial factors driving conversions.

Example code used:

sns.barplot(x=fi_series.head(15), y=fi_series.head(15).index)

💻 How to Run the Project
1. Clone the project
git clone https://github.com/yourusername/customer-conversion-model.git
cd customer-conversion-model

2. Create and activate virtual environment
python -m venv venv
venv\Scripts\activate

3. Install dependencies
pip install -r requirements.txt

4. Run Jupyter Notebook
jupyter notebook


Or simply open the notebook directly in VS Code.

📁 Project Structure
📦 customer-conversion-model
 ┣ 📜 bank.csv
 ┣ 📜 customer_conversion.ipynb
 ┣ 📜 requirements.txt
 ┣ 📜 README.md
 ┗ 📂 venv/

📝 Results Summary
Model	Accuracy
Logistic Regression	~85–87%
Random Forest	~88–92%

Random Forest achieves the best balance of accuracy and interpretability.

📌 Conclusion

This project demonstrates a complete ML workflow for predicting customer conversion.
It includes data preprocessing, modeling, evaluation, and extracting actionable insights that can support business decision-making and targeted marketing campaigns.

It serves as a strong portfolio project showcasing:

ML pipeline creation

Data analysis and visualization

Classification modeling

Feature engineering

Model evaluation

Insight-driven storytelling

👤 Author

Shubham Swarnakar
Machine Learning & Data Analytics Enthusiast
📧 s.swarnakar2003@gmail.com

🔗 linkedin.com/in/shubham-swarnakar-64319326a