Problem Statement: 
Find publicly available data for key factors that influence US home prices *nationally*. Then, build a data science model that explains how these factors impacted home prices over the last 20 years.
Use the S&P Case-Schiller Home Price Index as a proxy for home prices: fred.stlouisfed.org/series/CSUSHPISA.

Here are the steps reflecting the actions I have completed in my project:

1. **Defined My Objectives:**
   - I began by clearly stating my project objectives and the specific questions I wanted to answer. For instance, I aimed to understand how factors like GDP, interest rates, population growth,etc. influenced home prices over the past 20 years.

2. **Data Collection:**
   - I gathered publicly available data for key factors that influence home prices. I used sources such as government databases, economic indicators, housing market reports, and academic research. I also collected data on the S&P Case-Shiller Home Price Index, accessible through the link provided (fred.stlouisfed.org/series/CSUSHPISA).

   I collected all of the data from FRED website:
   Consumer Price Index- https://fred.stlouisfed.org/series/CPIAUCSL
   Consumer Sentiment Index- https://fred.stlouisfed.org/series/CSCICP03USM665S
   Inflation Rate- https://fred.stlouisfed.org/series/T10YIEM
   Population- https://fred.stlouisfed.org/series/POPTHM
   GDP- https://fred.stlouisfed.org/series/USALORSGPNOSTSAM
   Total Share Price- https://fred.stlouisfed.org/series/SPASTT01USM661N
   Real Disposable Personal Income- https://fred.stlouisfed.org/series/DSPIC96
   Personal Income- https://fred.stlouisfed.org/series/PI
   Unemployment Rate-https://fred.stlouisfed.org/series/UNRATE

3. **Data Preprocessing:**
   - I cleaned and preprocessed the collected data. This involved handling missing values, identifying outliers, and converting data into a suitable format for analysis.

4. **Exploratory Data Analysis (EDA):**
   - I performed EDA to gain insights into my data. I visualized the data, calculated summary statistics, and identified correlations between variables. EDA helped me understand the relationships between the factors and home prices.

5. **Feature Engineering:**
   - When necessary, I created new features. For instance, I calculated annual percentage changes for economic indicators and created lag variables to account for time delays in the impact of factors on home prices.

6. **Time Series Analysis:**
   - As I was dealing with time-series data, I conducted time series analysis to understand trends, seasonality, and stationarity in my data. I used methods like autocorrelation and differencing.

7. **Model Selection:**
   - I chose appropriate machine learning models for my analysis. Time series regression models like ARIMA, STL, and machine learning algorithms like Random Forest, Gradient Boosting, and Neural Networks were considered.

8. **Model Training:**
   - I split my data into training and testing sets and then trained my chosen model(s) on the training data. I also considered cross-validation to tune hyperparameters.

9. **Model Evaluation:**
   - I evaluated the performance of my model(s) using appropriate metrics. For time series data, I commonly used metrics like MAE, MSE, or RMSE.

10. **Interpretability:**
    - I interpreted the model results to understand the impact of each factor on home prices. Feature importance analysis and partial dependence plots helped in this regard.

11. **Visualization:**
    - I created visualizations to communicate my findings effectively. Time series plots, feature importance charts, and interactive dashboards aided in presenting the results.

12. **Report and Documentation:**
    - I documented my entire process, including data sources, preprocessing steps, model details, and results. I created a clear and concise report that explained my findings and insights.

13. **Future Projections (Optional):**
    - If my model allowed, I used it to make future projections or forecasts for home prices based on the selected factors.

14. **Fine-Tuning:**
    - I refined my model and analysis based on feedback and further research.

15. **Conclusion:**
    - In the end, I summarized my findings, drew conclusions, and offered recommendations based on my analysis.