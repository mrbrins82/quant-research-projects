# Mixed Quant Strategies in Crypto Trading

## Overview

This strategy explores a mixture of models. Here are the [project slides](https://github.com/mrbrins82/quant-research-projects/blob/main/ensemble-models-crypto-strat/quant_ensemble_crypto_project.pdf).

1. A technical indicator strategy based on moving averages, momentum indicators, drawdown indicators, and some other engineered indicators.
2. A supervised ML model that classifies the next day returns, emphasizing for precision since false positives cost money.
3. An unsupervised ML model that clusters different regimes during bullish-bearish-neutral periods.

## Results

These strategies were trained from 2021-01-01 to 2023-12-31, and validated on data from 2024-01-01 to 2024-12-31. For the OOS testing which ran from 2025-01-01 to 2026-02-28, the strategies were weighted using various methods based on their performance during the validation period. The best performing overall strategy was the one that combined individual strategies based on their Sharpe Ratios during the validation period. 

<u>__Overall Strategy Results__</u>

* __Sharpe Ratio: 2.001__
* __$\alpha$ t-stat: 2.150__
* __$\alpha$: 0.0010__
* __Information Ratio: 1.07__
