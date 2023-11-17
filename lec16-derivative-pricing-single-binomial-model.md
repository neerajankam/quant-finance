## ****Derivative Pricing in a Single Period Binomial Model****

- Single period binomial model terminology
    
In the single-period binomial model, which is commonly used in option pricing, several key terms and variables are involved:

- **t**: This represents the time period for the model. In the single-period model, there is only one time step, so "t" typically equals 1.
- **r**: "r" is the risk-free interest rate. It represents the return an investor can earn with no risk of financial loss. In the binomial model, this rate is used to calculate the risk-free discount factor for determining the present value of future cash flows.
- **S0**: This is the initial stock price at the beginning of the time period (t=0).
- **S1**: "S1" represents the stock price at the end of the time period (t=1). It can take on two values: one for an up movement (usually denoted as "u") and one for a down movement (usually denoted as "d").
- **u and d**: These are the factors representing the possible up and down movements of the stock price from time t=0 to t=1. "u" typically represents the factor by which the stock price increases in an up movement, while "d" represents the factor by which the stock price decreases in a down movement. They help model the uncertainty and volatility of the stock price.

In the single-period binomial model, you can calculate option values, particularly for European options, by considering the possible future values of the underlying asset at the end of the period (S1) and then working backward to determine option values at t=0. The option's payoff is determined by the relationship between the strike price and the future asset price (S1), and the risk-free discounting of this payoff to the present value.

This model provides a simple framework for understanding option pricing and how various factors, such as the risk-free interest rate and the possible up and down movements of the asset, influence option values. It's a building block for more complex option pricing models like the Black-Scholes model.
    
- Payoff of European options at t=1
    
The payoff for European call and put options at expiration (t=1) can be expressed as follows:

For a European call option with a strike price of "K":

- The call option payoff is given by: max(S1 - K, 0)

This means that the option holder will receive the positive difference between the stock price at expiration (S1) and the strike price (K) if it is positive; otherwise, the payoff is zero.

For a European put option with a strike price of "K":

- The put option payoff is given by: max(K - S1, 0)

This means that the option holder will receive the positive difference between the strike price (K) and the stock price at expiration (S1) if it is positive; otherwise, the payoff is zero.

These payoff expressions represent the profit or loss the option holder would realize at the expiration of the option, depending on the final stock price (S1) and the strike price (K). If the stock price is favorable, the option holder will exercise the option and receive a positive payoff; otherwise, the payoff is zero.
    
- Risk neutral probabilities
    
The real-world probabilities (p and q) and risk-neutral probabilities (p̃ and q̃) are concepts commonly used in the pricing and valuation of financial derivatives, such as options, in the context of the binomial pricing model and other mathematical models. These probabilities serve different purposes and reflect different assumptions about the behavior of financial markets:

1. **Real-World Probabilities (p and q)**:
    - **p**: The real-world probability of an "up" movement in the underlying asset's price. It represents the actual likelihood of the asset's price increasing.
    - **q**: The real-world probability of a "down" movement in the underlying asset's price. It represents the actual likelihood of the asset's price decreasing.
    - These probabilities are based on the actual dynamics of the financial market, including factors like supply and demand, market sentiment, and economic conditions.
2. **Risk-Neutral Probabilities (p̃ and q̃)**:
    - **p̃**: The risk-neutral probability of an "up" movement in the underlying asset's price. It is an assumed probability used in derivative pricing models, such as the binomial model and the Black-Scholes model. The risk-neutral assumption is that investors are risk-neutral and do not require a risk premium for holding the derivative.
    - **q̃**: The risk-neutral probability of a "down" movement in the underlying asset's price. It complements p̃ to ensure that the probabilities sum to 1.
    - These probabilities are constructed to make the expected return on the derivative equal to the risk-free interest rate. In other words, they are chosen to simplify the pricing calculations and remove the risk premium.
    
$$
p̃ = \frac{1 + r - d}{u - d}\\
q̃  =  (1-p̃)

$$


The key difference between real-world probabilities and risk-neutral probabilities is the purpose they serve. Real-world probabilities reflect the actual dynamics and uncertainties in the financial markets, while risk-neutral probabilities are theoretical probabilities used for pricing and valuation purposes. The use of risk-neutral probabilities allows for a more straightforward pricing framework and simplifies the mathematics of derivative valuation.

In summary, real-world probabilities represent the actual market dynamics, while risk-neutral probabilities are theoretical assumptions used to simplify the pricing and valuation of financial derivatives, making it easier to calculate option prices and other derivative values.
    
- Risk premium and risk neutral assumption
    
**Risk-Neutral Assumption:**

The risk-neutral assumption is an assumption made in financial modeling, especially in option pricing, that investors are indifferent to risk when it comes to expected returns. Under this assumption, investors are considered to be risk-neutral, meaning they make investment decisions based solely on expected returns without factoring in their risk preferences.

In a risk-neutral world:

1. **Expected Returns:** Investors are only concerned with the expected returns of their investments.
2. **Risk Aversion:** Investors are assumed to have no risk aversion; they don't require additional compensation for taking on risk.
3. **Risk-Adjusted Discount Rate:** The discount rate used in financial models is the risk-free rate, reflecting the time value of money without any risk premium.

This assumption simplifies certain financial models and makes them more tractable mathematically, especially in the context of option pricing models like the Black-Scholes model.

**Risk Premium:**

A risk premium is the excess return expected by investors for taking on additional risk. It represents the compensation investors require for bearing the uncertainty and volatility associated with a particular investment. In the context of the Capital Asset Pricing Model (CAPM), the risk premium is the difference between the expected return of an investment and the risk-free rate.

The formula for the expected return (\(E(R)\)) of an investment under the CAPM is:

\[ E(R) = R_f + \beta \cdot (E(R_m) - R_f) \]

Where:

- \( R_f \) is the risk-free rate,
- \( \beta \) is the beta of the investment,
- \( E(R_m) \) is the expected return of the market.

The risk premium (\(E(R) - R_f\)) is a measure of the additional return required by investors for taking on systematic (market) risk. It quantifies the compensation for the risk that cannot be diversified away.

In summary, the risk-neutral assumption simplifies models by assuming that investors are indifferent to risk, while the risk premium reflects the extra return demanded by investors for bearing risk in reality.
    
- Pricing formula
    
$$
V_{0} = 1/{1+r} \left(p̃ \cdot V1_{up} + q̃ \cdot V1_{down}\right)
$$

- *V0* is the option price at time t=0.
- 1/1+*r* is the risk-free discount factor, which accounts for the time value of money.
- *p*~ is the risk-neutral probability of an up movement in the stock price.
- *V*1*up* is the option payoff at time t=1 in the case of an up movement in the stock price.
- *q*~ is the risk-neutral probability of a down movement in the stock price.
- *V*1*down* is the option payoff at time t=1 in the case of a down movement in the stock price.