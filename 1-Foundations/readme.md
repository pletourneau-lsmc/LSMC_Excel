# Contingent Claim Pricing
For those who want an introduction to option pricing in general, we cover **risk-neutral** pricing approach, used by the vast majority of option pricing methods. Risk-neutral pricing typically provides one price estimate for an option.
For completeness, we also cover **stochastic dominance**. Stochastic dominance can provide upper and lower bounds on price estimates. We conclude this section by describing the extra complexity from allowing early exercise.

The objective here is not to provide a mathematically and theoretically rigourous exposé, but rather to give an intuitive explanation.


## 1.1-Risk-Neutral_Pricing
Risk Neutral pricing is a methodology for pricing financial derivatives. The general idea is that you can create a portfolio of assets, including the financial asset to price, that has risk-free cash flows. Then, if the portoflio is risk-free with deterministic cash flows, there can be only one price for the underlying asset, otherwise, there would be arbitrage opportunities. 

### 1.1.1-Pricing_Forward_Contract
To set ideas, let us cover the valuation of forward prices. A forward contract is a contract that stipulates that the **buyer** will buy an underlying asset on a specified future date that we call maturity at a specified price that we call the forward price from the **seller**. (and much more small prints.) At time $t=0$, the contract has no value as both parties agree on a fair forward price.

How do we find the fair forward price? We need to make several assumptions. First, the asset is tradable and can be bought or sold short. Second, there is a risk-free asset from which we can borrow or lend. Third, there is no default risk.

<!-- The idea is simple. The buyer want to buy the underlying asset, but only at a future date. So, the **market maker** will borrow enough money to buy the asset at today's price and will write his name as the seller on the forward contract. At maturity, the seller will sell the underlying asset at the forward price. If the price is too low, the buyer is happy, but the seller will not have enough money to pay back the loan he took. If the price is too high, the seller is happy, but the buyer will prefer to borrow the money and buy the asset himself.

So, what is the fair forward price? It is simply the price of the asset today, plus the cost of borrowing until the maturity of the contract. This is what leads to the Cost-of-Carry method. The cost of bowwing money to buy the underlying asset and **carry** it until maturity. -->

We will use two different portoflios.
Portfolio \#1 you buy the underlying for $S(0)$, and enter the forward contract as the seller with forward price $F(0,T)$.
At $t=0$, the cash flow is $-S(0)$, and because we entered the forward contract, the cash flow at $t=T$ is $+F(0,T)$, no matter what the price of the underlying will be at $t=T$. And, this is without risk since the value $F(0,T)$ is pre-determined.

Portfolio \#2 you lend $S(0)$ at the risk-free rate. At $t=0$, the cash-flow is $-S(0)$. At maturity, the cash flow will be $S(0) \times (1+r_f)$. And, this is without risk since it is the risk-free rate.

Now, if both portfolios have the same **cost** at $t=0$ and both have a determined (risk-free) cash flow at $t=T$, they must have the same cash flow at maturity, otherwise, this would create an arbitrage opportunity.

This is an example of a **replicating portfolio** as cash flows of portfolio \#2 replicates portfolio \#1. Applying this methodology, we conclude that the only fair forward price $F(0,T)$ is $S(0) \times (1+r_f)$.

**NOTE:** in this example, we do not have to make any assumption on the dynamics of the underlying price.


### 1.1.2-Pricing_a_call_option
