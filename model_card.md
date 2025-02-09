# Model Card

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
The data has a typical split of 75/25 for the train/test split.

Data Preprocessing
The date, close and change fields were removed as the model is predicting the output.
The code for the output was run (located at X) and a csv called out.csv was generated.

## Performance

The performance of the model is done with a classication report and a view of tree complexity. The full details are in the jupiter notebook 'Model_random_forest', the final comparison was on the test data which is a standard 25/75 split on test vs train on the overall dataset.


## Limitations

Training data
The model was trained when there was not market crashes in a relatively calm environment. This led to a smaller dataset to train from. 

Task Complexity
Limited to working with a trailing stop loss with a fixed margin. This is true when both testing on the upside and downside.
It is not trained to support other order types or strategies.

## Trade-offs

When the market is volatile, such as a crash or rapid decline, the model will perform poorly since it was not trained for this.