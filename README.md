Pima Indians Diabetes Risk Analysis
A comprehensive SQL analysis identifying key risk factors and patterns associated with diabetes in a population of 768 female Pima Indian patients.
🎯 Project Overview
This project uses SQL to analyze the Pima Indians Diabetes Database and uncover actionable insights about diabetes risk factors. Through 12 detailed queries, I explored relationships between patient characteristics (age, BMI, glucose levels, pregnancy history) and diabetes outcomes.
Key Question: What factors most strongly predict diabetes, and how do multiple risk factors compound?
📊 Dataset

Source: Pima Indians Diabetes Database (Kaggle)
Size: 768 patients (all female, Pima Indian heritage)
Outcome Variable: Diabetes diagnosis (0 = No, 1 = Yes)
Features: 8 medical/demographic variables including Pregnancies, Glucose, Blood Pressure, Skin Thickness, Insulin, BMI, Diabetes Pedigree Function, and Age

🔍 Key Findings
1. Glucose: Strongest Biological Predictor

Diabetic patients have 29% higher glucose levels (141 vs 109 mg/dL)
Top 25% glucose levels: 68.6% diabetes rate
Bottom 25% glucose levels: 7.3% diabetes rate
9.4x higher risk in highest vs lowest glucose quartile

2. BMI: Most Modifiable Risk Factor

Obese (BMI ≥30): 46.4% diabetes rate
Overweight (BMI 25-29.9): 22.3% diabetes rate
Normal weight (BMI 18.5-24.9): 6.9% diabetes rate
Obese individuals are 6.7x more likely to have diabetes

3. Age 30-60: Critical Risk Period

Under 30: 21.2% diabetes rate
Age 30-45: 49.6% diabetes rate (risk more than doubles!)
Age 46-60: 56% diabetes rate (highest risk)
Over 60: 25.9% diabetes rate

4. Risk Factors Compound Dramatically
Analysis of patients with 0-3 major risk factors (Age 40+, BMI 30+, Glucose 126+):

3 risk factors: 78.8% diabetes rate
2 risk factors: 53.1% diabetes rate
1 risk factor: 24.9% diabetes rate
0 risk factors: 7.0% diabetes rate

Critical Insight: Patients with all 3 risk factors are 11x more likely to have diabetes than those with none. Risk doesn't add up—it multiplies.
5. Combined Obesity + Age Over 40

Both factors present: 60.2% diabetes rate
Obese only (under 40): 41% diabetes rate
Over 40 only (not obese): 35.6% diabetes rate
Neither factor: 11.5% diabetes rate

💡 Clinical Implications

Weight Management Priority: Reducing BMI from obese to normal could prevent ~85% of diabetes cases
Early Screening: The dramatic increase at age 30 suggests screening should intensify in late 20s
Multi-Factor Assessment: The 10.5% of patients with all 3 risk factors account for 23.5% of all diabetes cases—targeting this group could have outsized impact
Glucose Monitoring: Regular screening essential, especially for patients with 2+ risk factors

🛠️ Tools & Technologies

SQL Server - All data analysis and querying
SQL Server Management Studio - Database management
Advanced SQL techniques:

Complex CASE statements for categorization
Aggregate functions (COUNT, SUM, AVG, ROUND)
Subqueries for comparative analysis
GROUP BY for segmentation
Percentile analysis using TOP PERCENT
Data quality assessment
Multi-condition filtering



📁 Repository Structure
├── README.md           # Project overview and key findings (this file)
├── queries.sql         # All SQL queries with detailed comments
└── findings.md         # Comprehensive analysis with clinical context
🚀 How to Use This Repository

Start with README.md (you're here!) for high-level insights
Review queries.sql to see the SQL code and methodology
Read findings.md for detailed analysis, interpretations, and implications


🎓 What I Learned:
How to translate business questions into SQL queries
Identifying and handling data quality issues
Creating categorical variables from continuous data
Analyzing interaction effects between multiple variables
Communicating technical findings to non-technical audiences
The importance of medical/clinical context in health data analysis

🔮 Future Enhancements

 Build interactive Tableau dashboard
 Develop predictive model using Python (logistic regression)
 Expand analysis to include interaction terms
 Compare with other demographic populations
 Time-series analysis if longitudinal data becomes available

📚 References

Pima Indians Diabetes Database: UCI Machine Learning Repository
American Diabetes Association diagnostic criteria
Clinical significance of BMI categories (WHO standards)

📬 Contact
-Anoushka Siddhada
- LinkedIn: https://www.linkedin.com/in/asiddhada/
- Email: asiddhada123@gmail.com
- Portfolio: https://github.com/asiddhada





Project completed: October 2025
Dataset: 768 patients | 12 SQL queries | 3 major risk factors analyzed
