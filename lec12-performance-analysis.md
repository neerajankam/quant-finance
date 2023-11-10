## **Performance Analysis**

## Risk decomposition framework

The variance of a security's return (i) can be expressed in terms of systematic and non-systematic risks as follows:

**Total Variance (σ²i) = Systematic Variance (σ²M) + Non-Systematic Variance (σ²E)**

$$
\sigma^2_i = (\beta_i \cdot \sigma_M)^2 + \sigma^2_E
$$

Where:

- **βi**: The security's beta
- **σ²i**: Total variance of the security's return.
- **σM**: Systematic variance, also known as market risk. It represents the part of the security's variance that is related to overall market movements and cannot be diversified away. Systematic risk affects all securities in the market.
- **σ²E**: Non-systematic variance, also known as unsystematic risk or idiosyncratic risk. It represents the part of the security's variance that is specific to the individual security and can be eliminated or reduced through diversification. Non-systematic risk is unique to each security and is not related to market movements.

In essence, the total risk (σ²i) of a security is composed of two components: the risk that is related to the overall market (systematic risk) and the risk that is specific to the security itself (non-systematic risk). Diversification across a portfolio of securities can help reduce non-systematic risk, leaving investors with exposure to systematic risk, which is inherent to the overall market.

## Indexes

Treynor's Index, Jensen's Index, and Sharpe's Index are commonly used performance measures for evaluating the performance of investment portfolios, particularly in the context of portfolio management and financial analysis. Here's an overview of each:

1. **Treynor's Index (Treynor Ratio):**
    - **Formula:** (Portfolio Return - Risk-Free Rate) / Portfolio Beta

    $$
    \text{Treynor Ratio (T)} = \frac{R_p - R_f}{\beta_p}
    $$

    Where:
    - *Rp*: Portfolio return.
    - *Rf*: Risk-free rate.
    - *βp*: Portfolio beta (systematic risk).

    - **Purpose:** The Treynor Ratio evaluates the risk-adjusted performance of a portfolio. It considers the excess return (return above the risk-free rate) per unit of systematic risk (beta). In other words, it measures how well the portfolio has performed given its level of market risk. A higher Treynor Ratio indicates better risk-adjusted performance.
    - **Use:** It is particularly useful for assessing the performance of portfolios with systematic risk exposure, such as those that are diversified but still sensitive to overall market movements.

2. **Jensen's Index (Jensen's Alpha):**
    - **Formula:** Portfolio Return - [Risk-Free Rate + Portfolio Beta * (Market Return - Risk-Free Rate)]

    $$
    \text{Jensen's Alpha (α)} = R_p - [R_f + \beta_p \times (R_m - R_f)]
    $$

    Where:
    - *Rp*: Portfolio return.
    - *Rf*: Risk-free rate.
    - *βp*: Portfolio beta (systematic risk).
    - *Rm*: Market return.

    - **Purpose:** Jensen's Alpha evaluates a portfolio's performance by comparing its actual return to its expected return based on the Capital Asset Pricing Model (CAPM). It quantifies how much the portfolio has outperformed or underperformed relative to its required rate of return, considering the risk-free rate, market return, and beta.
    - **Use:** It is used to determine whether a portfolio manager has added value (positive alpha) or underperformed (negative alpha) compared to what would be expected given the portfolio's risk.

3. **Sharpe's Index (Sharpe Ratio):**
    - **Formula:** (Portfolio Return - Risk-Free Rate) / Portfolio Standard Deviation

    $$
    \text{Sharpe Ratio (S)} = \frac{R_p - R_f}{\sigma_p}
    $$

    Where:
    - *Rp*: Portfolio return.
    - *Rf*: Risk-free rate.
    - *σp*: Portfolio standard deviation (total risk).

    - **Purpose:** The Sharpe Ratio evaluates the risk-adjusted return of a portfolio. It considers the excess return per unit of total risk, as measured by the portfolio's standard deviation. It quantifies how efficiently the portfolio has compensated investors for taking on additional risk.
    - **Use:** It is widely used to assess the trade-off between risk and return and helps investors compare different portfolios or investment strategies. A higher Sharpe Ratio indicates better risk-adjusted performance.

These performance measures help investors and portfolio managers assess the efficiency and risk-adjusted returns of investment portfolios, considering the level of risk taken and how it relates to the returns generated. Each of these indices provides a different perspective on portfolio performance and can be used in different investment contexts.

| Performance Measure | Good | Bad |
| --- | --- | --- |
| Treynor Ratio (T) | High value of T indicates good risk-adjusted returns, making it favorable. | Low value of T suggests that the portfolio hasn't generated sufficient returns given its systematic risk, making it less favorable. |
| Jensen's Alpha (α) | Positive alpha (α) suggests that the portfolio has outperformed its required rate of return based on CAPM, making it favorable. | Negative alpha indicates underperformance compared to what would be expected, making it less favorable. |
| Sharpe Ratio (S) | A higher Sharpe Ratio (S) implies better risk-adjusted returns, which is favorable. | A lower Sharpe Ratio indicates that the portfolio hasn't compensated investors adequately for the level of total risk taken, making it less favorable.

## Pricing formulae

### Price of a security using CAPM model

$$
S(0) = \frac{E[S(1)]}{1 + R + \beta (\mu_m - R)}
$$

Where:
- *S*(0) is the price of the security at time *t*=0.
- *E*[*S*(1)] is the expected price of the security at time *t*=1.
- *β* is the beta of the security.
- *μm* is the expected return of the market portfolio.
- *R* is the risk-free rate.

### Another formula using covariance

$$
S(0) = \frac{1}{{1 + R}} \left(E[S(1)] - \frac{1}{{\sigma_m^2}} \text{Cov}(S(1), M) \cdot (\mu_m - R)\right)
$$

Where:
- *S*(0) is the price of the security at time *t*=0.
- R is the discount rate or required rate of return.
- *E*[*S*(1)] is the expected price of the security at time *t*=1.
- *σm*2 is the variance of the market returns.
- Cov(*S*(1),*M*) is the covariance between the security's returns and the market returns.
- *μm* represents the expected return of the market portfolio
