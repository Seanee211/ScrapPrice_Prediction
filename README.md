# Steel Scrap Price Prediction and Analysis Platform

## Project Overview
This project focuses on predicting and analyzing the price trends of **steel scrap**, a critical resource in the steel industry.  
The goal is to assist stakeholders in securing steel scrap at lower costs, achieving carbon neutrality, and enhancing the sustainability of the steel industry.

- **Key Objectives**:  
  - Short-, mid-, and long-term price predictions (7-day, 14-day, 28-day)
  - Price trend analysis based on economic indicators and key variables
  - Development of an intuitive web-based UI/UX platform  

---

## Key Features
### 1. **Steel Scrap Price Prediction Model**
- **Applied Models**:
  - DLinear (Final Model)
  - Prophet
  - XGBoost, Random Forest, LSTM (For Benchmarking)
- **Prediction Performance**:
  - 7-day prediction: RMSE 3.81, Accuracy 84%
  - 14-day prediction: RMSE 7.99, Accuracy 73%
  - 28-day prediction: RMSE 20.13, Accuracy 62%

### 2. **Web Platform**
- **Pages**:
  - Home: Dashboard displaying average and predicted prices
  - Data Table: Steel scrap prices and associated economic indicators
  - Detailed Charts: Price trends, feature importance, and carbon emission maps
  - Support Center: FAQs, basic information, and developer details

### 3. **Automated Data Pipeline**
- **Data Collection**:
  - Web scraping using Selenium and BeautifulSoup
  - Resampling data to weekly and daily intervals
- **Automation**:
  - Weekly updates at 7 PM on Sundays with model retraining (Cron scheduled)

---

## Data and Technology Stack
### Data
- **Dependent Variables**: Average steel scrap prices (Iron Scrap, Heavy A, Light A, Turnings A, Turnings C)
- **Independent Variables**: Key economic indicators such as crude oil prices, gold prices, exchange rates, and iron ore imports
- **Data Period**: August 2006 ~ December 2023

### Technology Stack
- **Languages**: Python, JavaScript
- **Modeling Libraries**:
  - Pandas, Numpy, Scikit-Learn, Darts, Autogluon, Prophet, XGBoost
- **Web Frameworks**:
  - React, Node.js
- **Database**: PostgreSQL

---

## Benefits and Future Improvements
### Benefits
- Supports cost-effective steel scrap procurement to enhance corporate competitiveness
- Contributes to carbon neutrality and ensures sustainability in the steel industry
- Provides real-time insights into steel scrap prices and associated economic indicators

### Future Improvements
- **Automation**: Implement Cron-based scheduling for data updates and model retraining
- **Server Stability**: Transition from local to server-based infrastructure
- **Model Performance**: Improve prediction accuracy for 14-day and 28-day forecasts
