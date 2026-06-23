# Statistic-Project-2025.2
# Comparative Experimental Analysis of Statistical, Machine Learning, and Deep Learning Methods for Time Series Forecasting

---

## Course Information

**Course:** Applied Statistics and Experimental Analysis

**Project Type:** Experimental Research Study

**Project Title:**

Comparative Experimental Analysis of Statistical, Machine Learning, and Deep Learning Methods for Time Series Forecasting

---

# 1. Project Objective

The objective of this project is to conduct a statistical and experimental comparison between traditional statistical forecasting methods, machine learning approaches, and deep learning models across multiple real-world time series datasets.

Rather than focusing solely on prediction accuracy, this project aims to analyze:

* The impact of dataset characteristics on forecasting performance.
* The strengths and weaknesses of different forecasting approaches.
* Whether traditional statistical models remain competitive.
* The statistical significance of performance differences between models.

---

# 2. Research Questions

### RQ1

Can traditional statistical forecasting methods remain competitive on small seasonal datasets?

### RQ2

Do Machine Learning methods outperform classical statistical models on complex datasets?

### RQ3

Do Deep Learning models consistently outperform simpler approaches?

### RQ4

How do dataset characteristics influence forecasting performance?

### RQ5

Are the observed differences statistically significant?

---

# 3. Research Hypotheses

### H1

Traditional statistical models perform competitively on small seasonal datasets.

### H2

Machine Learning and Deep Learning models outperform statistical methods on multivariate datasets.

### H3

No forecasting model is universally optimal across all datasets.

### H4

Dataset complexity significantly affects forecasting performance.

---

# 4. Forecasting Methods

The project compares five forecasting approaches.

## Statistical Methods

### 1. Holt-Winters Exponential Smoothing

Purpose:

Forecasting seasonal time series using level, trend, and seasonality components.

---

### 2. ARIMA

Purpose:

Classical statistical forecasting model based on autoregression and moving averages.

---

## Machine Learning Method

### 3. XGBoost

Purpose:

Tree-based machine learning model capable of capturing nonlinear patterns.

---

## Deep Learning Methods

### 4. LSTM

Purpose:

Recurrent neural network designed for sequential data.

---

### 5. Transformer

Purpose:

Attention-based architecture capable of modeling long-range temporal dependencies.

---

# 5. Datasets and Team Assignment

Each member is responsible for ONE dataset and must run ALL FIVE forecasting methods.

---

## Member 1 — Airline Passengers Dataset

### Dataset Link

https://raw.githubusercontent.com/jbrownlee/Datasets/master/airline-passengers.csv

### Dataset Characteristics

* Univariate
* 144 observations
* Strong trend
* Strong seasonality

### Research Purpose

Evaluate whether traditional statistical forecasting methods can outperform complex models on small seasonal datasets.

### Target Variable

Passengers

---

## Member 2 — Daily Minimum Temperature Dataset

### Dataset Link

https://raw.githubusercontent.com/jbrownlee/Datasets/master/daily-min-temperatures.csv

### Dataset Characteristics

* Univariate
* 3650 observations
* Environmental time series
* Moderate seasonality

### Research Purpose

Evaluate forecasting methods on real-world environmental data.

### Target Variable

Temperature

---

## Member 3 — Apple Stock Price Dataset

### Dataset Link

https://www.kaggle.com/datasets/meetnagadia/apple-stock-price-from-19802021

### Dataset Characteristics

* Multivariate
* Financial time series
* High volatility
* Nonlinear behavior

### Features

* Open
* High
* Low
* Close
* Volume

### Target Variable

Close Price

### Research Purpose

Analyze forecasting performance on financial data.

---

## Member 4 — Daily Climate Dataset

### Dataset Link

https://www.kaggle.com/datasets/sumanthvrao/daily-climate-time-series-data

### Dataset Characteristics

* Multivariate
* Weather observations
* Multiple correlated variables

### Features

* Mean Temperature
* Humidity
* Wind Speed
* Pressure

### Target Variable

Mean Temperature

### Research Purpose

Evaluate forecasting performance on multivariate climate data.

---

## Member 5 — Tetuan City Power Consumption Dataset

### Dataset Link

https://www.kaggle.com/datasets/fedesoriano/electric-power-consumption

### Dataset Characteristics

* Multivariate
* Energy forecasting
* Medium-Hard complexity

### Features

* Temperature
* Humidity
* Wind Speed
* Diffuse Flows

### Target Variable

Power Consumption

### Research Purpose

Evaluate forecasting methods on energy demand forecasting.

---

# 6. Experimental Design

## Factor A — Forecasting Method

| Level | Method       |
| ----- | ------------ |
| A1    | Holt-Winters |
| A2    | ARIMA        |
| A3    | XGBoost      |
| A4    | LSTM         |
| A5    | Transformer  |

---

## Factor B — Dataset Type

| Level | Dataset           |
| ----- | ----------------- |
| B1    | Airline           |
| B2    | Temperature       |
| B3    | Stock             |
| B4    | Climate           |
| B5    | Power Consumption |

---

## Response Variables

### Forecasting Accuracy

* MAE
* RMSE
* MAPE
* R²

### Computational Metrics

* Training Time
* Inference Time

---

# 7. Statistical Analysis

Before training models, each member must perform descriptive statistical analysis.

## Required Statistics

* Number of observations
* Mean
* Median
* Variance
* Standard Deviation
* Minimum
* Maximum
* Skewness
* Kurtosis

---

## Required Visualizations

### Histogram

Distribution analysis

### Boxplot

Outlier detection

### Time Series Plot

Trend and seasonality analysis

---

# 8. Time Series Analysis

Each member must perform:

## Trend Analysis

Identify long-term patterns.

---

## Seasonality Analysis

Identify recurring cycles.

---

## Stationarity Analysis

Method:

Augmented Dickey-Fuller (ADF) Test

Hypotheses:

H₀: Time series is non-stationary

H₁: Time series is stationary

---

## Autocorrelation Analysis

Required Visualizations:

* ACF Plot
* PACF Plot

---

# 9. Data Preprocessing

All members must follow the same preprocessing procedure.

## Missing Values

Methods:

* Forward Fill
* Interpolation

---

## Scaling

Choose one:

* MinMaxScaler
* StandardScaler

---

## Sliding Window

Window Size:

30

---

## Train-Test Split

80% Training

20% Testing

No shuffling.

---

## Random Seed

42

---

# 10. Experimental Procedure

For each dataset:

### Step 1

Descriptive Statistical Analysis

### Step 2

Time Series Analysis

### Step 3

Data Preprocessing

### Step 4

Train Holt-Winters

### Step 5

Train ARIMA

### Step 6

Train XGBoost

### Step 7

Train LSTM

### Step 8

Train Transformer

### Step 9

Evaluate Performance

### Step 10

Compare Results

---

# 11. Evaluation Metrics

Every model must report:

### MAE

Mean Absolute Error

### RMSE

Root Mean Squared Error

### MAPE

Mean Absolute Percentage Error

### R² Score

Coefficient of Determination

---

# 12. Statistical Comparison of Results

After obtaining forecasting results, perform statistical comparison.

## Paired t-Test

Purpose:

Determine whether performance differences between forecasting models are statistically significant.

### Hypotheses

H₀:

No significant difference exists between models.

H₁:

A significant difference exists.

---

## Wilcoxon Signed-Rank Test (Optional)

Used when normality assumptions are violated.

---

# 13. Individual Deliverables

Each member must submit:

### Dataset Report

* Dataset description
* Data characteristics
* Statistical summary

### EDA Report

* Visualizations
* Trend analysis
* Seasonality analysis

### Forecasting Results

Results for:

* Holt-Winters
* ARIMA
* XGBoost
* LSTM
* Transformer

### Performance Table

Including:

* MAE
* RMSE
* MAPE
* R²

### Discussion

Answer:

* Which model performed best?
* Why?
* What dataset characteristics affected performance?

---

# 14. Final Group Deliverables

## Comparative Performance Table

| Dataset     | Holt-Winters | ARIMA | XGBoost | LSTM | Transformer |
| ----------- | ------------ | ----- | ------- | ---- | ----------- |
| Airline     |              |       |         |      |             |
| Temperature |              |       |         |      |             |
| Stock       |              |       |         |      |             |
| Climate     |              |       |         |      |             |
| Power       |              |       |         |      |             |

---

## Comparative Analysis

Discuss:

* Best overall model
* Best model on small datasets
* Best model on multivariate datasets
* Statistical vs Machine Learning vs Deep Learning
* Practical recommendations

---

# 15. Expected Contribution

This project provides a comprehensive experimental study comparing:

### Statistical Forecasting

* Holt-Winters
* ARIMA

### Machine Learning

* XGBoost

### Deep Learning

* LSTM
* Transformer

across five real-world datasets from transportation, environmental science, finance, climate, and energy domains.

The focus is not only forecasting accuracy but also statistical interpretation, experimental analysis, and evidence-based conclusions.
