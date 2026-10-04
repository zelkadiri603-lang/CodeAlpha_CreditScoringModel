Credit Scoring Model

📌 Project Overview

This project focuses on building a Credit Scoring Model using Machine Learning to predict whether a customer represents a good or bad credit risk based on financial and personal information.

The project was developed as part of a Machine Learning Internship at CodeAlpha and follows a complete machine learning workflow, from data exploration and preprocessing to model training, evaluation, and comparison.

The main objective is to develop a reliable classification model that can support credit risk assessment.

---

🎯 Objectives

The main objectives of this project are:

- Explore and understand the credit dataset.
- Clean and preprocess the data.
- Handle categorical and numerical features.
- Analyze relationships between variables and credit risk.
- Train different classification algorithms.
- Evaluate and compare model performance.
- Identify the most suitable model for credit risk prediction.

---

📊 Dataset

The project uses a credit risk dataset containing information about customers and their credit history.

The features include information such as:

- Credit history
- Loan purpose
- Credit amount
- Savings account
- Employment duration
- Installment rate
- Personal status and sex
- Age
- Housing
- Existing credits
- Number of dependents
- Other financial information

The target variable represents the customer's credit risk.

Target

The target is a binary classification problem:

- "Good Credit"
- "Bad Credit"

---

🛠️ Technologies & Libraries

The project was developed using Python and the following libraries:

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Jupyter Notebook

---

🔄 Machine Learning Workflow

The project follows these main steps:

1. Data Loading

The dataset is loaded and its structure is examined.

2. Data Exploration

The dataset is analyzed to understand:

- Number of observations and features
- Data types
- Missing values
- Duplicate records
- Distribution of the target variable
- Numerical feature distributions
- Relationships between variables

3. Data Preprocessing

The preprocessing stage includes:

- Handling missing values
- Encoding categorical variables
- Processing numerical features
- Preparing the target variable
- Splitting the data into training and testing sets

4. Exploratory Data Analysis

Different visualizations are used to identify patterns and relationships between the features and credit risk.

Examples include:

- Histograms
- Boxplots
- Countplots
- Correlation analysis
- Pairplots

5. Model Training

Several classification algorithms are considered:

- Logistic Regression
- Decision Tree
- Random Forest

These models are trained using the prepared training data.

6. Model Evaluation

The models are evaluated using several classification metrics:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

The use of multiple metrics provides a more complete evaluation of model performance, especially because both types of classification errors are important in credit risk assessment.

7. Model Comparison

The performance of the different models is compared to determine which approach provides the best results on the test data.

---

📈 Evaluation Metrics

Accuracy

Measures the proportion of correctly classified observations.

Precision

Measures how many customers predicted as a particular class actually belong to that class.

Recall

Measures how many customers belonging to a particular class were correctly identified.

F1-Score

The harmonic mean of Precision and Recall.

ROC-AUC

Measures the model's ability to distinguish between the two credit risk classes across different classification thresholds.

---

📁 Project Structure

CodeAlpha_CreditScoringModel/
│
├── data/
│   ├── german.data
│   └── german.doc
│
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   └── credit_scoring_gb_pipeline.joblib
│
├── stages/
│   └── ...
│
├── README.md
├── requirements.txt
└── .gitignore

«The project structure may be updated as the project develops.»

---

💻 Installation

Clone the repository:

git clone https://github.com/zelkadiri603-lang/CodeAlpha_CreditScoringModel.git

Navigate to the project directory:

cd CodeAlpha_CreditScoringModel

Create a virtual environment:

python -m venv .venv

Activate the virtual environment on Windows:

.venv\Scripts\activate

Install the required dependencies:

pip install -r requirements.txt

---

▶️ Usage

Open the Jupyter Notebook:

jupyter notebook

Then open:

notebooks/01_data_exploration.ipynb

Run the notebook cells sequentially to reproduce the data analysis and machine learning workflow.

---

💾 Saved Model

The trained machine learning pipeline is saved using Joblib:

credit_scoring_gb_pipeline.joblib

This allows the trained model and preprocessing steps to be reused without retraining the entire pipeline.

---

## 📌 Results

The performance comparison of the classification models evaluated on the test set:

| Model | Accuracy | Recall (Bad Risk) | Precision | F1-Score | ROC-AUC |
| :--- | :---: | :---: | :---: | :---: | :---: |
| Logistic Regression | 0.7050 | 0.4167 | 0.5102 | 0.4587 | 0.7461 |
| Random Forest | **0.7850** | 0.4500 | **0.7297** | 0.5567 | 0.7901 |
| **Gradient Boosting** | 0.7750 | **0.5167** | 0.6596 | **0.5794** | **0.8038** |

> **Note:** **Gradient Boosting** was selected as the final deployed pipeline (`credit_scoring_gb_pipeline.joblib`) because it achieved the highest **ROC-AUC (0.8038)** and **F1-Score (0.5794)**, offering the best balance for identifying credit default risks.
---

🔍 Key Insights

The exploratory data analysis helps identify important patterns related to credit risk, including the relationship between financial characteristics, credit history, and the target variable.

The comparison of several classification algorithms also helps determine which model provides the best balance between predictive performance and interpretability.

---

🚀 Future Improvements

Possible improvements include:

- Hyperparameter tuning
- Cross-validation
- Feature selection
- Handling class imbalance
- Testing additional Machine Learning algorithms
- Feature importance analysis
- Model explainability using SHAP
- Deployment as a web application or API

---

🎓 Internship

This project was developed as part of the Machine Learning Internship at CodeAlpha.

Internship Period: September 10 – October 10, 2026


---

## 👩‍💻 Author

**Zineb El Kadiri**  
*Data Science | Machine Learning | Python*  

* 🔗 **GitHub:** [@zelkadiri603-lang](https://github.com/zelkadiri603-lang)
* 💼 **LinkedIn:** [Zineb El Kadiri](https://www.linkedin.com/in/zineb-elkadiri-171057336?utm_source=share_via&utm_content=profile&utm_medium=member_android)

---

## 📄 License

This project is open-source and intended for educational and portfolio purposes.