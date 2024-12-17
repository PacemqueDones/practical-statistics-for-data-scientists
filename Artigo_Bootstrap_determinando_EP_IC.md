# Case Study: Determining Standard Error and Confidence Inverval of Annual Income Using Bootstrap Resampling

## Introduction
This paper analyzes the annual income of Lending Club loan applicants to determine the standard error of the mean and construct a confidence interval. Two distinct methodologies are employed: a non-parametric approach using bootstrap resampling, and a parametric approach that models income using a Log-normal distribution. The bootstrap method is advantageous when distributional assumptions are uncertain, while the parametric approach offers computational efficiency if the distributional assumption is valid. This analysis compares the results obtained from both methods to assess their relative accuracy and applicability.

## Development

### Data Acquisition:
Prior to commencing the analysis, the data was retrieved from a publicly available CSV file located at [link](https://raw.githubusercontent.com/PacemqueDones/practical-statistics-for-data-scientists/refs/heads/main/DataBase/loans_income.csv).

```python
path = 'https://raw.githubusercontent.com/PacemqueDones/practical-statistics-for-data-scientists/refs/heads/main/DataBase/loans_income.csv'

dfIncome = pd.read_csv(path)

dfIncome.head(5)
```