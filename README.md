# ML_AI_Project
# PROJECT TITLE 


## NON-TECHNICAL EXPLANATION OF YOUR PROJECT
100 words to explain what your project is about to a general audience. 
The project is to determine when to enter/exit a trade based on a trailing stop strategy
A trailing stop is:-
![Screenshot](./strategy_diagram.jpg)

The idea is that you cannot exactly state when you will reach a market top. Nor can you exactly state when the market has hit a bottom. 
A better approach is to wait for indications of a market recovering before entering a trade. Otherwise you are guessing while price is falling where to buy.

## DATA
A summary of the data you’re using, remembering to include where you got it and any relevant citations. 

The dataset is from Barchart and contains no personally identifiable data. All data is from publicly available sources of the stock market for the main information. The detailed stock information is downloaded from Barchart.
A datasheet for the project is in the folder. This includes steps to obtain your own data

It seems from this source that a time without significant movement is:-
1 March 2022 – 1 July 2024
https://en.wikipedia.org/wiki/List_of_stock_market_crashes_and_bear_markets

This is a period that did not have any major shocks for the US market. Major shocks would skew results and would mean that really you would need to include market sentiment to understand the move. This adds another layer of complexity and is out of scope for this project.
# Biases

The dataset dates used within the modelling are when there are not periods of market corrections. This period is also when AI was launched mainstream. This resulted in an unusually positive market (bullish) which may hinder performance in a neutral or down trending (bearish) market.
<Diagram of market trends>

## MODEL 
A summary of the model you’re using and why you chose it. 

The chosen model type is a random forest since this is a classification problem. Given there are different types of indicators, it is best to split these out and get an aggre

## HYPERPARAMETER OPTIMSATION
Description of which hyperparameters you have and how you chose to optimise them. 


## RESULTS
A summary of your results and what you can learn from your model 

You can include images of plots using the code below:
![Screenshot](image.png)

## (OPTIONAL: CONTACT DETAILS)
If you are planning on making your github repo public you may wish to include some contact information such as a link to your twitter or an email address. 

