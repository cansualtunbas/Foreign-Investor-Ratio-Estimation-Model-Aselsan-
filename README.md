Foreign Investor Ratio Estimation Model-Aselsan

The aim of this study is to estimate the foreign investor ratio in Aselsan stocks between 2010-2011. In the study, the independent variables selected were the stock's opening, closing, highest and lowest price information, four technical indicators, a dummy variable indicating whether there is a holiday, news headlines obtained from two separate websites (https://www.ft.com/turkish-economy,https://tradingeconomics.com) and variables created using 3-day lagged values ​​of the variables.There are 56 variables and 732 observations in total.

In the study, firstly tf-idf was created for the selected news headlines. Then, the significance level of the words for the dependent variable was determined, thus important words to be used in the analysis were selected. Selected words: low,high,manufacturing,growth,morale.

If this word is included in the news headline on the relevant date, it is tagged with 1, if not, it is tagged with 0.

Then, the textual data set was combined with the main data set and made ready for analysis.

First, data preprocessing steps were applied to the data set. Then, correlation analysis was performed to investigate the correlation caused by variables with high correlation.

It has been observed that there is a high correlation between stock-related variables. This is because the stock price is calculated by adding and subtracting a certain percentage from the previous day's closing price and the price of a stock moves between the highest and lowest prices.
It has been observed that there is a high correlation between some technical indicators. This is because some technical indicators are derived from each other.
The first model used to estimate the foreign investment rate is the Linear Model. However, two separate estimates were made for this model. The first was made by including highly correlated variables, and the second was made by removing some correlated variables.

Then the data set was changed and the dependent variable was made categorical. First data set: Did the foreign investment rate increase compared to the previous day? (if yes, 1, otherwise 0), second data set: Did the foreign investment rate decrease compared to the previous day? (if yes, 1, otherwise 0).

Variables with high correlation were left in the "decrease" dataset and predictions were made by performing hyperparameter optimization on multiple machine learning models. According to the prediction results, Ensemble Learning was performed by combining the powers of successful models.

Variables with high correlation were removed from the “decrease” dataset and predictions were made by performing hyperparameter optimization on multiple machine learning models. According to the prediction results, Ensemble Learning was performed by combining the powers of successful models.

Variables with high correlation were left in the "increase" dataset and predictions were made by performing hyperparameter optimization on multiple machine learning models. According to the prediction results, Ensemble Learning was performed by combining the powers of successful models.

Variables with high correlation were removed from the “increase” dataset and predictions were made by performing hyperparameter optimization on multiple machine learning models. According to the prediction results, Ensemble Learning was performed by combining the powers of successful models.
