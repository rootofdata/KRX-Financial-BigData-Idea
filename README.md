# KRX-Financial-BigData-Idea

###
**Idea Title:** Development of Funds Based on ETF Analysis and Prediction of Stocks  
  (ETF 종목 분석 및 예측을 통한 펀드 개발)

**Idea Overview:**  
- Utilizing historical quarterly data of individual stocks within a specific sector (semiconductors), machine learning techniques will be applied to predict the data for the upcoming quarters. Using these predicted data, time series analysis will be employed to select stocks within the sector that meet the criteria. These selected stocks will form a portfolio, creating a unique ETF product which will be developed and launched.

**Proposal Background and Objectives:**  
- This methodology, applicable across various sectors, has been specifically applied to the semiconductor sector, which is one of South Korea's key industries and plays a significant global role. The active growth of the semiconductor industry serves as an exemplary model. Out of 134 stocks listed in the semiconductor sector on KOSPI and KOSDAQ, 46 stocks included in three large ETFs were selected. Based on this selection, a portfolio will be constructed through data analysis and prediction. The purpose of this proposal is to suggest the development of an innovative investment product, providing investors with a unique opportunity.
  
- In situations where accessing individual company data is challenging, we have chosen to utilize time-series data regularly published, such as business reports, to analyze quarterly data for each stock. This approach involves grouping observed results based on specific criteria, defining it as collective data. The use of collective data is essential because accessing individual data is often difficult. Time-series data, obtainable from various high-quality sources like statistical reports, is relatively easy to acquire.  
  
- Additionally, we opted for time-series analysis due to its historical application in predicting volatility. These models offer quantitative methods for accurate analysis and systematically explaining market phenomena based on statistical reasoning (Reference: No Tae-Hyup et al., "Forecasting Volatility of KOSPI 200 Stock Index Using Artificial Neural Networks and Financial Time Series Models"). Moreover, challenges arose in regression analysis due to intercorrelation among independent variables, leading to high RMSE in the regression analysis results, which could produce inaccurate predictions. To mitigate this issue, we employed various models for analysis, ultimately selecting the **CatBoost model** with the smallest RMSE among XGBoost, CatBoost, LgBM, and AdaBoost.  
  
- The ultimate goal of this idea is to transform it into a form that can be effectively utilized in the market, creating an investment product accessible to a wide range of investors, similar to a publicly offered fund.

**Utilized Data**

- The analysis was based on six key financial metrics (assets, liabilities, equity, revenue, operating income, net income) from semiconductor ETFs from the first quarter of 2019 to the fourth quarter of 2021. Using this data, eight indicators were derived:

- **Stability Indicators (%)**
-   Debt Ratio: (Total Debt / Total Equity) * 100  
  - Equity Ratio: (Total Equity / Total Assets) * 100  
- **Profitability Indicators (%)**
  - Net Profit Margin: (Net Income / Revenue) * 100  
  - Operating Profit Margin: (Operating Income / Revenue) * 100  
- **Activity Indicators (%)**
  - Total Asset Turnover: Revenue / Total Assets  
  - Equity Turnover: Revenue / Total Equity  
- **Growth Indicators (%)**

  - Operating Income Growth Rate: ((Current Operating Income - Previous Operating Income) / Previous Operating Income) * 100
  - Net Income Growth Rate: ((Current Net Income - Previous Net Income) / Previous Net Income) * 100
    
**Portfolio Construction Method**

The portfolio was constructed based on the weighted average scores of the selected 34 stocks. The weights for each stock were adjusted to balance stability, profitability, and growth. Regular rebalancing was performed to optimize the investment portfolio.

**Product Differentiation**

This project utilized machine learning and time-series analysis, surpassing conventional methods to provide stable and precise predictions. Additionally, the results of the machine learning models were visualized, making them easily understandable even for non-experts. Moreover, this model can be applied not only to the semiconductor sector but also to various industries.

**Market Viability and Commercialization Potential**

With the growth in the financial market, there is an increasing demand for financial products. This project is accessible to novice investors and offers verified stocks through logical and rational analysis. Thus, it can expand as an investment product that considers both stability and profitability.

**Conclusion**

This report proposes a comprehensive data analysis and prediction model utilizing machine learning and time-series analysis, driving the innovation of investment products. This balanced product, considering stability, profitability, and growth, is expected to lead the future trends in the financial market.




