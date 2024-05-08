Continued progress based on prior work done by Franklin Williams (UW Computational Finance & Risk Management 2020)

Mean-Variance optimization is known to have several drawbacks. One important drawback is the estimation error within the covariance matrix. Correlations between assets can be shown to be unstable and vary throughout time. Another issue with the standard covariance matrix used in practice is that it is has a high condition number. Lopez de Prado explains how this affects the standard Markowitz Mean-Variance optimization problem,

“…Markowitz’s solution is guaranteed to be numerically stable only if ρ ≈ 0, which is precisely the case when we don’t need it! The reason we needed Markowitz was to handle the ρ≉0 case, but the more we need Markowitz, the more numerically unstable is the estimation of ω_. This is Markowitz’s curse.” [1]
de Prado shows two clustering techniques utilized to generate portfolio allocations that outperform the standard Mean-Variance optimization within the context of Monte Carlo simulation: hierarchical clustering asset allocation (HCAA) [1] and hierarchical risk parity (HRP) [2]. 

For this project, the empirical performance and portfolio composition of these two portfolio-optimization-specific algorithms, standard mean-variance optimization, critical line method, and a benchmark (equal weight) are analyzed. Due to the issues listed above, we hypothesize that the HCAA and HRP algorithms will produce more consistent portfolio results in out-of-sample return data.

All portfolios will be constructed with a one-year look back period and rebalanced weekly.
