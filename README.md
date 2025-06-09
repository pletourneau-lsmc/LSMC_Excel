# SUPER Least squares Monte Carlo
## How to price options efficiently for (almost) any dynamics model!

Financial options and contingent claims in general are complex to price when model parameters are known. 
Finding those model parameters can be an insurmontable challenge. 
Up until now!
Over the years, we have developed a methodology that allows calibrating a dynamics model on a sample of option prices in an instant.

Among the different methods allowing for pricing contingent claims with early exercise, the least square Monte Carlo (LSMC) method is the most flexible. 
The original method is not the most efficient, though. 
Our extensions that we developed through the years does make the LSMC method very competitive. We call it the SUPER-LSMC.

Our objective here is to make this as accessible as possible.
We will cover all the basics, from the theory of contingent claims pricing, all the way to how to use our method to calibrate the most complex dynamics model on all options traded on the CBOE.

Jump to [how to use our product]

Here is the plan:
<!--# The Least-Square Monte Carlo Method: A Comprehensive Guide -->

## ⏳1- Foundations of Contingent Claim Pricing
For those who want an introduction to option pricing in general, we cover **risk-neutral** pricing approach, used by the vast majority of option pricing methods. Risk-neutral pricing typically provides one price estimate for an option.
For completeness, we also cover **stochastic dominance**. Stochastic dominance can provide upper and lower bounds on price estimates. We conclude this section by describing the extra complexity from allowing early exercise.

### ⏳1.1- Risk-Neutral Pricing
- Intuitive Introduction to Risk-Neutral Pricing  
- Common Academic Assumptions and Their Realism  

### ⏳1.2- Stochastic Dominance in Pricing
- A Closed-Form Example  
- A Simulation-Based Example  

### ⏳1.3- Early-Exercise Contingent Claims
- The General Problem  
- Approaches to Determining the Exercise Boundary  


## ⏳2- Overview of Option Pricing Methods
Contingent claim pricing in general and option pricing in particular using the risk-neutral approach implies solving an extectation or, simply, an integral. If early exercise is possible, an optimal stopping time also needs to solved. There are many approaches available. Our objective here is simply to list all those methods, and then argue that a simulation based method is the most flexible, in the sense that it can be applied to the largest set of dynamics models. Simulation based methods can accomodate very complex dynamics. There are challenges, though. In particular, if you want to price options from a specific dynamics model, you first need to calibrate the model parameters. If you want your model to fit observed option prices, you need to price options with multiple strikes, multiple maturities, over multiple days. And, when optimizing for the best parameters, you will have to repeat this multiple times. On top of this, because of the simulation approach, you will have a noisy optimization which can be very challenging, though not impossible. 

### ⏳2.1- Survey of Pricing Approaches
- A Survey of Common Methods  
- Limitations of Each Method

### ⏳2.2- Simulation-Based Approaches
- Flexibility of Simulation in Option Pricing  
- Computational Challenges in Simulation  



## 3- The Least-Square Monte Carlo Method (LSMC)
Our very efficient method is based on the least square Monte Carlo (LSMC) method of [Longstaff and Schwartz (2001)](https://doi.org/10.1093/rfs/14.1.113). They use a small numerical example in their paper to help readers understand the steps involved. We provide two representation of that small numerical example: one in Excel, one in python.

- ⚠️ [3.1 Original Small Numerical Examples](https://github.com/pletourneau-lsmc/SUPER_LSMC/tree/main/3-LSMC/3.1-Original_example)  
- ⚠️ [3.2 Extended Examples](https://github.com/pletourneau-lsmc/SUPER_LSMC/tree/main/3-LSMC/3.2-Extended_Example)

<!--### ⏳Challenges in Simulation-Based Pricing
- Issues in Pricing  
- Issues in Model Calibration
- General computer limit issues-->


## ⏳4- Super LSMC
### ⏳Challenges in Simulation-Based Pricing
- Issues in Pricing  
- Issues in Model Calibration
- General computer limit issues

### ⏳Multiple useful extensions, leading to Super-LSMC
- Initial State Dispersion (ISD)
- Homogeneity and Multi-Strike Pricing  
- Markov Property and Multi-Maturity Pricing
- Bootstrapping
- ISD and Greeks
- ISD and model parameters
- Gigantic calibration setup
- How to use our output

## ⏳How to use our product





# References

Longstaff, F. A., & Schwartz, E. S. (2001). Valuing American Options by Simulation: A Simple Least-Squares Approach. The Review of Financial Studies, 14(1), 113–147. https://doi.org/10.1093/rfs/14.1.113 
