Sunspot Time Series Analysis 
Objective :
The aim of this practical is to analyze monthly mean total sunspot numbers using Python libraries such as NumPy, pandas, and Matplotlib, and to model the phenomenon using a Gamma distribution. The task includes time series visualization, distribution modeling, MCMC-based parameter estimation, and prediction of the Gamma parameters over different sample groups.

Dataset Description :
A sunspot is a region on the Sun’s surface (photosphere) with a lower temperature than its surroundings, caused by strong magnetic field concentrations that inhibit convection. 
Sunspots:
Often appear in pairs of opposite magnetic polarity 
Vary in number according to an approximate 11-year solar cycle

The dataset used here is the “Monthly mean total sunspot number”: 
Property                                Description 
Source                       World Data Center for the production, preservation and dissemination of the international sunspot number 
Time Range                   January 1749 to November 2018 
Frequency                    Monthly observations 
Variable                     Monthly mean total sunspot number

Tasks Performed :
Step 1 – Time Series Plot 
Plot the sunspot numbers over time (months/years) 
Visually inspect: 
o Overall trend 
o Periodicity / cycles (~11 years) 
o Variations in amplitude over time 

Step 2 – Gamma Distribution Modeling (Per Cycle) 
 Model the sunspot counts using a Gamma distribution 
 Assume a new cycle resets every 12 years 
 For each 12-year cycle: 
o Fit a Gamma distribution with parameters a (shape) and b (rate/scale, depending on convention) 
o Compare how the parameters vary across cycles

Step 3 – Histogram of Sunspot Counts 
 Plot a histogram of the sunspot counts 
 Compare the empirical distribution with the Gamma model 
 Check whether the Gamma distribution is a reasonable fit for the data 

Step 4 – MNMC with Different Sample Groups 
Given fixed parameters a = 4 and b = 10, compute and plot the MNMC (Monte Carlo-based quantity/estimate) for: 
First 50 samples 
All samples 
Last 50 samples 
This allows comparison of how estimates behave on early, full, and recent data segments. 

Step 5 – MCMC Traces for a and b 
 Use MCMC (Markov Chain Monte Carlo) to estimate the posterior distributions of a and b 
 Perform: 
o Burn-in / burn-out: discard initial part of the chain to remove dependence on starting 
values 
o Plot: 
Trace plots of a and b across iterations 
Histograms of the sampled values for a and b 
Check: 
o Convergence of the chains 
o Stability of the estimates 

Step 6 – Prediction of a and b 
 Use the posterior samples of a and b to: 
o Compute point estimates (mean/median) 
o Provide interval estimates (credible intervals) 
 Interpret these as the predicted Gamma parameters for the sunspot process: 
o How concentrated is the distribution? 
o How heavy is the tail? 
o What does that imply about extreme sunspot activity?


Tools Used :
Python 3.x 
NumPy 
pandas 
Matplotlib / Seaborn 
SciPy 
PyMC / PyMC3 / another MCMC library (for Bayesian inference) 
Jupyter Notebook / Google Colab







