# Analyzing Stock Price of Tesla Using CAPM

<i>Filsan Musa</i>

## Summary

> This project analyses the price of Tesla's stock, ticker TSLA, to determine whether the asset is fairly priced. This will be done through comparing the performance of TSLA to the overall performance of the stock market. To get the performance of the stock market the SPDR S&P 500 trust, ticker SPY, will be used. The SPY is a good indicator of the overall market performance as it mimics the S&P 500, and is the largest global ETF. <br>

## Understanding CAPM

The Capital Asset Pricing Model, known as CAPM, is model that evaluates the value of a stock, and is used to determine where a stock is overvalued, undervalued, or fairly priced. The following formula will be used to determine this:

<br>

<center>

$$
Y_t=\beta_o + \beta_1X_t + \epsilon_t
$$

</center>

<br>

$Y_t$: is the Excess Return of TSLA <br> $X_t$: is the Excess Return of the market <br> $\beta_o$: is the intercept/constant and measures pricing error <br> $\beta_1$: is the slope of the security charateristic line <br> $\epsilon_t$: is the error term <br>

## Install Packages

The following R libraries will be required: <br>

<ul>

<li>

Dplyr

</li>

<li>

Ggplot2

</li>

</ul>

## Meet the Data

You can include R code in the document as follows:

```{r}
df <- read.csv("/Users/filsanbeddel/Documents/PORTFOLIO PROJ/TSLA_CAPM/TSLA.csv", header = TRUE)
head(df, 10)
summary(df)
```
