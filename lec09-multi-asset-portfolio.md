## **Multi Asset Portfolio, Min.Variance Portfolio, Efficient Frontier & Min.Variance Line**

### **Multi asset portfolio**

A multi-asset portfolio can be expressed in terms of the following variables:

- \(x_i\): The number of shares or units of asset \(i\) held in the portfolio, where \(i\) can range from 1 to the total number of assets in the portfolio.
- \(S_i\): The price or value per share of asset \(i\).
- \(V\): The total value or investment in the portfolio.
- \(W_i\): The weight of asset \(i\) in the portfolio, which is typically calculated as the proportion of the value of asset \(i\) in the total portfolio value.

Here's how you can express a multi-asset portfolio using these variables:

1. **Value of Each Asset**: The value of each asset in the portfolio can be calculated as \(V_i = x_i \cdot S_i\), where \(i\) represents a specific asset.

2. **Total Portfolio Value**: The total value of the portfolio (\(V\)) is the sum of the values of all the assets in the portfolio, which can be expressed as \(V = \sum_{i=1}^{n} V_i\), where \(n\) is the total number of assets in the portfolio.

3. **Weights of Assets**: The weight of asset \(i\) in the portfolio (\(W_i\)) is calculated as the ratio of the value of asset \(i\) to the total portfolio value, expressed as \(W_i = \frac{V_i}{V}\).

4. **Portfolio Return**: The return of the portfolio (\(R_p\)) can be calculated as a weighted sum of the returns of individual assets. If \(K_i\) represents the return of asset \(i\), the portfolio return is given by

   \[R_p = \sum_{i=1}^{n} W_i \cdot K_i\]

5. **Portfolio Risk**: The risk or standard deviation of the portfolio (\(\sigma_p\)) is a function of the covariance between the returns of different assets in the portfolio and their respective weights. This can be expressed using the following formula:

   \[\sigma_p = \sqrt{\sum_{i=1}^{n} \sum_{j=1}^{n} W_i \cdot W_j \cdot \text{Cov}(K_i, K_j)}\]

   Where \(\text{Cov}(K_i, K_j)\) represents the covariance between the returns of asset \(i\) and asset \(j).

By using these variables and formulas, you can express and analyze a multi-asset portfolio in terms of \(x_i\), \(S_i\), \(V\), and \(W_i\), and calculate various portfolio performance metrics, such as return and risk.

### **Multi-asset portfolio using vectors and matrices:**

1. **Portfolio Return (\(R_p\))**: The portfolio return is calculated by taking a weighted sum of the expected returns of the individual assets. Each asset's expected return is multiplied by its weight in the portfolio and then summed up. This can be written as

   \[R_p = \vec{W} \cdot \vec{u}\]

   where \(\vec{W}\) is the vector of portfolio weights, and \(\vec{u}\) is the vector of expected returns for each asset.

2. **Portfolio Risk (\(\sigma_p\))**: The portfolio risk, often measured by the standard deviation, is a measure of the uncertainty or variability of the portfolio's returns. It is calculated using the portfolio weights, the covariance matrix (\(\vec{C}\)) of asset returns, and matrix multiplication. The formula for portfolio risk is

   \[\sigma_p = \sqrt{\vec{W}^\intercal \cdot \vec{C} \cdot \vec{W}\]

   where \(\vec{W}^T\) represents the transpose of the weight vector \(\vec{W\).

3. **Target Portfolio Expected Return (\(m\))**: The target portfolio expected return (\(m\)) is a predetermined goal or objective set by the investor. It represents the level of return that the investor seeks to achieve with the portfolio.

In summary, a multi-asset portfolio can be described by how it combines individual assets with their respective weights, expected returns, and risk considerations. The portfolio's expected return (\(R_p\)) is a weighted sum of expected asset returns, its risk (\(\sigma_p\)) considers the covariances between asset returns, and the target expected return (\(m\)) is the desired level of return for the portfolio.

### **MVP portfolio problem**

The minimum variance portfolio problem can be expressed as a constraint minimization problem using vectors. The goal is to minimize the portfolio variance subject to constraints on the portfolio weights. Here's how to formulate it:



Objective:
Minimize the portfolio variance subject to the following constraints.

\[
\min \sigma^2_p = \vec{w}^T \cdot \vec{C} \cdot \vec{w}
\]

1. **Weights Constraint**: The sum of the portfolio weights should equal 1 to represent a fully invested portfolio.

\[
\sum_{i=1}^n w_i = 1
\]

2. **Non-Negativity Constraint**: The weights of each asset should be non-negative.

\[
w_i \geq 0, \text{ for } i = 1, 2, \ldots, n
\]

3. **Target Return Constraint (Optional)**: You can also add a constraint on the expected return of the portfolio if you have a specific target return (\(m\)) in mind.

\[
\sum_{i=1}^n w_i \cdot \mu_i \geq m
\]

Where:

- \(n\) is the total number of assets in the portfolio.
- \(w_i\) is the weight of asset \(i\) in the portfolio.
- \(\mu_i\) is the expected return of asset \(i\).
- \(m\) is the target return for the portfolio.

**Formula to calculate MVP**

\[
\vec{w}_{\text{min-variance}} = \frac{1}{\vec{u}^T \cdot \vec{C}^{-1} \cdot \vec{u}} \cdot \vec{C}^{-1} \cdot \vec{u}
\]

### **Efficient Portfolio**

An optimal mix of investments that gives the best risk-return trade-off.

### **Efficient Frontier**

A graph showing all possible portfolios for different risk-return combinations, with those on the curve being the best choices.

![efficient frontier.png](https://prod-files-secure.s3.us-west-2.amazonaws.com/58c8d62c-66bc-4757-845d-1849a6bd8563/7ce16da2-2e11-46f4-b201-d73cd8769aa2/efficient_frontier.png)

### **Minimum Variance Line**

- *a*: This parameter represents the risk-free rate, denoted as \(R_f\). It reflects the expected return that an investor can earn without taking any risk. \(a\) is a scalar value that represents the risk-free rate.
- *b*: This parameter represents the coefficients that define the relationship between the expected return of the risky portfolio (often referred to as the market portfolio) and the standard deviation (risk) of the portfolio on the MVL. \(b\) is also a scalar value.

Together, \(a\) and \(b\) help determine the equation for the MVL, which describes the expected return of a portfolio as a linear combination of the risk-free rate (\(a\)) and the risk-return characteristics of the risky portfolio (\(b\) and \(\sigma_p\)).

The MVL equation is typically expressed as:

\[
\mu_p = a + b \cdot \sigma_p
\]