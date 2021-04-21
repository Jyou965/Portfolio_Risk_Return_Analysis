# Portfolio_Risk_Return_Analysis

This application evaluates given portfolios' risk-adjusted return and sensitivities to the broad market.  Based on the analysis, the user, who tends to be an investment advisor can make investment recommendation of which porfolio is the best addition to a client's retirement account.

---

## Libraries and Dependancies

This application leverages python 3.7 with the following packages:

* [pandas](https://pandas.pydata.org/docs/) - an open source, BSD-licensed library providing high-performance, easy-to-use data structures and data analysis tools for the Python programming language.

* [path library](https://docs.python.org/3/library/pathlib.html) - for utilizing filesystem paths with semantics appropriate for different operating systems.

* [numpy](https://numpy.org/doc/) - a Python library that provides a multidimensional array object, various derived objects (such as masked arrays and matrices), and an assortment of routines for fast operations on arrays, including mathematical, logical, shape manipulation, sorting, selecting, I/O, discrete Fourier transforms, basic linear algebra, basic statistical operations, random simulation and much more.

* [%matplotlib](https://matplotlib.org/) - a comprehensive library for creating static, animated, and interactive visualizations in Python.

---

## Usage

The application evaluates four given portfolios, including Berkshire Hathaway, Paulson & Co., Tiger Global Management and Soros Fund Management for the period of October 1, 2014 through September 11, 2020. The following characteristics are analysed against S&P 500 index in sequence:

1. Cummulative returns: As indicated by the chart below, none of the four portfolios outperformed the S&P 500 during the period, with Berkshire Hathaway delivering the best relative cummulative return results.

![Cummulative_Returns]()

2. Risks: Using 21-day rolling standard deviation over the period, the risk profile of the four portolios are demonstrated below, with and without S&P 500 benchmark. None of the portfolios had higher 21-day rolling standard deviation than the S&P 500, with Berkeshire Hathaway having the highest relative standard deviation for most of the period.

![21_day_std_w_snp]()

![21_day_std_wo_snp]()

3. Risk-adjusted Return: By using Sharpe Ratio, which indicates return per unit of risk, one can see the risk-adjusted return ranking.  Berkshire Hathaway not only had the highest Sharpe ratio among the four portfolios but also outperformed S&P 500 on this basis.

![sharpe_ratio]()

4. Diversification Considerations: Here we use Beta as a measurement. Beta indicates a portfolio's sensitivity toward the benchmark.  Berkshire Hathaway had an average of 60-day rolling beta of 0.22, while Soros Fund's 60-day rolling beta was 0.07.  The trajectory of the beta of the two porfolios are desplayed below:

![berkshire_beta]()

![soros_beta]()

Given a strong outlook for the S&P 500 as the world gets out of Covid-19 with the help of vaccination, portfolios with higher beta will benefit more from the market strength.  This, coupled with the highest Sharpe ratio makes Berkshire Hathaway our recommendation for client portfolios.

---

## Contributors

Jackie You with the support of FinTech Boot Camp Staff

---

## License

Berkeley
