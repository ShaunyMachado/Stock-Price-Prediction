# Stock-Price-Prediction
Stock Price prediction using Machine Learning Algorithms

1. Introduction


A stock exchange market depicts savings and investments that are advantageous to increase the effectiveness of national economic. Stock market prediction is the act of trying to determine the future value of a company stock or other financial instrument traded on a financial exchange.

Stock market forecasting contains uncovering the market trends, planning investment tactics, identifying the best time to purchase the stocks and which stocks to purchase. A stock exchange or equity business sector is a non-direct, non-parametric framework that is difficult to model with any sensible exactness. It is the mix of speculators who need to purchase or offer or hold a share at a specific time. Prediction will continue to be an exciting locale of research, making scientists in the analytics field always desiring to enhance the existing forecasting models.

Stock trend forecasting is considered as one of the most difficult tasks to achieve in money related gauging because of the difficulty in the multifaceted world of stock market. Many of the investors in the stock market are finding a technique that could guarantee easy profiting by forecasting the stock trends and minimize the risk of investing. This motivates the researchers in the domain field to delve and develop new forecasting models.

Every investor is interested in predicting the future stock prices, whether the investor may be a long-term investor or a day-trader. This possesses a major challenge to design and develop an effective and efficient predictive model that assists the investors to take appropriate decisions. The motivation is that companies and individuals are empowered to make investment decisions to develop viable system about their future endeavors. The successful prediction of a stock's future price will maximize investor’s gains.


1.1	Scope

The chief goal of this project is to add to the academic understanding of stock market prediction. The hope is that with a greater understanding of how the market moves, investors will be better equipped to prevent another financial crisis. This project will focus exclusively on predicting the daily trend (price movement) of individual stocks. The project will make no attempt to deciding how much money to allocate to each prediction. More so, the project will analyze the accuracies of these predictions. The algorithms presented will operate on the order of days and will attempt to be truly predictive of the market.






2. General Description


2.1 Pre-existing work

•	To forecast stock price trend, the authors Tao Xing, Yuan Sun, have introduced a method based on Hidden Markov Model, which is a kind of Markov Chain and is used for the pattern recognition technique.

•	The authors Vishwanath R Ha, Leena Sa have proposed a system called APST, which performs the preprocessing of verifiable stock time arrangement information to produce the grouping of approximated values by utilizing multi-scale segment mean methodology.

•	The author Li Zhe have used the method of technical analysis in which trading rules were established based on the ancient data of stock trading price and volume.

•	The author, Banerjee D, tried to develop an appropriate model that helps to forecast the unseen values of the Indian stock market, based on the information collected on the monthly closing stock indices.



2.3 Specifications of the project

In our project, the datasets we have taken for analyzing are of Apple Inc. (1980 – 2017) and Microsoft Corporation (1986 – 2017) from Equity-NASDAQ using Yahoo finance API. The data has been decomposed into two data sets, 75% training dataset and 25% testing dataset. We applied the following supervised learning theories to the training dataset:


•	SVM (Support Vector Machine)
•	Recurrent Neural Network

Then comparison of the result was done with the testing dataset (i.e. 25% of the dataset). Based on the outcomes, the accuracy of both algorithms was compared. For visualization of the accuracies of both the algorithms we have used line graphs.



3. Specific Requirements

3.1 Operating Environment

•	Ubuntu/Linux Operating Environment

3.2 Coding language used
•	   Python

3.3 Packages Used
•	sci-kit learn
•	numpy
•	matplotlib
•	pybrain
•	pandas
•	nvd3
•	ipython

3.4 Data Collection
•	Apple Inc. (AAPL) NasdaqGS - NasdaqGS Real Time Price. Currency in USD dataset from https://in.finance.yahoo.com/quote/AAPL?p=AAPL for 7 and 37 years
•	Microsoft Corporation (MSFT) NasdaqGS - NasdaqGS Real Time Price. Currency in USD dataset from https://in.finance.yahoo.com/quote/MSFT/history?p=MSFT for 7 and 31 years


4. Feature Selection

In the downloaded dataset 5 features were present for the daily stock price, namely:
•	Opening price
•	Closing price
•	High price
•	Low price
•	Volume


We have increased the number of features to 11 from the 5 already present for better training of our model, namely:

•	Open change percentage list
•	Close change percentage list
•	High change percentage list
•	Low change percentage list
•	Volume change percentage list
•	Open difference percentage list
•	Volume difference percentage list
•	Open price moving average list
•	Close price moving average list
•	High price moving average list
•	Low price moving average list

We have then made four feature lists comprising of all the 11 features to compare the accuracy for each set sets of features.

Feature list 1

•	Open change percentage list
•	Close change percentage list
•	High change percentage list
•	Low change percentage list
•	Volume change percentage list

Feature list 2

•	Open change percentage list
•	Close change percentage list
•	High change percentage list
•	Low change percentage list
•	Volume change percentage list
•	Open difference percentage list
•	Volume difference percentage list

Feature list 3

•	Open change percentage list
•	Close change percentage list
•	High change percentage list
•	Low change percentage list
•	Volume change percentage list
•	Open price moving average
•	Close price moving average
•	High price moving average
•	Low price moving average

Feature list 4

•	Open change percentage list
•	Close change percentage list
•	High change percentage list
•	Low change percentage list
•	Volume change percentage list
•	Open difference percentage list
•	Volume difference percentage list
•	Open price moving average
•	Close price moving average
•	High price moving average
•	Low price moving average



5. Implementation

The implementation was done in Python environment with packages namely sci-kit learn, numpy, matplotlib and pybrain. The supervised learning models i.e. SVM (Support Vector Machine) and Recurrent Neural Network were executed and their accuracies obtained.
The models were implemented separately on both Apple and Microsoft stock prices of sets of 7 years’ data and 37 years’ data separately. 

6. Conclusion

This project aimed to determine whether or not it is possible to make a profitable stock trading scheme using machine learning, to compare different machine learning algorithms and their performance, investigate whether a machine learning algorithm improves when given predictions from other algorithms as features and discuss whether it is possible at all to predict the stock market. 

In this project, we applied supervised learning techniques in predicting the stock price trend of a single stock. Our finds can be summarized into three aspects:
1.	Various supervised learning models have been used for the prediction and we found that SVM model can provide the highest predicting accuracy in the range 82-88%, as we predict the stock price trend in a long-term basis. 
2.	Our feature selection analysis indicates that when use all of the 11 features, we will get the highest accuracy. That’s because the number of data points is much bigger than that of the features. 
3.	The trading strategy based on our prediction achieves very positive results by significantly outrunning the stock performance.

The conclusion can be done by answering the questions;

•	Is it possible to make profit using Machine Learning?
A critical factor is that one cannot predict with a given few features. There can be many unknown factors that can influence the stock market. But, the results yielded show that there are machine learning algorithms that are profitable in the test period, and can be optimized to a much greater extent, which likely will increase potential profit yielded. We may conclude is that it is likely that one could apply some of the presented machine learning algorithms to generate a profit if we assume that the test period is representative for other time periods and that we were trading in a near perfect market with low trading fees. Unfortunately, the experiments conducted are not extensive enough to make a final decision on whether or not it is possible to make a profit. 

•	Is Binary Prediction suitable for a stock market problem?
The results presented give reason to believe, or at least imply, that binary prediction is suitable for making a profit predicting the stock market, as the results show a possible profit. One can also say that it is suitable because every profit making stock scheme boils down to the question; should I own this stock or not. On the other hand, the two-class predictor makes exploiting other ways of trading stocks such as shorting difficult, and may therefore not provide as much profit as possible.





8.References

8.1 Bibliography

•	Machine Learning in Stock Price Trend Forecasting by Yuqing Dai, Yuning Zhang

•	Banerjee, D., "Indian stock market model", 2nd IEEE Conference, January 2014

•	Wang, Y.F., “Mining stock price using fuzzy rough set system”, Expert Systems with Applications, 2006, pp. 13-23.

8.2 Webliography

•	www.analyticsvidhya.com/blog/2016/12/introduction-to-feature-selection-method/


