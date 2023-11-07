## **Minimum Variance Line Continued, Market Portfolio**

- Two fund theorem
    
    Two-Fund Theorem can be applied to portfolios that lie on the Minimum Variance Line (MVL) in the context of the Capital Market Line (CML). Here's how you can express it:
    
    1. **Portfolios on the MVL:** Portfolios that lie on the MVL are efficient portfolios with the minimum possible risk for a given level of return. The MVL represents the set of efficient portfolios that provide the best risk-return trade-offs.
    2. **Two Key Portfolios:**
        - **Risk-Free Asset (Fund 1):** The first fund is a risk-free asset, often represented by government bonds. It has a fixed return, which is the risk-free rate, denoted as (Rf).
        - **Market Portfolio (Fund 2):** The second fund is the market portfolio, which is a diversified portfolio containing all risky assets. It represents the entire universe of risky investments.
    3. **Weights and the Two-Fund Theorem:** For portfolios on the MVL, the Two-Fund Theorem still holds. You can express any portfolio on the MVL as a combination of the risk-free asset and the market portfolio.
        
        $$
        \mu_p = W_f \cdot R_f + (1 - W_f) \cdot \mu(\text{Market Portfolio})
        $$
        
    
    This formula demonstrates that, for portfolios on the MVL, you can achieve any expected return by adjusting the weight assigned to the risk-free asset while using the market portfolio as the second fund. It's a practical application of the Two-Fund Theorem in the context of efficient portfolios along the MVL.
    
    - **μp**: This represents the expected return of a portfolio on the Minimum Variance Line (MVL). It's the average rate of return that you can expect to earn from this portfolio.
    - **Wf**: This is the weight assigned to the risk-free asset in the portfolio. It indicates what proportion of your portfolio is invested in a risk-free asset, often represented by government bonds.
    - **Rf**: This is the risk-free rate, which is the fixed return you can earn from the risk-free asset. It serves as a benchmark for a safe, guaranteed return on your investment.
    - **(1 - Wf)**: This part of the formula represents the weight assigned to the market portfolio, which is a diversified portfolio containing all risky assets available in the market. It's complementary to the weight of the risk-free asset.
    - **μ(Market Portfolio)**: This is the expected return of the market portfolio, which represents the average return you can expect from investing in a diverse set of risky assets available in the market.

![Efficient-frontier-new(2).jpeg](https://prod-files-secure.s3.us-west-2.amazonaws.com/58c8d62c-66bc-4757-845d-1849a6bd8563/ead0656b-d958-498b-a065-33a4a902b152/Efficient-frontier-new(2).jpeg)

https://www.wallstreetmojo.com/market-portfolio/

![Market-Portfolio.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/58c8d62c-66bc-4757-845d-1849a6bd8563/a0a6be2d-dc86-4e7c-b74a-ed0d09fac3b9/Market-Portfolio.png)

$$
\text{Market Portfolio: } \left( \mu_M, \sigma_M \right)
$$

- *μM* represents the expected return of the market portfolio.
- *σM* represents the standard deviation (volatility) of the market portfolio.

$$
\vec{W_m} = \frac{\vec{C}^{-1} \cdot (\vec{m} - R_f \cdot \vec{u})}{\vec{u}^\intercal \cdot \vec{C}^{-1} \cdot (\vec{m} - R_f \cdot \vec{u})}
$$

- *Wm*: This represents the weight vector of the market portfolio.
- *m*: This is the vector of all asset returns.
- *C^*−1(det C ≠ 0): It is the inverse of the covariance matrix of asset returns.
- *Rf*: This is the risk-free rate.
- *u:* This is a vector consisting of all 1s.