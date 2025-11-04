# List your coin

The structure of the repository speaks for itself. Create a pull request to add your coin, using exactly the same format as for $PING, including:

1.	All fields in the JSON file are mandatory.
2.	The thumbnail must be named after the coin's lowercase symbol, have a resolution of 512×512, and be a compressed PNG.
3.	The pool must have sufficient (locked) liquidity.
4.  The pool must be a Uniswap v3 or v4 pool.

Even if the formatting is correct, there is no guarantee that your pull request will be accepted. Additionally, after the merge, some manual effort will be required to whitelist your coin onchain.

## Why?

Check [c402.markets](https://c402.markets) once it’s live. In short, c402 coins are minted with USDC. When they sell out, the USDC is used to purchase the qoute coin specified at creation, and liquidity is then provided for that pair. The paired token must be chosen from this list.

**Example:** Someone creates a c402 coin named $COIN and selects $PING as its quote token. Once the c402 coin sells out, all USDC raised will be used to purchase $PING through the configured pool. Liquidity for the $COIN/$PING pair will then be added and locked.
