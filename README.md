# Big Tech Stock Prices Analysis

## Datasets

- [Big Tech Stock Price Dataset](https://github.com/rfordatascience/tidytuesday/blob/main/data/2023/2023-02-07/readme.md)
- This dataset contains stock price data for big techs like Apple, Amazon, Google, Microsoft. The data is about daily trading info such as opening and closing prices, trading volume, and price adjustments, from January 2010 to 2023.
- Our team choose this dataset simply because we want to gain more insights about the fluctuations throughout the technology revolution, and see how important events and emerging technologies like LLMs reshaped the stock value of tech industry.
## Data Dictionary

| Variable     | Class     | Description                                                                                                                                                                                                                      |
| ------------ | --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| stock_symbol | character | Stock symbol                                                                                                                                                                                                                     |
| date         | double    | Date                                                                                                                                                                                                                             |
| open         | double    | The price at market open                                                                                                                                                                                                         |
| high         | double    | The highest price for that day                                                                                                                                                                                                   |
| low          | double    | The lowest price for that day                                                                                                                                                                                                    |
| close        | double    | The price at market close, adjusted for splits                                                                                                                                                                                   |
| adj_close    | double    | The closing price after adjustments for all applicable splits and dividend distributions. Data is adjusted using appropriate split and dividend multipliers, adhering to Center for Research in Security Prices (CRSP) standards |
| volume       | double    | The number of shares traded on that day                                                                                                                                                                                          |

## Questions

- What are the correlations between stock price trends of these big techs, and how have these correlations changed over time? If one exist, what market factors or industry trends might explain these relationships?
- How did major economic events (financial crisis, COVID-19 pandemic, the rise of LLMs) affected the volatility and recovery patterns of different tech stocks?

## Plan

- [X] Create repository and add dataset
- [ ] Data exploration and preprocessing
- [ ] Correlation analysis
  - [ ] Calculate and visualize correlations between companies
  - [ ] Analyze correlation changes over time
  - [ ] Identify market factors affecting correlations
- [ ] Events impact analysis
  - [ ] Define key event periods (financial crisis, COVID-19, rise of LLMs, ...) and get corresponding external datasets
  - [ ] Analyze trends during these periods and compare patterns across different stocks
- [ ] Final report
