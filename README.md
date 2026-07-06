# 🎬 Movie Industry Analytics & Profitability Prediction

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-orange)
![License](https://img.shields.io/badge/License-MIT-green)


An end-to-end marketing analytics project analyzing over **5,400 movies (1980–2025)** to identify the factors that drive movie profitability. This project combines exploratory data analysis, statistical modeling, and machine learning to uncover business insights and predict movie profits.

---

## ⭐ Project Highlights

- 📊 Analyzed **5,423 IMDb movies** from 1980–2025
- 🧹 Performed data cleaning and feature engineering
- 📈 Conducted exploratory data analysis and correlation analysis
- 🤖 Built **Multiple Linear Regression, Decision Tree, and Neural Network** models
- 💼 Generated business recommendations for marketing and production strategy

---

## 💼 Skills Demonstrated

- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Statistical Analysis
- Correlation Analysis
- Multiple Linear Regression
- Machine Learning
- Data Visualization
- Predictive Modeling
- Business Analytics

---

## 🤝 Project Information

This project was completed as part of the **MKT 568 – Marketing Analytics** course at **Worcester Polytechnic Institute**.

While the project was submitted as a team assignment, this repository documents **my implementation and primary contributions**, including data preprocessing, feature engineering, exploratory data analysis, statistical modeling, machine learning, visualization, and project documentation.

---

## 📌 Project Overview

The entertainment industry invests millions into movie production, yet not every high-budget film becomes profitable. This project explores historical movie data to answer key business questions about revenue, profitability, audience engagement, and release strategies.

### Objectives

- Analyze factors influencing movie profitability
- Identify high-performing genres, ratings, and release periods
- Examine relationships between movie characteristics and profit
- Build predictive models to estimate movie profitability
- Provide data-driven recommendations for marketing and production teams

---
## 📊 Dataset

This project uses the **Movie Industry** dataset by Daniel Grijalva, available on Kaggle.

**Dataset:** https://www.kaggle.com/datasets/danielgrijalvas/movies

The version used in this project (`IMDb_Movies.csv`) contains **5,438 movies** and **15 original features**. After removing records with a small number of missing values, **5,423 movies** remained for analysis. Additional variables were engineered during preprocessing, including inflation-adjusted budget, profit, release month, release season, release day bins, movie title length, and years since production.

| Attribute | Details |
|-----------|----------|
| Source | IMDb Movie Industry Dataset (Kaggle) |
| Kaggle Author | Daniel Grijalva |
| Original Dataset | 5,438 movies |
| Final Dataset Used | 5,423 movies |
| Original Features | 15 |
| Engineered Features | 10+ |

### Key Variables

- Budget
- Gross Revenue
- Inflation-adjusted Budget
- Profit
- IMDb Score
- IMDb Votes
- Genre
- Rating
- Runtime
- Release Month
- Release Season
- Release Day Bin
- Years Since Production
- Movie Name Length


---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Statsmodels
- SciPy
- Jupyter Notebook
- graphviz

---

# 🔄 Project Workflow

```text
IMDb Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Feature Engineering
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Correlation Analysis
      │
      ▼
Regression Analysis
      │
      ▼
Machine Learning Models
      │
      ▼
Business Recommendations
```

---

# 📈 Exploratory Data Analysis

## 1. Average Gross Revenue by Genre

<img width="940" height="515" alt="image" src="https://github.com/user-attachments/assets/628f4ea1-4931-4fde-94fa-31f19865e50a" />


### Key Insight

- Animation generated the highest average gross revenue.
- Family and Action movies consistently outperformed most genres.
- Western and Romance films earned comparatively lower revenue.

---

## 2. Average Profit by Genre

<img width="940" height="527" alt="image" src="https://github.com/user-attachments/assets/aef2f707-90ab-46ad-923f-34547c29135b" />


### Key Insight

- Animation and Family films achieved the highest average profitability.
- Mystery and Horror genres also generated strong profits.
- Higher revenue does not necessarily translate into higher profitability.

---

## 3. Average Gross Revenue by Release Month

<img width="940" height="495" alt="image" src="https://github.com/user-attachments/assets/bda79d67-8d3f-412b-bc1a-9fc2718b7fa5" />


### Key Insight

- June recorded the highest average gross revenue.
- May, July, November, and December also showed strong box office performance.
- Summer and holiday release windows remain the most favorable.

---

## 4. Average Profit by Season

<img width="940" height="512" alt="image" src="https://github.com/user-attachments/assets/ec420295-43cc-407f-900f-70f3bfc4df0a" />


### Key Insight

- Summer releases produced the highest average profits.
- Winter and Spring followed closely.
- Fall releases were comparatively less profitable.

---

## 5. IMDb Score vs Profit

<img width="940" height="516" alt="image" src="https://github.com/user-attachments/assets/0f49fe1d-bdff-411e-a727-fe8d58fea52f" />


### Key Insight

- Weak positive correlation (**r = 0.28**)
- Higher IMDb ratings alone are not strong predictors of profitability.

---

## 6. IMDb Votes vs Profit

<img width="940" height="528" alt="image" src="https://github.com/user-attachments/assets/4be7ee52-4d4a-4aaa-a2ac-dda98e66cc32" />


### Key Insight

- Moderate positive correlation (**r = 0.63**)
- Movies receiving greater audience engagement tend to generate substantially higher profits.

---

# 📉 Correlation Analysis

| Variable | Correlation with Profit |
|-----------|------------------------:|
| Gross Revenue | **0.80** |
| IMDb Votes | **0.63** |
| Budget | **0.30** |
| IMDb Score | **0.28** |
| Runtime | **0.11** |

### Key Findings

- Gross revenue is the strongest predictor of profitability.
- Audience engagement has a significant influence on financial success.
- Budget alone is not a reliable indicator of profit.
- Runtime has little impact on profitability.

---

# 🤖 Predictive Modeling

Three predictive approaches were developed to estimate movie profitability.

| Model | Purpose |
|---------|---------|
| Multiple Linear Regression | Identify statistically significant profitability drivers |
| Decision Tree Regressor | Predict movie profitability using nonlinear relationships |
| Neural Network | Capture complex patterns in the dataset |

### Model Performance

- Decision Tree achieved the strongest predictive performance (**R² ≈ 0.52**).
- Regression analysis identified the most influential business variables.
- Machine learning provided practical estimates for future movie profitability.

---

# 💡 Business Recommendations

Based on the analysis:

- Focus investment on high-performing genres such as **Animation, Family, and Action**.
- Schedule major releases during **May–July** and **December** to maximize revenue.
- Increase marketing efforts that improve audience engagement and visibility.
- Optimize production budgets rather than assuming higher spending guarantees success.
- Use predictive analytics to support release planning and investment decisions.

---

# 🚀 Future Improvements

- Build an interactive Streamlit dashboard
- Implement XGBoost and Random Forest models
- Incorporate movie review sentiment analysis
- Predict opening weekend revenue
- Deploy the project as a web application

---

# 📂 Repository Structure

```
movie-industry-analytics/
│
├── data/
│   └── IMDb_Movies.csv
│
├── notebooks/
│   └── Movie_Industry_Analytics.ipynb
│
├── reports/
│   ├── Movie_Industry_Analytics_Report.pdf
│   └── Presentation.pdf
│
├── images/
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```
---

# ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/VaishnaviChandalada/movie-industry-analytics.git
```

2. Install the required Python libraries:

```bash
pip install -r requirements.txt
```

3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `Movie_Industry_Analytics.ipynb` and run the notebook to reproduce the analysis and visualizations.

---

## 📄 Project Documentation

For a detailed explanation of the methodology, statistical analysis, predictive modeling, and business recommendations, see:

- 📘 **Full Project Report:** [Movie_Industry_Analytics_Report.pdf](Movie_Industry_Analytics_Report.pdf)
- 📊 **Presentation Slides:** [Presentation.pdf](Presentation.pdf)

---

# 👩‍💻 Author

**Vaishnavi Chandalada**

MBA Business Analytics  
Worcester Polytechnic Institute

- LinkedIn: https://www.linkedin.com/in/vaishnavi-chandalada-1abab0222/
- GitHub: https://github.com/VaishnaviChandalada
