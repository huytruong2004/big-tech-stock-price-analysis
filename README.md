# Big Tech Stock Prices Analysis

## Datasets

- [Big Tech Stock Price Dataset](https://github.com/rfordatascience/tidytuesday/blob/main/data/2023/2023-02-07/readme.md)
- This dataset contains stock price data for big techs like Apple, Amazon, Google, Microsoft. The data is about daily trading info such as opening and closing prices, trading volume, and price adjustments, from January 2010 to 2023.
- Our team choose this dataset simply because we want to gain more insights about the fluctuations throughout the technology revolution, and see how important events and emerging technologies like LLMs reshaped the stock value of tech industry.

## Data Dictionary

**Big Tech Stock Price Dataset**

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

**Events Timeline Dataset (External)**

| Variable     | Class     | Description                                                                |
| ------------ | --------- | -------------------------------------------------------------------------- |
| stock_symbol | character | Stock symbol                                                               |
| date         | date      | Date                                                                       |
| description  | character | Short description of what happened                                         |

## Questions
- What are some fundamentals and useful indicators that newbies must know to perform basic technical analysis?
- How did product/service launched dates, company-related events amd major economic events (financial crisis, COVID-19 pandemic, the rise of LLMs) affected the volatility and recovery patterns of different tech stocks?
- What are the correlations between stock price trends of these big techs, and how have these correlations changed over time? If one exist, what market factors or industry trends might explain these relationships?

## Plan

- [X] Create repository and add dataset
- [X] Manually collect data to form up the company-specific event time line dataset
- [ ] Events impact analysis
  - Use Plotly to create candlestick charts for all 15 big techs to show daily trading data (using open, high, low, close columns), with an option to choose the period (7D, 30D) to display.
  - Overlay with calculated indicators like moving averages (MA) and Bollinger Bands to illustrate volatility to support technical analysis, with an option to toggle on or off.
  - Overlay event markers (annotations) at specific dates to denote product launches, company events, or economic milestones and showing details only on hover. 
- [ ] Correlation analysis
  - Pick some high-impact events between companies during that event period.
  - Use interactive heatmaps and correlation matrices that update over different sliding window.
  - Give insights about the companies' correlation (Why are they behaving like that? What causes?, What market factors or industry trends might explain these relationships?)
- [ ] Presentation
- [ ] Final report
