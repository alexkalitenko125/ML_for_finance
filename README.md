# ML_for_finance
ML for finance forecasting (colab version).

This project was created to test the ability of neural networks to predict the stock market's behavior in stable times, when force majeure events are not significant. Neural networks take into account price periodicity, trends, and correlations between index values. Oil and gas prices, for example, only affect the ruble and the Moscow Exchange index after a certain period of time, and in turn, the ruble and Moscow Exchange affect each other. The author's models use recurrent neural networks and conventional fully connected neural networks, which were built intuitively and adjusted for maximum predictive accuracy based on subjective assessment and the basics of technical market analysis.

## Scientific interest
This project may be useful for specialists in financial analytics or the scientific field. Please refer to the repository when using it.

## Data
The data is downloading from Yahoo Finance and MOEX. 


***Important update: Yahoo Finance no longer displays data from the Russian stock market.  apimoex has been integrated.*** 

## NN architecture with LSTM
By going through and learning from the basics of technical analysis, the following scheme looks promising for a long time 

<img src="./Finance5.png"  width="500" 
     height=auto>

## Reinforcement learning 
Technical analysis is based on patterns - certain patterns of changes in stock prices and futures. There is a complex system - the *Elliot wave principle* based on Fibonacci numbers. Due to the difficulty of diagnosing patterns using these rules, some analysts win more often and others lose using their interpretations. Machine learning can train on the past, develop relevant rules and use them in games. Reinforcement learning is used for this, when the agent is in the environment, playing and learning.

The challenge is to find the optimal architecture to prevent overfitting. Dropouts can have a negative impact on the performance of an agent. A large neural network learns from the data provided, but it is necessary to manually select the appropriate learning rate and architecture. After that, it is important to test the model with different seeds to ensure accuracy. Only after these steps can the model be used in the market with confidence.

### NN stack 
PyTorch, Pandas, sklearn, yfinance, LSTM, Multi-Dimensional Regression, apimoex, reinforcement learning



