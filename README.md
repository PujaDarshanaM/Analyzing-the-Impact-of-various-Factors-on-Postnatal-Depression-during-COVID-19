# Analyzing-the-Impact-of-various-Factors-on-Postnatal-Depression-during-COVID-19
Statistical analysis project exploring the impact of maternal age, income, and education on postnatal depression levels (EPDS scores) in pregnant women during the COVID-19 pandemic using R.
This project explores the relationship between key demographic factors and the occurrence of postnatal depression among pregnant women during the COVID-19 pandemic using statistical analysis techniques in R.
As mental health challenges surged during the COVID-19 pandemic, pregnant women faced unique stressors. This study investigates how maternal age, education level, and household income are associated with depression levels as measured by the Edinburgh Postnatal Depression Scale (EPDS).

**Research Question**  
Is there a significant correlation between demographic variables (age, household income, and maternal education) and EPDS depression scores during pregnancy?

## 📊 Dataset

- Source: Kaggle – [Mental Health in the Pregnancy During the COVID-19](https://www.kaggle.com/datasets/yeganehbavafa/mental-health-in-the-pregnancy-during-the-covid-19/data)
- 10,772 responses and 16 variables
- Variables include: Maternal Age, Education, Household Income, NICU stay, Mode of Delivery, EPDS scores

##  Data Preparation

- Replaced missing values using median and random sampling
- Handled outliers using the IQR method
- Categorized maternal age, education, income, and EPDS scores
- Recoded EPDS scores into four levels:
  - 0–6: None/minimal
  - 7–13: Mild
  - 14–19: Moderate
  - 20–30: Severe

## 📈 Analysis & Visualizations

- Explored variable distributions using histograms, bar charts, and pie charts
- Created scatter plots and segmented bar charts to visualize relationships
- Used correlation heatmaps and matrices for variable relationships

## 🧪 Statistical Methods

- **Normality Testing**: Used Kolmogorov-Smirnov test due to large sample size
- **Pearson’s Chi-Square Test** & **Fisher’s Exact Test**: Found significant associations between age, income, education and EPDS categories (p < 0.001)
- **Simple Linear Regression**: Explored relationship between maternal age and EPDS scores (p < 2e-16, low R² suggests age alone is insufficient)
- **Spearman’s Rank Correlation**: Found weak to moderate negative correlations between all independent variables and depression levels
- **Ordinal Logistic Regression**: Modeled EPDS categories using all three demographic predictors with confidence intervals and residual diagnostics

## 📌 Key Findings

- Maternal age, education level, and household income are significantly associated with postnatal depression levels
- Higher income and education correlate with lower EPDS scores
- Ordinal logistic regression supported these findings with strong statistical significance

## ⚠️ Limitations

- NICU stay and mode of delivery were excluded due to missing data
- Correlation does not imply causation
- Low R² in linear regression implies presence of other unaccounted factors

## 📚 Dataset

- Kaggle Dataset: [Link](https://www.kaggle.com/datasets/yeganehbavafa/mental-health-in-the-pregnancy-during-the-covid-19)

## 🛠 Tools Used

- R
- RMarkdown
- ggplot2, dplyr
- Base R stats functions
- Data wrangling & cleaning


## Contributors
- Puja Darshana Mishra
- Ramya Keerthi Majji
- Sushruthi Panakanti
- Nikhil Chowdary Gali
