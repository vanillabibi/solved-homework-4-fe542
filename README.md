Download Link: https://assignmentchef.com/product/solved-homework-4-fe542
<br>
<strong>Problem 1 </strong>(50pt)

Suppose that the monthly log returns, in percentages, of a stock follow the following Markov switching model:

if <em>s<sub>t </sub></em>= 1   if <em>s<sub>t </sub></em>= 2

where the transition probability are

P(<em>s<sub>t </sub></em>= 2 | <em>s<sub>t</sub></em><sub>−1 </sub>= 1) = 0<em>.</em>2<em>,                   </em>P(<em>s<sub>t </sub></em>= 1 | <em>s<sub>t</sub></em><sub>−1 </sub>= 2) = 0<em>.</em>1<em>.</em>

Suppose that     = 50, and <em>s</em><sub>100 </sub>= 2 with probability 1.

<ul>

 <li>What is the 1-step-ahead volatility forecast at the forecast origin <em>t </em>= 100?</li>

 <li>If the probability of <em>s</em><sub>100 </sub>= 2 is reduced to 0<em>.</em>75, what is the 1-step-ahead volatility forecast origin <em>t </em>= 100.</li>

</ul>

Bonus In R create a report in pdf format using RMarkdown (or, if you choose to use Python instead, create a Jupyter notebook) to implement this Markov switching model and compare the forecasts you computed to simulated results.

<strong>Problem 2 </strong>(50pt)

In R create a report in pdf format using RMarkdown (or, if you choose to use Python instead, create a Jupyter notebook) to:

<ul>

 <li>Download daily price data for January 1, 2000 through December 31, 2020 of Amazon stock from Yahoo Finance. Compute the <em>weekly </em>logarithmic returns <em>r<sub>t</sub></em>. You may use the quantmod package in R for this purpose.</li>

 <li>Using lagged returns <em>r<sub>t</sub></em><sub>−1</sub><em>,r<sub>t</sub></em><sub>−2</sub><em>,r<sub>t</sub></em><sub>−3 </sub>as input, build a 3-2-1 feed-forward neural network to forecast 1-step-ahead returns. Use data up to December 31, 2018 as the training data set and the remainder as the testing data. Calculate the mean squared error on the test data.</li>

</ul>

1

<ul>

 <li>Using lagged returns <em>r<sub>t</sub></em><sub>−1</sub><em>,r<sub>t</sub></em><sub>−2</sub><em>,r<sub>t</sub></em><sub>−3 </sub>and their signs (directions) to build a 6-5-1 feedforward neural network to forecast the 1-step-ahead <em>direction </em>of Microsoft stock price movement (with 1 denoting upward movement and 0 downward movement). Use data up to December 31, 2018 as the training data set and the remainder as the testing data. Calculate the mean squared error on the test data.</li>

</ul>

<em>Note</em>: Let rtn denote a time series in R. To create a direction variable for rtn, use the command drtn = ifelse(rtn &gt; 0, 1, 0)

2