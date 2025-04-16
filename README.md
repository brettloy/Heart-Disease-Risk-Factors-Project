# Practice in Statistical-Data-Science-Project
# Heart Disease Risk Factors: Analyzing Associations and Covariate Interactions

This project explores complex relationships between various health indicators and the risk of heart disease using statistical modeling techniques. We focus on **conditional entropy** and **odds ratios** to evaluate both individual predictor strength and interaction effects between covariates.

## 📊 Project Objective

To identify key predictors of heart disease and explore whether combinations of variables (e.g., age and general health) show synergistic effects. The analysis uses both conditional entropy and odds ratio methodologies to offer statistical and visual insights.

---

## 🧬 Dataset

- **Source**: [Behavioral Risk Factor Surveillance System (BRFSS) 2015 – Kaggle](https://www.kaggle.com/datasets/alexteboul/heart-disease-health-indicators-dataset)
- **Size**: 253,680 responses
- **Variables**: 22, including:
  - Demographics: Age, Sex, Education, Income
  - Health Indicators: HighBP, HighChol, BMI, Smoking, Stroke, Diabetes
  - Lifestyle: Physical Activity, Alcohol, Diet
  - Access to Healthcare

---

## 📐 Methods Used

### 1. **Conditional Entropy Analysis**
- Used to quantify the predictive power of each variable.
- General Health and Age were found to be the strongest predictors (lowest entropy values).
- Interaction testing between variables (e.g., Age + GenHlth, Age + PhysHlth) was performed using entropy comparisons.

### 2. **Odds Ratio Analysis**
- Quantified the likelihood of heart disease given the presence of each health condition.
- HighBP, Stroke, and Physical Inactivity emerged as top predictors.
- Two-way odds ratios explored combinations like (Stroke + HighBP) and their combined effect.

---

## 🔍 Key Findings

- **General Health** and **Age** had the most predictive power with conditional entropies of ~0.280 and ~0.284 respectively.
- **Stroke** had an odds ratio of **6.94** — individuals with a stroke were almost 7x more likely to have heart disease.
- **High Blood Pressure** had an OR of **4.59**.
- **Physical activity** and **diet** (fruits and veggies) had **protective effects** (OR < 1).
- No significant interaction effects were found between Age and GenHlth or between Age and PhysHlth — their effects were additive.

---

## 📁 Files in This Repository

- `STA_160_Midterm_Project.pdf` – Full project report
- `code/` – R scripts for entropy and odds ratio calculations
- `figures/` – Correlation heatmaps, entropy plots, bar charts
- `README.md` – Project summary and documentation

---

## 📌 Tools & Libraries

- R (ggplot2, DescTools, epitools, infotheo, dplyr)
- Entropy-based modeling
- Exploratory Data Analysis and Visualization

---

## 🧠 Limitations

- Categorical encoding of continuous variables may limit predictive resolution
- Dataset is observational, not causal
- Interaction analysis limited to pairwise combinations

---

## 🔭 Future Directions

- Use logistic regression or machine learning models for multivariate analysis
- Explore higher-order interactions or clustering methods
- Apply time-series or survival analysis for longitudinal prediction

---

## 👥 Authors

- Brett Loy  
- Yucheng Zhao  
- Abhi Gupta  
- Alexander Yu


