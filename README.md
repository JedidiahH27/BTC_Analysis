# Analysis of Bitcoin Price vs. Fear/Greed Index and S&P 500
This analysis investigates the relationship between Bitcoin (BTC) price movements, the Fear and Greed Index, and the S&P 500 Index. The analysis includes:

Descriptive statistics and correlation analysis.

Time series visualization of BTC, Fear and Greed Index, and S&P 500 prices.

Analysis of BTC daily returns, including distribution fitting and statistical tests.

Linear regression modeling to predict BTC daily returns based on the Fear and Greed Index and S&P 500 Index changes.

## Key Findings
### Descriptive Statistics and Correlations:

Provides summary statistics for BTC price, Fear and Greed Index, and S&P 500 price.

Calculates the correlation matrix to show relationships between these variables.  The code shows moderate correlation between BTC and S&P500.

### Time Series Analysis:

Visualizes the trends of BTC price, Fear and Greed Index, and S&P 500 price over time.

Calculates and plots the 30-day moving averages for BTC and S&P 500 prices.

### BTC Daily Return Analysis:

Calculates and describes the descriptive statistics of BTC daily returns.

Plots a histogram of BTC daily returns and fits a Gaussian distribution.

Analyzes BTC daily returns conditional on the previous day's return (positive and negative).

Analyzes BTC daily returns conditional on the previous two days' returns.

Performs t-tests, Levene's test, and Shapiro-Wilk tests to compare the distributions of BTC daily returns under different conditions.

Fits various distributions (Normal, Student's t, Exponential) to the BTC daily return data and performs Kolmogorov-Smirnov tests.

Compares the distributions of BTC daily returns following positive and negative two-day returns using the Kolmogorov-Smirnov test and Mann-Whitney U test.  The code finds statistically significant differences.

### Fear and Greed Index Analysis

Classifies the Fear and Greed Index into categories (Extreme Fear, Fear, Neutral, Greedy, Extreme Greed).

Analyzes the distribution of BTC daily returns for each category and performs Kolmogorov-Smirnov tests.

Compares the distributions of BTC daily returns between different Fear and Greed Index categories using the Kolmogorov-Smirnov test.  The code finds statistically significant differences in BTC returns based on the Fear and Greed Index.

### Relationship with S&P 500:

Calculates the correlation between BTC daily returns and lagged S&P 500 Index changes.

Visualizes the relationship between BTC daily returns and S&P 500 Index changes using scatter plots.

Calculates the correlation between BTC daily returns and the Fear and Greed Index.

Visualizes the relationship between BTC daily returns and the Fear and Greed Index using a scatter plot.

### Linear Regression Modeling:

Builds a simple linear regression model to predict BTC daily returns based on the lagged Fear and Greed Index.

Splits the data into training and testing sets, standardizes the data, and trains the model using PyTorch.

Evaluates the model's performance and visualizes the results.

Builds a multiple linear regression model to predict BTC daily returns based on both the lagged Fear and Greed Index and lagged S&P 500 Index changes.

Evaluates the model and visualizes the results in a 3D scatter plot and a residual plot.
