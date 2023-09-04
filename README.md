# Control Variates for GARCH Model - GitHub Repository

## Introduction
This GitHub repository contains a project focused on implementing and exploring the use of control variates for a GARCH (Generalized Autoregressive Conditional Heteroskedasticity) model. The project is inspired by a numerical example presented in the paper titled [link to the paper](https://doi.org/10.1007/s11222-012-9344-6).

## Project Overview
The primary objectives of this project are as follows:

1. **Implement a Random Walk Metropolis Sampler** (source/MCMC_Q1.ipynb): The project begins by following the guidelines outlined in the referenced paper to create a Random Walk Metropolis sampler. This sampler targets the posterior distribution of a GARCH model. Initially, the implementation utilizes simulated data, and subsequently explores real-world data, specifically log-returns computed from exchange rates. 

2. **Introduction of Control Variates** (source/ZV_MCMC_P1_Q2.ipynb.ipynb): The project introduces control variates as proposed in the paper. Special attention is given to the control variates based on a first-order polynomial (Equation (8) in the paper). The project elucidates how these control variates can be effectively incorporated into the GARCH model through linear regression.

3. **Expanding Control Variates Set** (source/ZV_MCMC_P2_Q3.ipynb.ipynb) : To enhance the analysis, a broader array of control variates is considered, including those based on a polynomial of order 2. However, the project acknowledges the potential computational challenges that arise when dealing with a large number of control variates. An explanation is provided for why the linear regression approach, as introduced in Step 2, might become prohibitively expensive. The project proposes an alternative method inspired by [this paper](https://doi.org/10.1007/s11222-021-10011-z) that leverages the Lasso technique and conducts a comparative analysis against the naive linear regression approach.

4. **Bonus Challenge**: The project goes beyond the core objectives to address the question of whether applying linear regression to an MCMC (Markov Chain Monte Carlo) sample is entirely valid. It explores potential solutions to make MCMC simulations less dependent, such as sub-sampling.

## Purpose of this Repository
This GitHub repository serves as a comprehensive resource for understanding and replicating the project's findings related to control variates for GARCH modeling. It provides access to the project code, data sources (including simulated and real-world data), detailed explanations, and insights gained from the analysis.

Feel free to explore the repository to gain a deeper understanding of control variates in the context of GARCH modeling and their potential impact on statistical analysis in financial applications.
