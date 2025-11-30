PART A – Metropolis Algorithm 
1. Objective 
To implement the Metropolis algorithm, a Markov Chain Monte Carlo (MCMC) 
technique, for sampling from complex probability distributions that cannot be 
sampled directly. 
 To generate samples from a given target distribution (unnormalized allowed). 
 To analyze the sampling behavior using trace plots, histograms, acceptance rate, 
and autocorrelation. 
2. Description 
The Metropolis algorithm is an MCMC method used to simulate samples from a probability 
distribution when direct sampling is difficult. 
Key Ideas 
 Start from an initial guess. 
 Propose a new state using a symmetric proposal distribution (usually Normal). 
 Accept or reject the proposed state using an acceptance probability. 
 Over iterations, the chain converges to the target distribution. 
Why It Is Used 
 Works even when the target density is unnormalized. 
 Useful for Bayesian inference, statistical physics, and probabilistic modeling. 
 Can sample from multimodal or complicated distributions. 
3. Workflow of Metropolis Algorithm 
Step 1 — Define Target Distribution 
 Provide the log of the density (unnormalized is acceptable). 
Step 2 — Initialize 
 Choose: 
o a starting value x0x_0x0 
o number of iterations NNN 
o proposal distribution scale (e.g., Normal(0, σ²)) 
Step 3 — Iterate (Markov Chain Sampling) 
For each iteration: 
1. Propose a new sample: 
y=x+ϵ where ϵ∼N(0,σ2) 
2. Compute the acceptance ratio: 
α=min(1,p(y)/p(x)) 
3. Accept/Reject: 
If accepted → move to y 
If rejected → stay at x 
Step 4 — Post-processing 
Remove burn-in (initial low-quality samples) 
Plot: 
o Trace plot 
o Histogram of samples 
o Autocorrelation 
Compute: 
o Acceptance rate 
o Effective Sample Size (ESS) 
PART B – Deterministic Model 
1. Objective 
To implement a deterministic mathematical model, such as the logistic growth 
model or any ODE-based system. 
 To solve the ODE using numerical integration (Euler or RK4). 
 To study system behavior for different parameter values. 
2. Description 
A deterministic model describes how a system evolves predictably over time using 
mathematical equations (usually ODEs). 
No randomness is involved—same initial conditions produce the same output. 
Example Used 
Logistic Growth Model 
dx/dt = rx(1-x/K) 
Where: 
 r: growth rate 
 K: carrying capacity 
 x(t): population at time t 
Numerical Solver 
The Runge–Kutta 4 (RK4) method is used: 
 More accurate than Euler’s method 
 Widely used for biological, physical, and engineering models 
3. Workflow of Deterministic Model 
Step 1 — Define the ODE 
Provide the function f(t,x) describing the system. 
Step 2 — Choose Parameters 
 Growth rate r 
 Carrying capacity K 
 Initial value xo 
 Time range to to t1 
Step 3 — Implement Numerical Solver 
 Use RK4 (or Euler) to compute the next value of the state variable. 
 Repeat for all time steps. 
Step 4 — Simulate for Different Parameters 
Run the solver for multiple values of r to observe: 
 Faster/slower growth 
 How quickly population approaches carrying capacity 
Step 5 — Plot Results 
 Plot x(t) vs. t for each growth rate
 Compare the trajectories 
