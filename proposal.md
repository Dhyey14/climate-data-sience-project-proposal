Summary:
In this project, we estimate the risk premium associated with firm-level climate change exposure among S&P 500 companies from 2005 to 2020. This exposure is measured 
based on the attention given by market participants to climate-related risks and opportunities during earnings calls. While the unconditional risk premium derived from
realized returns is generally insignificant, there are notable periods of positive risk premium, particularly before the 2008 financial crisis and in the years 
following it. The peak risk premium, ranging from 0.5% to 1% per annum, is observed between 2011 and 2014 when using forward-looking expected return proxies. However, 
since 2015, the risk premium has decreased, especially for stocks with high climate exposure, which tend to present higher opportunities and lower crash risks. The 
time-series analysis shows that the risk premium is negatively associated with green innovation, Big Three (Vanguard, BlackRock, and State Street) holdings, and ESG 
fund flows, while it is positively correlated with climate change adaptation programs. This project aims to model and analyze these dynamics, providing insights into 
how climate change exposure influences asset pricing over time.

Data collection:
Data needs to collected very carefully and merged in such a way that it aligns with the project requirements. For this research paper, climate data, stock prices for 
S&P 500 companies, climate risk scores, economic data of companies which affects their risk premium or any other data which is crucial to analyse the impact. 

Data cleaning and preprocessing:
First, missing values needs to be addressed by either removing those entries or using imputation techniques. Then, outliers need to be handled based on how big impact 
they could have on the models. The dataset needs to be scaled because of the various types of units of the features. Feature engineering can also be performed to 
introduce new features that can increase the performance of the models.

Analysis:
Local Interpretable Model-agnostic Explanation (LIME) and SHapleyAdditive exPlanation (SHAP) are two feature importance techniques which can be used to understand the 
relationship among the features. LIME shows the explanation for evey prediction of the models whereas SHAP compares the weight of each features based on the model used.

Model selection:
For this project, predicitve models such as logistic regression, and time series models such as a combination of LSTM-GARCH(Long Short Term Memory Network - Generalized
Autoregressive Conditional Heteroskedasticity) model can be employed to predict the risk premium, the prices of the stocks, and to forecast the stock prices. For the 
hybrid LSTM-GARCH models, LSTM models the nonlinear relationships in the data, and GARCH models the volatility. This can provide a more comprehensive understanding of
the risk premium dynamics. Logistic regression helps understand the probability that a firm falls into a high-risk premium category based on its climate exposure and 
other factors. This is particularly relevant when examining how different economic factors and investor preferences influence the distribution of risk premiums.

Model testing:
K-fold Cross Validation can be used for model validation. To improve the performance of the models, hyperparameter tuning can be utilised. Performance metrics are 
tested and compared to evaluate the models such as RMSE (Root Mean Squared Error) to assess the accuracy of predictions, and R-squared to determine the proportion of 
variance explained by the model.

Documentation:
The entire process is documented by preparing a report with the objectives, methodology, data and model preparations, model comparisons, results and analysis, 
conclusion, and any future work that can be done to enhance the project. Data visualization tools can be used to create visualizations and present the key findings to 
the stakeholders.
