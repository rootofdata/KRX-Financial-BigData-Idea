# KRX-Financial-BigData-Idea

###
**Idea Title:** Development of Funds Based on ETF Analysis and Prediction of Stocks (ETF 종목 분석 및 예측을 통한 펀드 개발)

**Idea Overview:**  
- Utilizing historical quarterly data of individual stocks within a specific sector (semiconductors), machine learning techniques will be applied to predict the data for the upcoming quarters. Using these predicted data, time series analysis will be employed to select stocks within the sector that meet the criteria. These selected stocks will form a portfolio, creating a unique ETF product which will be developed and launched.

- 한가지 섹터(반도체)의 종목별 과거 분기 데이터를 활용하여 머신러닝 기술을 적용하여 다음 분기 데이터를 예측 및 예측된 데이터들을 기반으로 시계열 분석을 이용하여 섹터 내에서 기준에 부합하는 종목들을 선정하고, 이를 포트폴리오로 구성하여 특별한 ETF 상품을 개발하여 출시

**Proposal Background and Objectives:**  
- This methodology, applicable across various sectors, has been specifically applied to the semiconductor sector, which is one of South Korea's key industries and plays a significant global role. The active growth of the semiconductor industry serves as an exemplary model. Out of 134 stocks listed in the semiconductor sector on KOSPI and KOSDAQ, 46 stocks included in three large ETFs were selected. Based on this selection, a portfolio will be constructed through data analysis and prediction. The purpose of this proposal is to suggest the development of an innovative investment product, providing investors with a unique opportunity.
  
- In situations where accessing individual company data is challenging, we have chosen to utilize time-series data regularly published, such as business reports, to analyze quarterly data for each stock. This approach involves grouping observed results based on specific criteria, defining it as collective data. The use of collective data is essential because accessing individual data is often difficult. Time-series data, obtainable from various high-quality sources like statistical reports, is relatively easy to acquire.  
  
- Additionally, we opted for time-series analysis due to its historical application in predicting volatility. These models offer quantitative methods for accurate analysis and systematically explaining market phenomena based on statistical reasoning (Reference: No Tae-Hyup et al., "Forecasting Volatility of KOSPI 200 Stock Index Using Artificial Neural Networks and Financial Time Series Models"). Moreover, challenges arose in regression analysis due to intercorrelation among independent variables, leading to high RMSE in the regression analysis results, which could produce inaccurate predictions. To mitigate this issue, we employed various models for analysis, ultimately selecting the **CatBoost model** with the smallest RMSE among XGBoost, CatBoost, LgBM, and AdaBoost.  
  
- The ultimate goal of this idea is to transform it into a form that can be effectively utilized in the market, creating an investment product accessible to a wide range of investors, similar to a publicly offered fund.

- 여러 섹터에 적용 가능한 방법론 중 하나로, 그 중 반도체 섹터는 우리나라 주요 산업 중 하나이며, 또한 전 세계적으로 중요한 역할을 하는 반도체 산업의 활발한 성장으로 예시로 삼았음. 이를 위해 KOSPI 와 POSDAQ에 상장된 반도체 섹터에 속하는 134종목 중에서 대형 ETF 3개에 포함된 46종목을 선정함. 이를 토대로 데이터 분석과 예측을 통해 포트폴리오를 구성하여 혁신적인 투자 상품으로 투자자들에게 제공할 목적으로 이 아이디어를 제안

- 개별 회사의 데이터에 접근하기 어려운 상황에서, 사업보고서와 같은 정기적으로 발행되는 시계열 데이터를 활용하여 종목별 분기 데이터를 분석하는 방법을 선택. 이는 집합적 자료로, 관찰 결과를 특정 기준에 따라 그룹화하는 것을 의미. 집합적 자료의 사용 이유는 개별 데이터에 접근하기 어려운 경우가 많기 때문임. 시계열 데이터는 상대적으로 쉽게 얻을 수 있는 고품질 데이터로, 다양한 통계 보고서 등에서 얻을 수 있음.  
- 또한 시계열 분석을 적용한 이유는 이전부터 변동성 예측에 사용되어 왔고, 이러한 모델들은 정량적인 방법으로 정확한 분석이 가능하며 시장 현상을 통계적 논리를 기반으로 체계적으로 설명할 수 있는 장점이 있기 때문임. (참고문헌: 노태협 외 2명, "인공신경망-금융시계열 모형을 이용한 KOSPI 200 주가지수의 변동성 예측")  
또한, 독립 변수들 간의 상관성으로 인해 회귀 분석 결과의 RMSE가 높아 부정확한 예측 결과가 나올 수 있는 문제가 있음. 이러한 오차를 줄이기 위해 다양한 모델을 활용하여 분석하였으며, XGBoost, CatBoost, LgBM, AdaBoost 중에서 RMSE 값이 가장 작은** CatBoost** 모델을 선택함.  

- 이 아이디어의 최종 목표는 시장에서 성공적으로 활용 가능한 형태로 만들어 공모펀드와 같이 다수의 투자자에게 접근 가능한 투자 상품으로 만들어내는 것  

