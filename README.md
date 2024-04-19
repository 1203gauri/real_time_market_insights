
![image](https://github.com/1203gauri/real_time_market_insights/assets/147191401/711ea98c-1f30-493d-9444-aedddd86c69d)

Candle Stick Pattern Detection:
It is Japanese method for prediction of the stock prices. Candlestick pattern prediction involves analyzing the formations of candlesticks on a price chart to forecast future price movements in financial markets, such as stocks, forex, or cryptocurrencies. Traders use patterns formed by candlesticks, such as doji, hammer, engulfing, and others, along with other technical indicators, to anticipate potential market direction changes.


![image](https://github.com/1203gauri/real_time_market_insights/assets/147191401/6e241e5d-bfa8-4e0b-95ce-8457f65530ab)


Methodology:
The aim of this project is to build an application which outputs accurate recommendations in a quantifiable manner. For this purpose, 3 modules are implemented which are as follows:

Machine Learning module
Sentiment Analysis module
Fuzzy logic Module
Machine learning Module
The purpose of this module is to output Stock Prediction value. Stock Prediction value is the strength of difference in opening price and closing price. For this we need to predict the closing price of the stock. This is achieved by applying Machine Learning on Historical data of the stock.


![image](https://github.com/1203gauri/real_time_market_insights/assets/147191401/3c2e4765-7ce6-4c7c-9fa2-02a87d54e95b)


Sentiment Analysis Module:
The purpose of this module is to obtain the sentiment value of latest news headlines regarding each stock and output its average as sentiment value to fuzzy module. The steps used in this module are as follows:

Data Collection: The data is collected by crawling through Indian Financial news websites. Minimum 4 news Headlines are scraped for each stock and stored against the company Symbol.
Tokenizing: Each news headline is broken down into sentences and then in turn broken down into words.
Lemmatizing: It is the process of reducing inflected (or sometimes derived) words to their word stem, base or root form. For example, “the boy's cars are different colours” reduces to “the boy car be differ colour”
Finding Most Informative Features: Words that contribute most in adding polarity to a sentence are found.
Fuzzy logic Module
The purpose of this module is to output Stock Faith which is the strength of Recommendation. The activation rules for this module are:

IF the News Sentiment was good or the Stock Prediction value was good, THEN the Stock faith will be high.
IF the Stock Prediction value was average, THEN the Stock faith will be medium and completely based on weights assigned.
IF the News Sentiment was poor and the Stock Prediction value was poor THEN the Stock faith will be low.
