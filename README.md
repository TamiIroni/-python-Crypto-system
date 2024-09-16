Bitcoin Price Prediction Model
Introduction
The cryptocurrency market is known for its high volatility, with Bitcoin’s volatility reaching 45.31% over the past year. Given this, Bitcoin is highly attractive for day traders who typically rely on technical indicators like the Relative Strength Index (RSI) and moving averages. However, these indicators only focus on price behavior and overlook broader economic factors. Our machine learning model aims to predict the next day's closing price by considering a range of economic indicators beyond just technical metrics, providing deeper insights for day trading.

Model Overview
Our model uses a Random Forest Regressor to predict the next-day closing price of Bitcoin. It integrates various parameters reflecting the global economic landscape and their impact on Bitcoin’s price, including:

Bitcoin Price: Last price of the day, used to predict the next day’s closing price.
Trading Volume: Indicates market activity and liquidity, influencing price movements.
S&P 500: Represents risk appetite in the broader market, correlating with high-risk assets like Bitcoin.
DXY Index: Measures the value of the U.S. dollar against major currencies; influences Bitcoin prices due to changing investor preferences.
Gold Price: Acts as a hedge against inflation, similar to Bitcoin; retained to monitor potential shifts in Bitcoin’s behavior.
Ethereum Price & Volume: Ethereum’s correlation with Bitcoin provides additional insights into market trends.
Oil Price: Reflects global economic conditions that indirectly impact Bitcoin prices.
Days Since Last Halving: Tracks Bitcoin's supply inflation, influencing long-term price trends.
Correlation Analysis & Feature Selection
Our analysis found strong correlations between Bitcoin’s price and factors like the S&P 500, Gold, and Ethereum prices. Weaker correlations were observed with the DXY Index, Ethereum volume, and days since the last halving. Despite these weaker correlations, we chose to retain these variables due to their potential business value and future relevance.

Key Observations:
Strongest correlations: Bitcoin price, S&P 500, Gold, Ethereum price.
Moderate correlations: Trading volume, Oil price.
Weakest correlations: DXY, Ethereum volume, days since last halving.
In tests excluding weakly correlated parameters, the model’s performance, measured by Mean Squared Error (MSE), remained stable, confirming that these parameters don’t currently impact model accuracy. However, they were retained to monitor future shifts in Bitcoin behavior.

Algorithm Performance
The model achieved an R-squared value of 99%, indicating a high fit with the actual data. The MSE was 1,249,049, which, considering Bitcoin’s volatility, is acceptable.

Recommendations
While some features don’t currently influence the model’s predictions, we suggest re-evaluating the model in 1-2 years. If Bitcoin’s behavior evolves to align more closely with these variables, the model may need adjustments.

