```markdown
# 📊 Customer Churn Prediction — Machine Learning Project

## 📊 Customer Conversion Prediction Model

**Machine Learning • Python • Scikit-learn**

---

## Project Description

This project focuses on predicting whether a customer will subscribe to a term deposit using machine learning models. It demonstrates a complete ML workflow including data exploration, preprocessing, model training, evaluation, and feature importance analysis.

The primary goal is to build a reliable prediction system leveraging classical machine learning techniques, helping businesses better understand key drivers behind customer conversion and support data-driven marketing strategies.

---

## 🚀 Project Overview

Key components of this project:

- Loading and understanding the dataset  
- Exploratory Data Analysis (EDA)  
- Cleaning and preprocessing data  
- Encoding categorical features  
- Building classification models  
- Evaluating model performance  
- Identifying key drivers behind customer conversion  

The final output provides actionable insights into customer attributes that influence subscriptions, ultimately supporting improved marketing decision-making.

---

## 📂 Dataset Details

- **Rows:** 11,162  
- **Columns:** 17  
- **Target variable:** `deposit`  
  - `1` → customer subscribed  
  - `0` → customer did not subscribe  

### Feature Types

| Type       | Examples                                |
|------------|----------------------------------------|
| Numerical  | age, balance, day, duration, etc.      |
| Categorical| job, marital, education, housing, etc. |

**Note:** The dataset contains no missing values.

---

## 🛠️ Technologies Used

- Python 3  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Jupyter Notebook / VS Code  

---

## 🔎 Exploratory Data Analysis (EDA)

Key steps in EDA included:

- Statistical summary of columns  
- Identifying duplicated rows  
- Visualizing distribution of the target variable  
- Checking numeric feature correlations  
- Understanding campaign behavior (e.g., duration, calls made)  

Example visualization:

```python
import seaborn as sns
sns.countplot(x=df["deposit"])
```

---

## 🔧 Data Preprocessing

- Converted target variable `deposit`: {`yes`: 1, `no`: 0}  
- Handled duplicate entries  
- Label encoding for categorical variables  
- Train/Test split — 80% training, 20% testing  
- Ensured clean, model-ready input data  

---

## 🤖 Machine Learning Models

Two classification models were implemented and evaluated:

| Model                 | Description                                           |
|-----------------------|-----------------------------------------------------|
| Logistic Regression   | Baseline model predicting conversion probability.     |
| Random Forest Classifier | Final model offering better accuracy and handling nonlinear relationships.|

### Model Evaluation Metrics

- Accuracy  
- Precision  
- Recall  
- F1-Score  
- Classification Report  

**Result:** Random Forest Classifier outperformed Logistic Regression on all metrics.

---

## 📈 Feature Importance Analysis

Using the Random Forest model, the top predictors influencing customer conversion included:

- `duration`  
- `pdays`  
- `previous`  
- `balance`  
- `campaign`  

This analysis provides insights into behavioral and financial factors that drive conversions.

Example feature importance plot:

```python
import seaborn as sns
sns.barplot(x=fi_series.head(15), y=fi_series.head(15).index)
```

---

## 💻 How to Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/customer-conversion-model.git
   cd customer-conversion-model
   ```

2. Create and activate a virtual environment:

   - On Windows:
     ```bash
     python -m venv venv
     venv\Scripts\activate
     ```
   - On Unix or MacOS:
     ```bash
     python3 -m venv venv
     source venv/bin/activate
     ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Run the Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

   Or open `customer_conversion.ipynb` directly using VS Code with Python extension installed.

---

## 📁 Project Structure

```
customer-conversion-model
┣ 📜 bank.csv
┣ 📜 customer_conversion.ipynb
┣ 📜 requirements.txt
┣ 📜 README.md
┗ 📂 venv/
```

---

## 📝 Results Summary

| Model                | Accuracy      |
|----------------------|---------------|
| Logistic Regression  | ~85–87%       |
| Random Forest       | ~88–92%       |

*Random Forest Classifier achieves the best balance between accuracy and interpretability.*

---

## 📌 Conclusion

This project demonstrates a complete ML pipeline for customer conversion prediction:

- Comprehensive data preprocessing  
- Exploratory data analysis and visualization  
- Multiple classification modeling approaches  
- Rigorous evaluation of models  
- Insights extraction through feature importance  

It serves as a strong portfolio project showcasing practical skills in machine learning, data analytics, and business-driven predictive modeling.

---

## 👤 Author

**Shubham Swarnakar**  
Machine Learning & Data Analytics Enthusiast  
📧 [s.swarnakar2003@gmail.com](mailto:s.swarnakar2003@gmail.com)  
🔗 [LinkedIn](https://linkedin.com/in/shubham-swarnakar-64319326a)

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).  
Feel free to use, modify, and distribute with proper attribution.

---
```
