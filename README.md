## DSA210 Term Project: Impact of Economic Indicators on Stock Returns

I am Neslihan Ünal, a sophomore at Sabancı University majoring in Computer Science and pursuing a double major in Economics. My goal in this project is to analyze how macroeconomic indicators (such as GDP, unemployment, interest rates) impact stock returns.

---
## Contents
- [Motivation](#motivation)
- [Project Goals](#project-goals)
- [Hypotheses](#hypotheses)
- [Data Sources and Preprocessing](#data-sources-and-preprocessing)
  - [Data Sources](#data-sources)
  - [Data Collection](#data-collection)
  - [Data Preprocessing](#data-preprocessing)
- [Planned Data Analysis](#planned-data-analysis)
  - [Exploratory Data Analysis (EDA)](#1-exploratory-data-analysis-eda)
  - [Statistical Analysis](#2-statistical-analysis)
  - [Machine Learning Techniques](#3-machine-learning-techniques)
- [Visualization Strategy](#visualization-strategy)
- [Ethical Considerations & Limitations](#ethical-considerations--limitations)
  - [Disclaimer](#️-disclaimer)
- [Project Timeline](#project-timeline)
- [Repository Structure](#repository-structure)

---
## Motivation
Understanding the connection between macroeconomic indicators and stock market returns is crucial for investors, policymakers, and economists. Investors can use insights from economic indicators to make informed decisions, reduce risks, and identify profitable investment opportunities.

As a student at Sabancı University majoring in Computer Science and Economics, with a keen interest in financial markets, this project aligns closely with my academic goals and practical interests, helping me strengthen my analytical, economic, and programming skills.

---

## Project Goals

The main goals of this project include:
- Understanding the relationship between macroeconomic indicators (interest rates, GDP growth, inflation, unemployment rates, and exchange rates) and stock market returns.
- Identifying which economic indicators most significantly influence stock returns.
- Developing predictive models to forecast stock returns based on these indicators.

---

## Hypotheses
- **Hypothesis 1:** Stock returns are negatively correlate with increases in interest rates.
- **Hypothesis 2:** GDP growth rates positively correlate with stock returns.
- **Hypothesis 3:** Higher unemployment rates correlate negatively with stock returns.

---

## Data Sources and Preprocessing

### Data Sources:
- **Stock Price Data:**
   - Historical stock price data will be gathered from:
     - [Yahoo Finance](https://finance.yahoo.com/)
     - [Alpha Vantage API](https://www.alphavantage.co/).

- **Economic Indicator Data:**
  - Economic indicators (interest rates, GDP growth, inflation rates, unemployment rates, exchange rates) sourced from:
    - [World Bank](https://data.worldbank.org/)
    - [FRED Economic Data](https://fred.stlouisfed.org/)

### Data Collection:
- Datasets will be downloaded in CSV format through direct exports or APIs.
- Historical stock price data and economic indicators will be matched based on timestamps for accurate alignment. (i.e Data will be merged and aligned accurately based on date/time stamps.)

---

## Data Preprocessing
- Address missing data points through interpolation, averaging methods, or dropping minimal missing data points.
- Compute **log returns** for stocks to accurately measure percentage changes:

    $r_t = \ln\left(\frac{P_t}{P_{t-1}}\right)$

- Normalize economic indicator values to improve model accuracy and interpretability.

---

## Planned Data Analysis

### 1. Exploratory Data Analysis (EDA)
- Examine the distribution, volatility, and patterns in stock returns.
- Visualize trends in economic indicators over time.
- Investigate correlations between indicators and stock returns.
- Analyze correlations between indicators and stock returns via heatmaps.

### 2. Statistical Analysis
- Correlation analysis: Pearson correlation coefficients to examine relationships between returns and economic indicators.
- Statistical hypothesis tests (e.g., regression analysis, ANOVA).

### 3. Machine Learning Techniques
- Apply regression algorithms (Linear, Ridge, Lasso regression).
- Predictive modeling with machine learning algorithms like:
  - **Random Forest** (interpretability and feature importance)
  - **Gradient Boosting Machines** (high predictive performance)
- Possibly experiment with LSTM models for time series forecasting (optional).

---

## Visualization Strategy
- **Histograms and boxplots** to explore data distributions.
- **Line plots and time series charts** for stock returns and economic indicators.
- **Scatter plots and heatmaps** to represent correlation results.
- Potentially interactive visualizations (e.g., `plotly`) to clearly communicate insights.

---

## Ethical Considerations & Limitations
- All data used is publicly available and will be properly cited.
- I will clearly document the use of AI tools (e.g., ChatGPT) for guidance, if applicable.
- Results will be interpreted objectively, without bias or intentional misrepresentation.
- - The project and its outcomes are strictly educational.  
- **Not to be used as financial advice** (Disclaimer below).

### ⚠️ Disclaimer
>This project is developed strictly for educational purposes as part of my DSA210 course at Sabancı University. The analysis, data, and conclusions presented here **should not be interpreted as financial or investment advice**. I am not liable for financial decisions or any outcomes resulting from the use of this project’s analysis.

---

## Project Timeline

| Date           | Task Description                                      |
|----------------|-------------------------------------------------------|
| **March 10**   | Proposal Submission (this README.md)                  |
| April 18       | Complete Data Collection & Exploratory Analysis (EDA) |
| May 23         | Implementation of ML models                           |
| May 30         | Final Submission                                      |

---

## Repository Structure
```bash
DSA210_Economic_Indicators_Stock_Returns/
│
├── data/
│   ├── raw/           # original raw datasets
│   └── processed/      # cleaned, ready-to-analyze datasets
│
├── scripts/
│   ├── preprocessing.py
│   ├── exploratory_analysis.ipynb
│   └── predictive_modeling.ipynb
│
├── visualizations/    # Visual outputs and figures
├── requirements.txt   # Python dependencies
└── README.md          # Project details clearly documented

