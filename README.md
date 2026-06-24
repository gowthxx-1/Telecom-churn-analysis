Telco Customer Churn Analysis
A data analytics project that identifies why telecom customers leave, which customer segments are highest risk, and what business actions can reduce churn.

Business Problem
A telecom company is losing approximately 26.5% of its customers annually. Since acquiring a new customer costs 5–7x more than retaining an existing one, understanding and predicting churn is a critical business priority.

This project answers three core questions:

How many customers are churning?
Who exactly is churning?
Why are they churning?
Key Findings
Month-to-month contracts have a churn rate of ~43% compared to just ~3% for two-year contracts
New customers (0–12 months tenure) are the highest risk group — churn drops significantly after the first year
Fiber optic internet users churn at nearly 2x the rate of DSL users (~42% vs ~19%)
Churned customers pay ~$10 more per month on average than retained customers
Logistic Regression model achieved ~80% accuracy in predicting customer churn
Project Structure
telco-churn-analysis/
│
├── data/
│   └── churn_cleaned.csv          # Cleaned dataset exported from Python
│
├── notebooks/
│   └── Telco_Churn_Analysis.ipynb # Full analysis notebook (Colab)
│
├── images/
│   ├── churn_by_contract.png
│   ├── churn_by_tenure.png
│   ├── charges_vs_churn.png
│   ├── churn_by_internet.png
│   └── churn_drivers.png
│
├── dashboard/
│   └── churn_dashboard.pbix       # Power BI dashboard file
│
├── requirements.txt
└── README.md
Dataset
Source: IBM Telco Customer Churn Dataset (via Kaggle)
Size: 7,043 rows × 21 columns
Target variable: Churn (Yes / No)
Features include: tenure, contract type, internet service, monthly charges, total charges, payment method, and more
Tools & Technologies
Tool	Purpose
Python (pandas, numpy)	Data loading and cleaning
Matplotlib, Seaborn	Exploratory data analysis charts
Scikit-learn	Logistic Regression model
Power BI	Interactive business dashboard
Google Colab	Development environment
Analysis Workflow
Data Cleaning — Fixed TotalCharges data type, removed 11 null rows, dropped customerID
Exploratory Data Analysis — Investigated churn across contract type, tenure, internet service, and monthly charges
Machine Learning Model — Logistic Regression to predict churn and extract top churn drivers
Dashboard — Power BI dashboard summarizing all findings for business stakeholders
How to Run
Clone this repository
git clone https://github.com/yourusername/telco-churn-analysis.git
cd telco-churn-analysis
Install dependencies
pip install -r requirements.txt
Open the notebook
jupyter notebook notebooks/Telco_Churn_Analysis.ipynb
Or open directly in Google Colab

Dashboard Preview
Power BI dashboard file available in the dashboard/ folder.
Open with Power BI Desktop (free).

Author
Gowtham
B.E. Computer Science & Engineering 
SRM Madurai College for Engineering and Technology

GitHub • LinkedIn
