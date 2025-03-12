# UCM

The **Universal Content Marketplace (UCM)** is a protocol on the permaweb designed to enable the **trustless exchange of atomic assets**. It empowers creators and users to trade and transact with digital content, ranging from images and music to videos, papers, components, and even applications.

## How it works

The UCM functions by accepting a deposit from a buyer or seller and fulfilling orders based on the swap pair, quantity, and possibly price that are passed along with the deposit. UCM allows creators and users to trade and transact with any form of digital content. Here is a list of actions that take place to complete a UCM order.

1. A user deposits (transfers) their tokens to the UCM. The user will also have to add additional tags to the **Transfer Message** which are forwarded to the UCM process and will be used to create the order.
2. The token process issues a **Credit-Notice** to the UCM and a **Debit-Notice** to the user.
3. The UCM **Credit-Notice Handler** determines if the required tags are present in order to create the order.
4. The UCM uses the forwarded tags passed to the **Transfer Handler** to submit an order to the orderbook. The order creation input includes the swap pair to execute on, as well as the quantity of tokens and price of tokens if the order is a limit order.

A key feature of UCM is its incentivizing token, PIXL. Users who purchase atomic assets via UCM can earn [PIXL](https://bazar.arweave.net/#/asset/DM3FoZUq_yebASPhgd8pEIRIzDW6muXEhxz5-JwbZwo) tokens, by maintaining **buying streaks** (purchasing one or more atomic assets on consecutive days).

#### Core Functionality

- **Powered by AO**: The UCM now runs on AO, a hyper-parallel computing system built on the Arweave network. AO offers a unified environment for executing decentralized applications and processes.
- **Trustless Transactions**: UCM eliminates the need for third-party intermediaries in transactions.
- **Licensable Data**: The [Universal Data License](https://udlicense.arweave.net/) (UDL) ensures that value flows equitably to creators and contributors on the permaweb. This standard framework allows creators to set their own terms for the usage of content they upload. Learn more about UDL [here](https://ao-bazar.arweave.net/#/docs/creators/universal-data-license).
- **Earn $PIXL Rewards**: The UCM protocol rewards users with PIXL tokens for maintaining a buying streak. The longer the streak, the larger the daily PIXL rewards! Learn more about earning PIXL [here](https://ao-bazar.arweave.net/#/docs/collectors/earn-pixl).

## UCM Fees

The UCM captures a **0.5% fee** per transaction. If the trade involves $wAR tokens, the fee is used to purchase PIXL tokens as follows:

1. The contract buys available PIXL sell orders.
2. If no sell orders exist, it initiates a “Buy” order through a **reverse Dutch auction**.
3. PIXL tokens purchased through this process are **burned**, reducing the overall supply

Higher trading volumes and fees result in more tokens being purchased and burned, increasing PIXL scarcity. See the PIXL tokenomics [here](https://bazar.arweave.net/#/docs/collectors/earn-pixl)

## Links

- [UCM source code](https://github.com/permaweb/ao-ucm).
- [Bazar (UCM UI)](https://bazar.arweave.net/#/)
