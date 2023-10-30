# Lec 03: Introduction to Options

## Options

Options are derivative contracts that give the holder the right, but not the obligation, to buy or sell an asset at a predetermined price and date in the future. They are widely traded in financial markets and are used for various purposes, including speculation, hedging, and income generation.

### Types

#### American Options

An American option gives the holder the right to buy or sell an underlying asset at a predetermined price, known as the strike price, at any time before the expiration date of the option. The holder has the flexibility to exercise the option at their discretion.

#### European Options

A European option gives the holder the right to buy or sell an underlying asset at a predetermined price, known as the strike price, only on the expiration date of the option. The holder can exercise the option only at the expiration date.

### Why Are They Traded?

Options are traded for several reasons. First, they provide a way for investors and traders to speculate on the price movements of underlying assets without owning the assets themselves. Options allow for leveraged positions, enabling traders to potentially earn higher returns with a smaller upfront investment.

Second, options are used for hedging purposes. Investors can use options to protect their portfolios against adverse price movements. For example, if an investor holds a large number of shares of a company and expects the stock price to decline, they can purchase put options as a form of insurance. If the stock price does indeed fall, the put options will offset the losses on the stock holdings.

Lastly, options can be used for income generation. By selling options, investors can collect premiums and earn income. This strategy, known as writing options, involves taking on the obligation to buy or sell the underlying asset if the option buyer exercises their rights.

Overall, options are traded to speculate on price movements, hedge against risk, and generate income. They provide flexibility and opportunities for profit in various market conditions.

Please note that options trading involves risks, and individuals should have a good understanding of options before engaging in trading activities.

### Call Options

A call option is a type of financial contract that gives the holder the right, but not the obligation, to buy an underlying asset at a predetermined price (strike price) within a specific time period. The buyer of a call option expects the price of the underlying asset to rise, allowing them to profit from the increase.

For example, let's say an investor purchases a call option on Company XYZ stock with a strike price of $50 and an expiration date of one month. If the stock price rises above $50 during that month, the investor can exercise the call option and buy the stock at the predetermined price. They can then either hold the stock or sell it at a higher market price, generating a profit.

The payoff for a call option in terms of t (current time), T (expiration time), S (spot price), and K (strike price) can be represented by the following formula:

Payoff = max(S(T) - K, 0)

Where:

- S(T) represents the spot price at time T (expiration time)
- K represents the strike price

This formula calculates the positive difference between the spot price at expiration and the strike price. If the spot price is higher than the strike price, the call option has value and the payoff is the difference between the two prices. If the spot price is lower than the strike price, the call option has no value and the payoff is zero.

### Put Options

A put option is another type of financial contract that gives the holder the right, but not the obligation, to sell an underlying asset at a predetermined price (strike price) within a specific time period. The buyer of a put option expects the price of the underlying asset to decline, allowing them to profit from the decrease.

Continuing with the example above, let's say an investor purchases a put option on Company XYZ stock with a strike price of $50 and an expiration date of one month. If the stock price falls below $50 during that month, the investor can exercise the put option and sell the stock at the predetermined price. This allows them to protect their investment or potentially profit from the decline in the stock price.

Call and put options provide investors with the opportunity to benefit from price movements in the underlying asset without actually owning the asset itself. They can be used for various investment strategies, including speculation, hedging, and income generation.

It's important to note that options trading involves risks, and individuals should have a good understanding of options and their associated risks before engaging in trading activities.

### Vanilla and Exotic Options

Vanilla options are based on stocks and bonds as underlying assets.

Exotic options are based on assets other than stocks and bonds.

Options can be used to create different investment strategies based on the type of asset they are derived from.
