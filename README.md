# Investments Project

## Description

This project is designed to provide a comprehensive analysis of investment strategies by integrating multiple financial signals to construct optimal portfolios. The strategies explored include Betting Against Beta (BaB), Momentum (Mom), and Idiosyncratic Volatility (IV). By leveraging data from CRSP and Ken French’s website, the project aims to evaluate the effectiveness of these strategies and to develop industry-neutral portfolios. The analysis involves assessing the performance of these strategies using standard risk factors, examining their exposure to industry risks, and comparing different portfolio construction approaches.

## Project Structure

1. **Introduction**: Overview of the project objectives and data sources. Details on the financial data collected, including stock returns from CRSP and additional data from Ken French’s website.
3. **Betting Against Beta Strategy (BaB)**: Analysis of the BaB strategy, including computation of time-varying market beta and portfolio performance evaluation.
4. **Momentum Strategy (Mom)**: Examination of the Momentum strategy, with a focus on portfolio returns based on past stock performance.
5. **Idiosyncratic Volatility Strategy (IV)**: Evaluation of portfolios based on idiosyncratic volatility, and comparison of performance across different volatility levels.
6. **Optimal Fund Portfolio Return (STRAT)**: Construction of an optimal portfolio by combining BaB, IV, and Mom strategies using different approaches (equal weighting, risk parity, and mean-variance optimization).
7. **Performance and Risk Analysis for the Fund Strategy**: Regression analysis of strategy returns on industry portfolios and Fama-French factors to identify significant risk factors.

## Data and Tools

- **Data Sources**: Monthly stock returns from CRSP (1964-2023) and Fama-French factors from Ken French’s website.
- **Tools Used**: Python, Jupyter Notebook, and various libraries (pandas, numpy, statsmodels, matplotlib).

## Repository Contents

- `notebooks/`: Jupyter Notebooks with the analysis code and results.
- `report/`: Final report in PDF format, detailing the methodology, analysis, and conclusions.
- Data files: The data files used in the analysis are not included in this repository. They can be downloaded directly from CRSP database and Ken French’s website.

## Key Findings

- **BaB Strategy**: While higher beta portfolios generally achieve higher returns, they exhibit a decreasing Sharpe ratio, suggesting additional risk factors beyond those accounted for by CAPM.
- **Momentum Strategy**: The strategy yields significant excess returns, challenging the CAPM by highlighting the importance of momentum effects in stock returns.
- **IV Strategy**: Higher idiosyncratic volatility portfolios show better returns and risk-adjusted performance, further exposing the limitations of CAPM.
- **Optimal Fund Portfolio**: The mean-variance optimization approach delivers the highest returns and Sharpe ratio, demonstrating the superiority of advanced optimization techniques.
- **Risk Analysis**: Significant factors influencing strategy returns include Durbl, Money, and Other, with an R-squared of approximately 26.9% for the industry regression and 28.5% for the Fama-French factors regression.

## Conclusion

The analysis highlights the importance of incorporating multiple signals and advanced optimization techniques to construct superior investment portfolios. Traditional models like CAPM provide foundational insights, but integrating additional factors is crucial for achieving comprehensive risk management and enhanced returns.

## Authors

This project was conducted by Youssef Belghmi, Hamza Morchid, Othmane Idrissi Oudghiri, and Mhamed Sefrioui, Master’s students in Data Science at EPFL. It was completed as part of the end-of-semester project for the Investments (FIN-405) course, taught by Professor P. Collin-Dufresne, contributing to their minor in Finance.
