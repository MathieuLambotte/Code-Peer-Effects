# Codes-Peer-Effects
R Codes to estimate Peer Effects with different models, building on Lee, Li and Lin (2014)'s Binary Choice Models with Social Network under Heterogeneous Rational Expectation (https://doi.org/10.1162/REST_a_00401) for the Simulated Iterative Maximum Likelihood estimator (SIML_LLL function in my code) and on Boucher and Bramoullé 2020's Binary Outcomes and Linear Interactions (https://halshs.archives-ouvertes.fr/halshs-03031767/document) for the Nonlinear Least Squares estimator (NLS_BB) and the 2SLS estimator (IV_BB). 

This a work in progress, intended for my own research but someone might find it useful.

For now, SIML_LLL only accepts models with exogenous peer effects and fixed effects, while NLS_BB and IV_BB accept models with or without fixed effects and exogenous peer effects. So I created seperate but similar functions for SIML witout fixed effects (SIML_LLL2) and SIML without exogenous peer effects and fixed effects (SIML_LLL3).
In addition, IV_BB is more complete at the estimator allows for demeaning when using fixed effects (as in a panel data with fixed effects) and clustered-robust standard errors. You can also extract the model matrix using get.df=TRUE in IV_BB.
