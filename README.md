# Spatio-Temporal Modeling of Equity Markets Using Graph Neural Networks

This repository contains model code files and the final PDF version of my Master's thesis, **"Spatio-Temporal Modeling of Equity Markets Using Graph Neural Networks"**, submitted for the Master's Degree in Data Science for Economics at the **Università degli Studi di Milano**.

## Overview

The thesis investigates whether spatio-temporal Graph Neural Networks (GNNs) can improve cross-sectional stock return ranking in the Indian equity market. Traditional time-series models often treat assets as independent sequences, while equity markets are strongly influenced by sectoral relationships, price co-movement, liquidity shocks, and cross-stock spillover effects.

To address this, the thesis develops a quantamental graph-based framework that combines:

- market-cap-scaled volume shocks as node-level features,
- sector-based graph edges,
- return-correlation-based graph edges,
- temporal financial features,
- and a Hybrid Quantile-Ranking Loss for return ranking and downside-risk calibration.

The empirical analysis compares three modeling approaches:

1. **LSTM baseline** — a temporal-only benchmark model.
2. **GAT-LSTM Hybrid** — a graph-attention and temporal fusion model.
3. **ROLAND architecture** — a dynamic graph neural network for evolving market structure.

## Key Findings
- The GAT-Hybrid model outperforms the temporal-only LSTM baseline in out-of-sample trading performance.
- Graph-based relational structure improves the modeling of cross-sectional equity returns.
- Liquidity-aware features, especially market-cap-scaled volume shocks, provide useful predictive information.
- The ROLAND model achieves strong validation performance but shows out-of-sample degradation, highlighting the difficulty of modeling financial regime shifts.
- The results support the use of graph-based learning for capturing relational dependencies in equity markets.

## Topics
- Graph Neural Networks for financial markets
- Spatio-temporal modeling
- Equity return prediction
- Cross-sectional stock ranking
- Indian stock market (NSE) analysis
- Graph Attention Networks
- Dynamic GNNs and ROLAND
- Quantile regression and ranking loss
- Liquidity shocks and market microstructure

## Author

**Akash Mittal**  
Master's Degree in Data Science for Economics  
Università degli Studi di Milano

## Supervisors

- **Prof. Matteo Zignani** — Supervisor
- **Prof. Anita Quas** — Co-supervisor

## Academic Year

**2023–2025**

This repository is intended for academic documentation and public reference. Some materials related to the thesis, including datasets, source code, LaTeX files, and intermediate experiment outputs, are not included because they may be proprietary, too large, restricted by data-provider terms, or outside the scope of this public repository.
