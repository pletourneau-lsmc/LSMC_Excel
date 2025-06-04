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
### ⏳Risk-Neutral Pricing
- Intuitive Introduction to Risk-Neutral Pricing  
- Common Academic Assumptions and Their Realism  

### ⏳Stochastic Dominance in Pricing
- A Closed-Form Example  
- A Simulation-Based Example  

### ⏳Early-Exercise Contingent Claims
- The General Problem  
- Approaches to Determining the Exercise Boundary  

## ⏳2- Overview of Option Pricing Methods
### ⏳Traditional Pricing Approaches
- A Survey of Common Methods  
- Limitations of Traditional Methods  

### ⏳Simulation-Based Approaches
- Flexibility of Simulation in Option Pricing  
- Computational Challenges in Simulation  

## 3- The Least-Square Monte Carlo Method (LSMC)
- ⚠️ [3.1 Original Small Numerical Examples](https://github.com/pletourneau-lsmc/SUPER_LSMC/tree/main/3-%20LSMC/3.1-%20Original)  

### ⏳Challenges in Simulation-Based Pricing
- Issues in Pricing  
- Issues in Model Calibration
- General computer limit issues


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
