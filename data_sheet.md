## Motivation

The data sheet was created to form a source for the Machine learning project which is part of the MLAI course.
It was created by myself for this purpose and had no attached funding. Barchart was used as a source.
 
## Composition

The data sheet contains the daily market information of the SPY etf which is a sequence of values of data in a CSV. There are 543 rows and 18 columns (15 used)
There is no missing data in the time period of 1/3/2022 to 1/7/2024.
The technical information does not contain personal information. The expanded columns can be calculated from the source of (open/close/volume) as they are all technical indicators.

## Collection process

The data was acquired from Barchart. Sign up for an account and download CSV data for SPY.
The data is available to be extracted at a more detailed time frame e.g. per hour but daily time period was used to keep size requirements low.
The data was collected as one click, there is the ability to download data.

## Preprocessing/cleaning/labelling

The original data contained information from 08/01/2020 it was truncated to 1/3/2022 to 1/7/2024. The reason is due to how technical indicators operate, there was missing data (e.g. a 200D average needs 200 price entries). Data after 1/7/2004 was truncated to avoid crashes as defined at [https://en.wikipedia.org/wiki/List_of_stock_market_crashes_and_bear_markets]
The remaining data had no null fields.
There are 15 columns out of 18 used. The unused fields where Date, Close, Change. These are dropped in the model but kept should there be a future use. 

## Uses

The dataset was intended to train the model for this project, however it could not be used for other personal purposes.
This should not be used for financial determinations it is meant as an example dataset within a specific time period.
To mitigate potential harm, users should sign up at Barchart and download the dataset themselves.

## Distribution

The dataset that was created has not been shared. Instructions from the university task and lecturers and Barchart License mean that the dataset is not shared.

The data is used under license [https://www.barchart.com/terms]
    In addition, you may use the Barchart Services as follows for your personal, non-commercial use only:
        You may use Barchart Content offered for downloading, such as daily data files, for personal use only and subject to the rules, if any, that accompany           that particular Content.
Hence the use is personal, non-commercial in nature (using to train a model for personal use and coursework submission) and not sharing the data.
This is why you are directed to download the dataset yourself to be compliant.

## Maintenance

The dataset is not subject to maintenance through personal use.
