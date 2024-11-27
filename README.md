Volitility Analysis of S&P-500 using GARCH models

data_manipulation.ipynb - Contains code which imports SnP 500 data from yahoofinance api. It then splits it into pre,during and post covid values and also plots the 7 day,30 day,6 month rolling variance on each of the 3 subsets.

finalresults(2).ipynb - Contains code which fits precovid, during covid and post covid data to ARCH(1), ARCH(2), GARCH(1/2,1/2), EGARCH(1/2,1/2), T-GARCH(1/2,1/2), GJR-GARCH(1/2,1/2).
It also contains a 7 day volitility forcast(non-rolling) with all its models.It also contains the residues of these models(actual-fitted) values over along with their residue distribution to show channging dynamics of these models.

rolling_window_fit.ipynb - Contains code used to split data in time period in 70/30 splits. Trained on the 70 split and then test using rolling window on the remaining 30%. The last fitted model summary and relevant model metrics are displayed and saved

Pre-COVID_model_performance_metrics.csv, In-COVID_model_performance_metrics.csv and Post-COVID_model_performance_metrics.csv - Contains the test errors, AIC, BIC and log-likelihood of the various models in their respective time periods.

model_evaluation_metrics.csv - csv file which contains AIC, BIC,Log_likelihood, MSE training, MSE testing(non-rolling), MAE training, MAE testing(non-rolling) for all the fitted models.
