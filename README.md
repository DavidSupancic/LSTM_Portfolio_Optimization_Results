# LSTM_Portfolio_Optimization_Results

Each image pair (e.g., img1) shows the results of my code applied to different asset combinations using a specific loss function.

Example:
img1 - Assets : Gold, SPY...
	 - Signals : VIX, MA50, RSI...
     - Loss function : Sharpe ratio
	 

The naming and ordering of image pairs correspond to different runs or experiments, each potentially using distinct asset sets and optimization criteria.


img1 - SPY, Short-term bonds, Medium-term bonds, Long-term bonds, Corporate bonds, Gold, 	   Real estate, Oil, Emerging markets, Euro stoxx 50
	 - VIX, (MA21 - MA50) / MA50, 50 days historical Sharpe, 21-days Relative Strength Index (RSI)
	 - Sharpe ratio
	 
img2 - SPY, Gold, Real estate, Long-term bonds
	 - VIX
     - Sharpe ratio
	 
img3 - XLK, XLF, XLE, XLV, XLI, XLY, XLP, XLU, XLB, Gold, Real estate, Long-term bonds
	 - VIX
	 - Sharpe ratio

img4 - SPY, Short-term bonds, Medium-term bonds, Long-term bonds, Corporate bonds, Gold, 	   Real estate, Oil, Emerging markets, Euro stoxx 50
	 - VIX, (MA21 - MA50) / MA50, 50 days historical Sharpe, 21-days Relative Strength Index (RSI)
	 - Utility function (risk aversion=1)
	 
img5 - SPY, Short-term bonds, Medium-term bonds, Long-term bonds, Corporate bonds, Gold, 	   Real estate, Oil, Emerging markets, Euro stoxx 50
	 - VIX, (MA21 - MA50) / MA50, 50 days historical Sharpe, 21-days Relative Strength Index (RSI)
	 - Utility function (risk aversion=5)