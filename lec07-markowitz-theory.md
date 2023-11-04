Here's the provided text formatted in markdown:

## **Markowitz Portfolio Theory**

Markowitz Portfolio Theory, developed by Harry Markowitz in the 1950s, is a widely recognized framework for constructing an efficient investment portfolio. This theory is a cornerstone of modern portfolio management and is based on the idea that investors can maximize returns for a given level of risk or minimize risk for a given level of returns by carefully selecting and diversifying a combination of assets in their investment portfolio.

**Key concepts and components of Markowitz Portfolio Theory include:**

- **Risk and Return**
    
    Markowitz recognized that investors care about both the expected return on their investments and the associated risk. In finance, risk is typically measured as the volatility or standard deviation of an asset's returns. The goal is to find a portfolio that offers the best trade-off between risk and return.
    
- **Efficient Frontier**
    
    Markowitz introduced the concept of the efficient frontier, which represents a set of portfolios that offers the maximum expected return for a given level of risk or the minimum risk for a given level of expected return. Portfolios that lie on the efficient frontier are considered optimal because they offer the best risk-return trade-off.
    
- **Diversification**
    
    One of the central ideas of the theory is diversification. By combining assets with low or negative correlations, investors can reduce portfolio risk without necessarily sacrificing returns. Diversification is a way to spread risk across different assets, which can help to mitigate the impact of poor performance in any single asset.
    
- **Covariance and Correlation**
    
    To quantify the benefit of diversification, Markowitz introduced the concepts of covariance and correlation. Covariance measures how two assets move together, while correlation standardizes this relationship, providing a number between -1 (perfect negative correlation) and 1 (perfect positive correlation).
    
- **Risk-Return Trade-Off**
    
    Markowitz Portfolio Theory shows that investors can choose portfolios with varying degrees of risk and return by adjusting the weight of each asset in their portfolio. As more assets are combined, risk can be reduced for a given level of expected return, or expected return can be increased for a given level of risk.
    
- **Optimal Portfolio**
    
    The optimal portfolio on the efficient frontier is the one that best suits an investor's risk tolerance and return objectives. Markowitz's theory provides a mathematical framework to determine this optimal portfolio based on individual preferences.

Markowitz Portfolio Theory is a fundamental concept in modern finance and is the basis for many investment strategies and financial models, such as the Capital Asset Pricing Model (CAPM). It has helped investors and portfolio managers better understand the trade-offs between risk and return, leading to the development of diversified and well-balanced investment portfolios.

**Return:**

$$
\text{Expected Return} = \frac{E(S(T)) - S(0)}{S(0)}
$$

- **E(S(T))** represents the expected future value of the investment at time *T*.
- **S(0)** represents the initial price at time *t*=0.

**Risk:**

$$
\text{Var}(K) = E((K - E(K))^2) \\
\text{SD}(K) = \sqrt{\text{Var}(K)}
$$

**Weights:**

$$
W_1 = \frac{x_1 \cdot S_1}{V(0)} \\
W_2 = \frac{x_2 \cdot S_2}{V(0)}
$$

- *W*1 and W2 represent the weights of securities 1 and 2 in the portfolio, respectively.
- *x*1 and x2 are the number of shares of securities 1 and 2, respectively.
- *S*1 and S2 are the prices of security 1 and security 2, respectively.
- *V*(0) is the total initial investment.

**Expected Value of a Portfolio:**

$$
E(K_v) = W_1 \cdot E(K_1) + W_2 \cdot E(K_2)
$$

- *E*(*Kv*) is the expected value of the portfolio.
- *W*1 and W2 are the weights of the two assets in the portfolio.
- *E*(*K*1) and E(K2) are the expected returns of the two assets.
- *K*1 and K2 are the returns of the two assets.

**Calculating the Expected Value of a Portfolio Taking into Account Different Economic Outlooks:**

$$
E(K_v) = P_{\text{recession}} \cdot [W_1 \cdot E(K_1)_{\text{recession}} + W_2 \cdot E(K_2)_{\text{recession}}] \\

+ P_{\text{stagnation}} \cdot [W_1 \cdot E(K_1)_{\text{stagnation}} + W_2 \cdot E(K_2)_{\text{stagnation}}] \\

+ P_{\text{boom}} \cdot [W_1 \cdot E(K_1)_{\text{boom}} + W_2 \cdot E(K_2)_{\text{boom}]
$$
