# Market Volatility Modeller

## Motivation
Financial markets are inherently uncertain, and volatility is one of the most important measures of this uncertainty.  
Understanding and modelling volatility is crucial for pricing derivatives, managing risk, and gaining deeper insights into market behavior.  
In this project, historical volatility data is modelled using stochastic processes.
These are defined by stochastic differential equations which can be approximated for simulation using numerical methods.

## Overview
In this project, we study market volatility using **stochastic differential equations (SDEs)**.  
Specifically, we focus on two classical models:  
1. **Ornstein–Uhlenbeck (OU) Process** – a mean-reverting process.  
2. **Cox–Ingersoll–Ross (CIR) Process** – widely used in financial mathematics for interest rates and volatility.  

The models are discretized using the **Euler–Maruyama method**, simulated numerically, and then **fitted to real market data**.  

Model performance is assessed using **Akaike Information Criterion (AIC)** and **Bayesian Information Criterion (BIC)**.  

- AIC is generally preferred when the goal is prediction accuracy. AIC comes from information theory and approximately minimizes expected **KL divergence** from the true model.
- BIC is often preferred when the goal is identifying the true model, especially for large datasets. BIC comes from Bayesian reasoning and approximates the **marginal likelihood** of the model.