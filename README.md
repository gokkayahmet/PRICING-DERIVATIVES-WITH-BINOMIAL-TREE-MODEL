# PRICING DERIVATIVES WITH BINOMIAL TREE MODEL
## Exersice via Python


The binomial tree model is a commonly used approach for pricing derivatives, such as options. The basic idea behind the model is to create a tree of possible stock prices over time, based on a set of input parameters


The binomial tree model is a commonly used approach for pricing derivatives, such as options. The basic idea behind the model is to create a tree of possible stock prices over time, based on a set of input parameters. By working backwards through the tree, we can calculate the fair value of the derivative at each node, and ultimately arrive at a price for the derivative at the current time.

The key inputs to the binomial tree model are:

$$\boldsymbol{The\ current\ stock\ price (S0)}$$

$$\boldsymbol{The\ volatility\ of\ the\ stock (σ)}$$

$$\boldsymbol{The\ risk-free\ interest\ rate\ (r)}$$

$$\boldsymbol{The\ time\ to\ maturity\ of\ the\ derivative\ (T)}$$

$$\boldsymbol{The strike price of the derivative (K)}$$

$$\boldsymbol{The\ number\ of\ time\ steps\ in\ the\ tree\ (n)}$$




Using these inputs, we can construct the binomial tree by calculating the possible stock prices at each node in the tree, using the following formulas:

$$\boldsymbol{The\ up\ factor\ (u)\ is\ calculated\ as\ e^(σ * sqrt(dt)),\ where dt = T/n}$$

$$\boldsymbol{The\ down\ factor\ (d)\ is\ calculated\ as\ 1/u}$$

$$\boldsymbol{The\ probability\ of\ an\ up\ move\ (p)\ is\ calculated\ as\ (e^(r*dt) - d) / (u - d)}$$

$$\boldsymbol{The\ probability\ of\ a\ down\ move\ (1-p)\ is\ simply\ 1-p}$$


Once we have constructed the binomial tree, we can work backwards through the tree to calculate the fair value of the derivative at each node, using the following formulas:

$$\boldsymbol{For\ a\ call\ option,\ the\ option\ value\ at\ a\ given\ node\ is\ Max(S-K, 0)}$$

$$\boldsymbol{For\ a\ call\ option,\ the\ option\ value\ at\ a\ given\ node\ is\ Max(S-K, 0)}$$

$$\boldsymbol{For\ a\ call\ option,\ the\ option\ value\ at\ a\ given\ node\ is\ Max(S-K, 0)}$$


By working backwards through the tree in this way, we can calculate the fair value of the derivative at the current time, which is the price we would expect to pay to enter into the derivative contract.

Overall, the binomial tree model provides a relatively simple and intuitive way to price derivatives, and can be extended to handle more complex instruments, such as American options, which can be exercised at any point prior to expiration.


