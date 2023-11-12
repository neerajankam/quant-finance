## **Futures, Options and Put Call Parity**

## Marking to market - futures
    
Marking to Market, in the context of futures trading, is the daily process of adjusting the futures contract price to reflect its current market value. This adjustment is made based on the changes in the market price of the underlying asset and ensures that the futures contract is accurately valued at the end of each trading day. The marking to market process typically involves comparing the current futures price, denoted as f(n, T), to the previous day's futures price, denoted as f(n-1, T).

Here's how marking to market works for both long and short positions:

1. **Long Position (Buyer)**:
    - For a trader with a long (buy) futures position, marking to market involves updating the value of the contract to reflect the current market conditions.
    - The daily change in the futures price is calculated as f(n, T) - f(n-1, T).
    - If the futures price has increased, the trader's contract value has also increased, resulting in a profit.
    - If the futures price has decreased, the contract value has decreased, resulting in a loss.
2. **Short Position (Seller)**:
    - For a trader with a short (sell) futures position, marking to market similarly involves updating the contract's value to reflect the current market conditions.
    - The daily change in the futures price is calculated as f(n, T) - f(n-1, T).
    - If the futures price has increased, the contract value has decreased, resulting in a loss for the short seller.
    - If the futures price has decreased, the contract value has increased, resulting in a profit for the short seller.

Marking to market ensures that traders are aware of their daily profit or loss and that margin requirements are adjusted accordingly. It helps maintain the integrity of the futures market by ensuring that traders have sufficient funds to cover potential losses.

## Futures - related terms
1. **Margin**:
    - **Initial Margin**: When you open a futures position, you are required to deposit an initial amount of money, known as the initial margin, with your broker. This margin serves as collateral and ensures that you have the financial capability to cover potential losses in your position.
    - **Maintenance Margin**: After opening a position, you must maintain a certain minimum account balance, known as the maintenance margin. If the value of your account falls below this level due to adverse price movements, you may receive a margin call.
2. **Margin Call**:
    - A margin call is a notification from your broker that your account balance has fallen below the maintenance margin level. It is a request for you to deposit additional funds into your account to bring it back up to the required level. Failure to meet a margin call may result in the liquidation of your futures position to cover potential losses.
3. **Leverage**:
    - Leverage allows traders to control a larger position with a relatively small amount of capital. It is a characteristic of futures trading where a small margin deposit can control a much larger contract value. While leverage can amplify profits, it also increases the potential for losses.
4. **Contract Size**:
    - The contract size refers to the standardized quantity of the underlying asset in a futures contract. It varies depending on the type of futures contract, and traders should be aware of the specific contract size for the assets they are trading.
5. **Settlement Price**:
    - The settlement price is the final price at which a futures contract is settled, typically at the end of the trading day. It is used to calculate profits and losses for the day.
6. **Open Interest**:
    - Open interest is the total number of outstanding futures contracts for a particular asset. It provides insights into market sentiment and potential liquidity.
7. **Hedging**:
    - Hedging is a strategy where traders use futures contracts to offset the risk of price movements in the underlying asset. It is often employed by businesses and investors to protect against adverse price changes.
8. **Delivery and Cash Settlement**:
    - Some futures contracts can result in physical delivery of the underlying asset, while others are settled in cash. Cash settlement means the profit or loss is paid in cash, and no physical delivery of the asset occurs.
9. **Expiration Date**:
    - The expiration date is the date on which a futures contract matures and is no longer tradable. At this point, traders must close their positions or roll them over to a new contract.
10. **Tick Size**:
    - The tick size is the minimum price movement allowed in a futures contract. It varies by contract and is important for determining profit and loss.
11. **Long and Short Positions**:
    - A long position is when a trader buys a futures contract, expecting the price to rise.
    - A short position is when a trader sells a futures contract, expecting the price to fall.
12. **Marking to Market**:
    - Marking to market is the daily process of adjusting the futures contract's value based on the current market price. It helps determine margin requirements and ensures that accounts have adequate funds to cover potential losses.
## Put-call parity

Put-Call Parity is a fundamental principle in options pricing, especially for European-style options. It establishes a relationship between the prices of European call and put options with the same strike price and expiration date, in the context of a risk-free and dividend-free underlying asset. Put-Call Parity ensures that options with equivalent terms must have prices that are in balance with each other.
    
The Put-Call Parity formula for European options is as follows:

$$
C^E - P^E = S(0) - \frac{X}{e^{rT}}
$$
  
If dividends:

$$
C^E - P^E = S(0) - \frac{X}{e^{rT}}+ \frac{D}{e^{rT}}
$$

- *CE* = Price of a European call option
- *PE* = Price of a European put option
- *S*(0) = Initial price of the underlying asset
- *X* = Strike price of the options
- *e* = The base of the natural logarithm (approximately 2.71828)
- *r* = Risk-free interest rate
- *T* = Time to expiration
- *D* = Total dividends expected to be paid during the option's lifespan

The Put-Call Parity formula essentially states that the combined cost of buying a European call option and investing in risk-free bonds (with the present value of the strike price as the principal amount) should be equal to the cost of buying a European put option and the current price of the underlying asset.

Here's how Put-Call Parity works:

1. If the left side of the equation (buying a call option and investing in bonds) is cheaper than the right side of the equation (buying a put option and the asset), there is an arbitrage opportunity, and traders can take advantage of it.
2. Conversely, if the left side is more expensive than the right side, there is another arbitrage opportunity, and traders can capitalize on it.

Put-Call Parity ensures that options with identical terms are priced correctly relative to each other. Any deviation from the parity relationship can trigger arbitrage activities, which, in turn, should bring the options back into alignment.

In practice, Put-Call Parity is a valuable tool for options traders and market participants to evaluate the fairness of option prices and identify trading opportunities when pricing discrepancies arise. It is important to note that Put-Call Parity assumes an idealized market with no transaction costs, taxes, or dividends, and it specifically applies to European-style options due to their exercise characteristics.