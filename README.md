# LSTM_Portfolio_Optimization_Results

- Designed and implemented a custom deep learning model using LSTM architecture with Attention mechanism, Dropout layer and Fully Connected Layer for portfolio optimization, taking asset returns and trading signals as inputs

- Implemented optional shorting capability allowing the model to take negative positions when market conditions warrant

- Engineered a custom loss function incorporating financial objectives (Sharpe Ratio, Sortino Ratio, CVaR, utility-based functions) to directly align model training with investment performance

- Developed a backtesting framework supporting both expanding and sliding window validation schemes for robust performance evaluation

- Applied asset selection, hyperparameter tuning, and validation across custom datasets and multiple temporal resolutions—including monthly, daily, and intraday data—to identify asset combinations with strong complementary dynamics, enabling more effective portfolio construction and validation, beating SP500 and other assets on returns and Sharpe ratio over 15 years period



Assets : SPY, Short-term bonds (SHY), Medium-term bonds (IEF), Long-term bonds (TLT), Corporate bonds (LQD), Gold (GLD), Real estate (VNQ), Oil (USO), Emerging markets (VWO), Euro stoxx 50 (FEZ)

Indicators : VIX, T-Bill yield, (MA21 - MA50) / MA50, RSI, 50-day historical Sharpe


###TABLE OF ALL RESULTS


Loss function                  | Annual return | Annual std dev | Sharpe  | Sortino | Max daily DD | Max DD | Image
-------------------------------|---------------|----------------|---------|---------|---------------|--------|-------
Sharpe                         | 0.0768        | 0.0729         | 1.1612  | 1.6991  | 0.0671        | 0.2292 | 
Sharpe                         | 0.0742        | 0.0682         | 1.1857  | 1.7211  | 0.0665        | 0.2262 | Sharpe
EWR                            | 0.1782        | 0.2707         | 0.7729  | 1.1244  | 0.1663        | 0.4661 | EWR
Sortino                        | 0.1222        | 0.1926         | 0.8359  | 1.1378  | 0.1254        | 0.3679 | 
Simple utility λ=-5            | 0.1043        | 0.3301         | 0.3297  | 0.4760  | 0.2131        | 0.6380 | 
Simple utility λ=0.5           | 0.1499        | 0.2264         | 0.7570  | 1.1150  | 0.1210        | 0.3922 | Utility_0.5
Simple utility λ=1             | 0.0922        | 0.1491         | 0.8070  | 1.1848  | 0.0953        | 0.2857 | Utility_1
Simple utility λ=5             | 0.0111        | 0.0122         | 0.2532  | 0.4506  | 0.0120        | 0.0517 | Utility_5
Returns                        | 0.1406        | 0.2642         | 0.6017  | 0.8935  | 0.1524        | 0.4185 | img515


Notes:
- Annual return: Annualized return
- Annual std dev: Annualized standard deviation
- Sharpe: Sharpe ratio
- Sortino: Sortino ratio
- Max daily DD: Maximum daily drawdown
- Max DD: Maximum drawdown
- λ (lambda): Risk aversion parameter
- EWR: Exponentially weighted return function (state-of-the-art function that I created)

