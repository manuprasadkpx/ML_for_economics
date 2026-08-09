# ML_for_economics
A beginner-friendly Machine Learning repository for Economics students, covering ML concepts, Python implementations, datasets, notebooks, econometric applications, and practical projects. Designed as a one-stop learning resource to help students understand, practice, and apply machine learning in academics and research.

# Machine Learning for Economics

A beginner-friendly introduction to Machine Learning for students of Economics, Econometrics, Finance, and related disciplines.

This repository connects fundamental Machine Learning algorithms with classic economic and financial problems. Each model includes a practical dataset, Python implementation, data analysis, model evaluation, and interpretation of results.

---
# Machine Learning for Economics

A practical and beginner-friendly repository for learning Machine Learning through Economics, Econometrics, Finance, and real-world economic problems.

This repository is designed primarily for students who already have basic knowledge of Python, statistics, economics, or econometrics and want to understand how Machine Learning can be applied to economic data.

The central idea of this repository is:

**Economic Problem → Data → Model → Prediction → Evaluation → Interpretation → Economic Insight**

---

## Why Machine Learning for Economics?

Economics has traditionally relied heavily on statistical and econometric methods to understand relationships between variables, test hypotheses, estimate parameters, and evaluate policies.

Machine Learning provides a complementary approach that is particularly powerful when the objective is prediction, classification, pattern recognition, or dealing with large and complex datasets.

Economic datasets can contain thousands or millions of observations across:

- Individuals
- Households
- Firms
- Banks
- Countries
- Regions
- Financial assets
- Products
- Time periods

Machine Learning can help identify nonlinear relationships, interactions, complex patterns, and predictive signals that may be difficult to capture using simple parametric models.

However, an important distinction must always be remembered:

> **Prediction is not the same as causality.**

A Machine Learning model can predict that people with higher education tend to have higher wages, but this alone does not prove that increasing education causes higher wages.

Therefore, this repository treats Machine Learning as a complement to Economics and Econometrics rather than a replacement for economic theory or causal inference.

---

# Models Covered

This repository focuses on ten fundamental Machine Learning techniques that provide a strong foundation for students interested in Economics, Econometrics, Finance, and Data Science.

| No. | Model | Learning Type | Main Purpose | Economic Example |
|---|---|---|---|---|
| 01 | Linear Regression | Supervised | Regression | Wage Prediction |
| 02 | Logistic Regression | Supervised | Classification | Loan Default |
| 03 | Decision Tree | Supervised | Classification / Regression | Unemployment |
| 04 | Random Forest | Supervised | Classification / Regression | House Prices |
| 05 | K-Means | Unsupervised | Clustering | Consumer Segmentation |
| 06 | Support Vector Machine | Supervised | Classification / Regression | Financial Distress |
| 07 | Naive Bayes | Supervised | Classification | Economic Text Classification |
| 08 | Principal Component Analysis | Unsupervised | Dimensionality Reduction | Economic Activity Index |
| 09 | XGBoost | Supervised | Classification / Regression | Credit Risk & Forecasting |
| 10 | Neural Networks | Supervised | Regression / Classification | GDP & Financial Prediction |

---

# 01. Linear Regression

Linear Regression is one of the most fundamental Machine Learning models and provides an important bridge between Econometrics and Machine Learning.

The model attempts to predict a continuous variable using one or more explanatory variables.

A basic specification is:

`Y = β₀ + β₁X₁ + β₂X₂ + ... + ε`

## Economic Example: Wage Determination

A classic application is predicting an individual's wage using education and work experience.

**Research question:**

> Can education and work experience predict an individual's wage?

Possible variables include:

- Education years
- Work experience
- Age
- Gender
- Occupation
- Location

The target variable could be hourly wage or annual income.

A simple economic model could be:

`Wage = β₀ + β₁Education + β₂Experience + ε`

## Analysis

Students can:

- Explore the distribution of wages
- Calculate descriptive statistics
- Examine correlations
- Visualize education and wages
- Split the data into training and testing sets
- Train the model
- Generate predictions
- Analyse residuals
- Compare actual and predicted wages

## Evaluation

Common regression metrics include:

- R²
- Adjusted R²
- MAE
- MSE
- RMSE

## Applications in Economics

Linear Regression can be applied to:

- Wage determination
- Consumption estimation
- Investment analysis
- GDP prediction
- Demand estimation
- Housing prices
- Inflation modelling
- Tax revenue prediction
- Energy consumption
- Carbon emissions

## Connection with Econometrics

Linear Regression is especially useful for Economics students because it provides a natural introduction to the difference between:

**Prediction**

and

**Statistical inference / causal interpretation**

The same regression model can be used in both econometrics and Machine Learning, but the objectives, validation methods, and interpretation may differ.

---

# 02. Logistic Regression

Logistic Regression is a supervised Machine Learning algorithm used primarily for binary classification.

Instead of predicting a continuous value, the model estimates the probability of an event.

For example:

`Default = 1`

`No Default = 0`

## Economic Example: Loan Default Prediction

**Research question:**

> Can we predict whether a borrower will default on a loan?

Possible features include:

- Annual income
- Credit score
- Debt-to-income ratio
- Loan amount
- Employment status
- Age
- Previous defaults

The target variable is:

`0 = No Default`

`1 = Default`

The model produces a probability such as:

`P(Default = 1) = 0.73`

This means the model estimates a 73% probability of default.

## Analysis

Students can examine:

- Default rates
- Credit-score distributions
- Income distributions
- Debt-to-income relationships
- Predicted probabilities
- Classification thresholds
- Confusion matrices
- ROC curves

## Evaluation

Classification metrics include:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- PR-AUC
- Confusion Matrix

Accuracy should not be used alone when the classes are highly imbalanced.

## Applications in Economics and Finance

Logistic Regression can be used for:

- Credit scoring
- Loan default
- Bankruptcy prediction
- Employment probability
- Poverty classification
- Financial distress
- Financial inclusion
- Program participation
- Consumer churn

---

# 03. Decision Tree

A Decision Tree predicts an outcome by repeatedly splitting observations according to their characteristics.

The model can be interpreted as a sequence of economic decision rules.

For example:

`Education > 12 years?`

If yes, follow one branch.

If no, follow another branch.

This makes Decision Trees particularly attractive when interpretability is important.

## Economic Example: Unemployment Classification

**Research question:**

> Can we classify individuals according to whether they are employed or unemployed?

Possible variables include:

- Education
- Experience
- Age
- Gender
- Sector
- Region

Target:

`0 = Employed`

`1 = Unemployed`

## Analysis

Students can:

- Train a Decision Tree
- Visualize the tree
- Identify important variables
- Change tree depth
- Compare training and testing accuracy
- Examine overfitting
- Study feature importance

## Applications

Decision Trees can be used for:

- Employment prediction
- Poverty classification
- Credit approval
- Bankruptcy prediction
- Consumer classification
- Policy targeting
- Financial risk assessment
- Firm classification

## Important Concept: Overfitting

A Decision Tree can become extremely complex and memorize the training data.

Important parameters include:

- `max_depth`
- `min_samples_split`
- `min_samples_leaf`

This provides a useful introduction to model complexity and regularization.

---

# 04. Random Forest

Random Forest is an ensemble learning algorithm that combines multiple Decision Trees.

Instead of relying on one tree, the algorithm creates many trees and combines their predictions.

The basic idea is:

`Many Decision Trees → Combined Prediction`

Random Forest generally provides more stable predictions than a single Decision Tree.

## Economic Example: House Price Prediction

**Research question:**

> Can we predict house prices from property and economic characteristics?

Possible variables include:

- House area
- Number of rooms
- Household income
- Distance from city centre
- Location
- Age of property

Target:

`House Price`

## Analysis

Students can compare:

- Linear Regression
- Decision Tree
- Random Forest

This allows students to understand how different models handle nonlinear relationships.

## Evaluation

For regression:

- MAE
- RMSE
- R²

For classification:

- Accuracy
- Precision
- Recall
- F1
- ROC-AUC

## Applications

Random Forest is useful for:

- Real estate valuation
- Credit risk
- Bankruptcy prediction
- Financial risk
- Poverty prediction
- Consumer behaviour
- Employment prediction
- Economic classification

---

# 05. K-Means Clustering

K-Means is an unsupervised Machine Learning algorithm.

Unlike supervised models, there is no predefined target variable.

Instead, the objective is to discover groups or clusters within the data.

## Economic Example: Consumer Segmentation

**Research question:**

> Can households be grouped according to their economic behaviour?

Possible variables:

- Annual income
- Annual consumption
- Annual savings

The algorithm may discover groups such as:

- Low-income households
- Middle-income households
- High-income households

However, the researcher must interpret the economic characteristics of each cluster rather than assuming the labels beforehand.

## Analysis

Students can:

1. Explore the data
2. Standardize variables
3. Select the number of clusters
4. Train K-Means
5. Visualize clusters
6. Use the Elbow Method
7. Calculate Silhouette Score
8. Interpret the economic characteristics of clusters

## Applications

K-Means can be used for:

- Consumer segmentation
- Household classification
- Poverty profiling
- Regional development analysis
- Country classification
- Banking customer segmentation
- Investor segmentation
- Income-group analysis

---

# 06. Support Vector Machine

Support Vector Machine, or SVM, is a supervised Machine Learning algorithm that attempts to find an optimal decision boundary between classes.

It can also model nonlinear relationships using kernel functions.

## Economic Example: Financial Distress Prediction

**Research question:**

> Can firms be classified as financially healthy or financially distressed?

Possible variables include:

- Debt-to-equity ratio
- Profitability
- Liquidity
- Interest coverage
- Cash flow
- Asset growth

Target:

`0 = Financially Healthy`

`1 = Financially Distressed`

## Applications

SVM can be applied to:

- Bankruptcy prediction
- Credit risk
- Financial fraud
- Firm classification
- Market regime classification
- Employment classification
- Poverty classification

## Advantages

- Effective in high-dimensional datasets
- Can model nonlinear decision boundaries
- Useful for classification problems

## Limitations

- Requires careful feature scaling
- Kernel selection can be difficult
- Less interpretable than simple regression
- Computationally expensive for very large datasets

---

# 07. Naive Bayes

Naive Bayes is a probabilistic classification algorithm based on Bayes' theorem.

It assumes conditional independence between features.

Although this assumption is often unrealistic, Naive Bayes can perform surprisingly well in text classification problems.

## Economic Example: Economic News Classification

**Research question:**

> Can economic news articles be classified according to their sentiment?

Possible categories:

- Positive
- Negative
- Neutral

Data can come from:

- Newspapers
- Financial reports
- Central bank statements
- Government announcements
- Company reports

## Why This Matters for Economics

Modern economic research increasingly uses textual information.

Economists can analyse:

- Economic sentiment
- Inflation expectations
- Central bank communication
- Government policy
- Financial news
- Corporate announcements

## Applications

Naive Bayes can be used for:

- Economic sentiment analysis
- Financial news classification
- Policy-document classification
- Central bank communication
- Consumer sentiment
- Company sentiment
- Text-based financial analysis

It provides a simple introduction to:

**Natural Language Processing + Economics**

---

# 08. Principal Component Analysis

Principal Component Analysis, or PCA, is an unsupervised dimensionality-reduction technique.

It is useful when a dataset contains many correlated variables.

Instead of using every variable separately, PCA creates a smaller number of components that capture much of the information contained in the original variables.

## Economic Example: Economic Activity Index

Suppose we have:

- GDP growth
- Industrial production
- Employment
- Unemployment
- Consumption
- Investment
- Exports
- Imports
- Money supply

These variables may be strongly correlated.

PCA can combine them into a smaller number of components representing broader economic conditions.

For example:

`Economic Indicators → PCA → Economic Activity Component`

## Applications

PCA is useful for:

### Macroeconomics

- Economic activity indices
- Business-cycle indicators
- Financial conditions indices

### Finance

- Risk factors
- Portfolio analysis
- Factor extraction

### Development Economics

- Development indices
- Socioeconomic indicators

### International Economics

- Country development dimensions
- Competitiveness indicators

## Why PCA Matters

PCA is particularly useful when:

- There are many variables
- Variables are highly correlated
- Multicollinearity is a concern
- Dimensionality needs to be reduced
- Visualization of high-dimensional data is required

---

# 09. XGBoost

XGBoost stands for:

**Extreme Gradient Boosting**

It is one of the most powerful and widely used Machine Learning algorithms for structured or tabular datasets.

XGBoost belongs to the family of gradient-boosting algorithms.

Instead of building independent trees, XGBoost builds trees sequentially, with each new tree attempting to correct errors from previous trees.

The basic idea is:

`Tree 1 → Errors → Tree 2 → Errors → Tree 3 → ... → Final Prediction`

## Why XGBoost is Important for Economics

A large proportion of economic data is structured as tables:

- Individual × Variables
- Firm × Variables
- Country × Variables
- Household × Variables
- Bank × Variables
- Year × Variables

XGBoost is particularly powerful for these types of datasets.

---

## Economic Example: Credit Risk

**Research question:**

> Can we predict whether a borrower will default on a loan?

Possible features:

- Income
- Credit score
- Debt
- Loan amount
- Employment
- Age
- Previous defaults
- Interest rate
- Loan duration

Target:

`Default = 0 / 1`

XGBoost can capture nonlinear relationships and interactions between these variables.

---

## Deep Applications of XGBoost in Economics

### Banking

- Credit scoring
- Loan default prediction
- Fraud detection
- Customer risk
- Mortgage risk

### Macroeconomics

- GDP nowcasting
- Inflation prediction
- Recession prediction
- Economic activity prediction

### Labour Economics

- Employment prediction
- Wage prediction
- Worker attrition
- Skill-demand prediction

### Development Economics

- Poverty prediction
- Household vulnerability
- Financial inclusion
- Food-security prediction

### International Economics

- Export prediction
- Import prediction
- Trade-flow prediction
- Trade-partner classification

### Environmental Economics

- Carbon-emission prediction
- Energy demand
- Pollution prediction
- Climate-risk prediction

### Finance

- Credit risk
- Asset-return prediction
- Volatility prediction
- Market-regime classification

---

## Important XGBoost Parameters

Students should understand:

- `n_estimators`
- `max_depth`
- `learning_rate`
- `subsample`
- `colsample_bytree`
- `min_child_weight`
- `gamma`
- `reg_alpha`
- `reg_lambda`

Hyperparameter optimization can be performed using:

- Grid Search
- Random Search
- Cross Validation
- Bayesian Optimization

---

## XGBoost vs Random Forest

Random Forest builds many trees independently and combines them.

XGBoost builds trees sequentially and attempts to correct previous errors.

| Feature | Random Forest | XGBoost |
|---|---|---|
| Strategy | Bagging | Boosting |
| Trees | Independent | Sequential |
| Main focus | Reduce variance | Reduce prediction error |
| Nonlinear relationships | Excellent | Excellent |
| Feature interactions | Yes | Yes |
| Tabular data | Excellent | Excellent |
| Tuning | Moderate | Important |
| Interpretability | Moderate | Moderate |

---

# 10. Neural Networks

Neural Networks are flexible Machine Learning models capable of learning highly nonlinear relationships.

A basic neural network consists of:

`Input Layer → Hidden Layer(s) → Output Layer`

Each layer transforms information before passing it to the next layer.

## Economic Example: GDP Forecasting

**Research question:**

> Can macroeconomic indicators be used to predict future GDP growth?

Possible features:

- Inflation
- Interest rate
- Unemployment
- Industrial production
- Exports
- Imports
- Investment
- Money supply
- Government expenditure

Target:

`Future GDP Growth`

## Applications

### Macroeconomics

- GDP forecasting
- Inflation forecasting
- Recession prediction
- Economic nowcasting

### Finance

- Asset-price prediction
- Volatility prediction
- Credit risk
- Fraud detection

### Labour Economics

- Wage prediction
- Employment forecasting
- Skill-demand prediction

### Environmental Economics

- Energy demand
- Carbon emissions
- Climate-risk prediction

### Development Economics

- Poverty prediction
- Regional development
- Satellite-based economic activity

---

# Beyond the Ten Models

Once students understand these ten models, they can progress to more advanced techniques.

## Regularization

- Ridge Regression
- Lasso Regression
- Elastic Net

## Advanced Boosting

- LightGBM
- CatBoost
- AdaBoost

## Deep Learning

- Deep Neural Networks
- CNN
- RNN
- LSTM
- Transformers

## Advanced Econometric Machine Learning

- Causal Forests
- Double Machine Learning
- Debiased Machine Learning
- Treatment Effect Estimation
- Heterogeneous Treatment Effects

---

# Machine Learning and Econometrics

Machine Learning and Econometrics should be viewed as complementary disciplines.

| Econometrics | Machine Learning |
|---|---|
| Causal inference | Prediction |
| Hypothesis testing | Predictive performance |
| Parameter estimation | Generalization |
| Economic theory | Pattern recognition |
| Identification | Feature engineering |
| Statistical inference | Cross-validation |
| Policy evaluation | Forecasting |

Modern research can combine both approaches.

For example:

`Economic Theory + Econometrics + Machine Learning + Domain Knowledge`

can provide a much stronger research framework than using any one method alone.

---

# Prediction ≠ Causality

This is one of the most important lessons in the repository.

Suppose a model finds:

`Education → Higher Predicted Wage`

This does not automatically establish:

`Education → Higher Wage`

There may be omitted variables such as:

- Ability
- Family background
- Location
- Occupation
- Social networks
- Industry
- Selection effects

Therefore:

> **Machine Learning can identify predictive relationships, but predictive importance alone does not establish causality.**

Students interested in causal questions should study:

- Randomized experiments
- Instrumental Variables
- Difference-in-Differences
- Regression Discontinuity
- Matching
- Synthetic Control
- Causal Machine Learning

---

# Evaluation Metrics

## Regression

Common metrics:

- MAE
- MSE
- RMSE
- R²
- MAPE

### MAE

Measures the average absolute prediction error.

### RMSE

Penalizes large prediction errors more heavily.

### R²

Measures the proportion of variation explained by a regression model in the standard regression setting.

---

## Classification

Common metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC
- PR-AUC
- Confusion Matrix

Accuracy can be misleading when the dataset is imbalanced.

For example:

`95% No Default`

`5% Default`

A model predicting "No Default" for everyone achieves 95% accuracy but completely fails to identify defaulting borrowers.

---

# Feature Engineering for Economic Data

Machine Learning performance depends heavily on the quality of the features.

Economic knowledge can be used to construct meaningful variables.

## Growth Rates

Examples:

- GDP growth
- Income growth
- Export growth
- Productivity growth

## Ratios

Examples:

- Debt-to-GDP
- Debt-to-income
- Exports-to-GDP
- Tax-to-GDP

## Log Transformations

Examples:

- Log GDP
- Log income
- Log trade
- Log population

## Lag Variables

Examples:

- GDP(t-1)
- Inflation(t-1)
- Interest rate(t-1)

## Moving Averages

Examples:

- 3-month average
- 6-month average
- 12-month average

## Interaction Variables

Examples:

- Education × Experience
- Income × Age
- Interest Rate × Inflation

Economic theory should guide feature engineering whenever possible.

---

# Time-Series Economic Data

Economic data often contains a time dimension.

Examples:

`1990 → 1991 → 1992 → ... → 2025`

Randomly splitting observations can cause future information to enter the training dataset.

This is known as **data leakage**.

For forecasting, use time-aware validation.

Example:

`Training: 1990–2018`

`Testing: 2019–2025`

Traditional time-series models remain highly relevant:

- ARIMA
- SARIMA
- VAR
- VECM
- State Space Models

Machine Learning models such as Random Forest, XGBoost, and Neural Networks can complement these approaches.

---

# Common Problems in Economic Machine Learning

## Overfitting

The model performs extremely well on training data but poorly on unseen data.

## Underfitting

The model is too simple to capture the underlying pattern.

## Data Leakage

Information from the test period accidentally enters the training process.

## Multicollinearity

Features are strongly correlated with one another.

## Class Imbalance

Some economic events are relatively rare:

- Bankruptcy
- Default
- Fraud
- Recession

## Missing Data

Economic datasets frequently contain missing observations because of:

- Different reporting systems
- Survey non-response
- Structural changes
- Data collection problems

## Non-Stationarity

Economic time series may change their statistical properties over time.

## Structural Breaks

Economic relationships can change because of:

- Financial crises
- Policy changes
- Pandemics
- Wars
- Technological changes
- Institutional reforms

---

# Recommended Python Libraries

The main Python ecosystem used in this repository includes:

```python
import numpy as np
import pandas as pd

import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.model_selection import train_test_split
from sklearn.model_selection import cross_val_score

from sklearn.linear_model import LinearRegression
from sklearn.linear_model import LogisticRegression

from sklearn.tree import DecisionTreeClassifier
from sklearn.ensemble import RandomForestClassifier
from sklearn.ensemble import RandomForestRegressor

from sklearn.cluster import KMeans

from sklearn.svm import SVC

from sklearn.naive_bayes import GaussianNB

from sklearn.decomposition import PCA

from xgboost import XGBClassifier
from xgboost import XGBRegressor



