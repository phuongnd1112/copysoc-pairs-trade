# Pairs Trading Strategy (copy) 

## Description 
We looked at a potential equity trading strategies, using cointegration of two securities: 
- Antero Resources (NYSE:AR) 
- Diversified Gas and Oil (LON:DGOC) 

## Building the Model 
1. Testing for stationarity using Augmented Dickey-Fuller Test (statsmodels) ; if p_value <= 0.05 -> cointegrated. 
2. Visualised the spread (beta hedge ratio-adjusted) - notice how there was roughly a pattern from May 2020 - Sept 2020 but pattern broken afterwards 
![spread image] 
3. Generating buy/sell signal using the spread's z-scores as thresholds
