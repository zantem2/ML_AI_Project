# Model Card

See the [example Google model cards](https://modelcards.withgoogle.com/model-reports) for inspiration. 

## Model Description

This model is to predict the result of a stock trade when fed in real life information. 

**Input:**
The X input is a dataset of daily stock market performance
The y input is the result of running a stop loss model

**Output:** 
The output of the model is the determination of weather to buy or sell a stock while following a trailing stop/loss approach. Therefore it is returning a binary classification.

**Model Architecture:**
Since this is a classification problem, the random forest architecture has been used. This will allow the different indicators to be used to generate an overall opinion. e.g. MACD, RSI indicate an upward trend so buy since the stop loss has not been hit.

The underlying performance of the model has been improved by Bayesian optimisation.

## Model Data

Training Dataset
The training data is made up of a subset of daily trade information from 1st Marcb 2022 - 1 July 2024. This is a period of relative calm in the markets avoiding crashes.
The data has a typical split of 75/25 for the train/test split

Data Preprocessing
The date field was removed due to parsing error.
The code for the output was run (located at X) and a csv called out.csv was generated

## Performance

Give a summary graph or metrics of how the model performs. Remember to include how you are measuring the performance and what data you analysed it on. 

accuracy report
graph of actual vs predicted

## Limitations

Outline the limitations of your model.
Training data
The model was trained when there was not market crashes in a relatively calm environment. This led to a smaller dataset to train from. 

Task Complexity
Limited to working with a trailing stop loss with a fixed margin. This is true when both testing on the upside and downside.
It is not trained to support other order types or strategies.

## Trade-offs

Outline any trade-offs of your model, such as any circumstances where the model exhibits performance issues. 
When the market is volatile, such as a crash or rapid decline, the model will perform poorly since it was not trained for this.