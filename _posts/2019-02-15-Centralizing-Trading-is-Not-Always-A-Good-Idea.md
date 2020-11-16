---
layout: post
title: "Centralizing is not always good for trading"
description: "From the observed enormous amount of volume traded within exchanges each day, another huge chunk of the volume is traded within market agents, not near any centralized exchange. These contracts are known as over-the-counter (OTC), although there are technologies and space for a lot of them to become standard tradable products, that's not always the optimal solution."
keywords: "over-the-counter, trading, microstructure, financial-markets, markets, electricity-markets"
---

### An Over-the-Counter Example

##### ~ 8 minutes reading time article | [Original LinkedIn Article](https://www.linkedin.com/pulse/always-centralizing-good-trading-why-otc-still-persists-gruber)

-----------------------

From the observed enormous amount of volume traded within exchanges each day, another huge chunk of the volume is traded within market agents, not near any centralized exchange. These contracts are known as over-the-counter (OTC), although there are technologies and space for a lot of them to become standard tradable products, that's not always the optimal solution.

Centralization in trading, for the most part, has provided more benefits than anything, providing more auditing control to authorities and liquidity to other market agents. It would be the only natural to try to centralize negotiations of certain securities that have remained OTC-only for decades, for very good reasons, [as agents of the market themselves tried to tell regulators back in 2007](https://www.thestreet.com/story/904680/1/new-age-securities-firms-to-testify-against-central-limit-order-book.html).

The initial idea was called Centralized Limit Orderbook (Or *CLOB* for short), which means a single order book for that instrument measures and informs price for all market participants simultaneously, standardizing products that were distant from exchanges in multiple aspects directly to the already implemented format for how all securities are currently traded.

### An example of a classical ‘LOB’ price formation process
![example-lb](https://media-exp1.licdn.com/dms/image/C4E12AQHJqePwbpi4vg/article-inline_image-shrink_1000_1488/0?e=1611187200&v=beta&t=jmcVuw4qq75ANHAUFZ4k0PEjVNMDRTuDCWeXUXzF6aw)

This means all players observing Trader n interact with the market can be considered a price of reference because, in a normal exchange, all institutions assume that both trader and counterpart have no credit risk associated with this particular trade, the weight of the trade is uniform. This changes when institutions need to price counterparty risk, most commonly found in OTC products. They change the price for each counterpart based on its risk assessment of that trade since they’ll have to charge more or less for the risk they’re exposed[1] – the same way you’d charge a higher premium for an option with a higher volatility expectancy in a vanilla option. They trade using RFQ’s, or, “Requests for quotes” – to this day, banks still trade OTC contracts through RFQ’s when credit risk is involved directly or indirectly, and when asked on how the market predicts its future developments and possible technological advances, instead of saying the migrating towards a CLOB ‘direction’ would be ideal, they say the complete opposite: they’d expect a more synchronous and efficient process of RFQ - even continuous in some sort, instead of manually calling or pricing through a terminal using chats[2].

This may seem like traders being "lazy" to adapt to new changes or trying to stick themselves to the “old-school known system" like equity traders did, except this time, they're right.

### A *“request for quote”* simplified diagram 
![rfq-diagram](https://i.imgur.com/yCSxiBE.png)

Not all markets and instruments can be traded through clearing exchanges, forcing all trading parties to go OTC environment, where pricing counterparty risk is an important component of the price formation process: creating bilateral contracts that also prices risk complements to the market maker essential information on how much it should charge for its services to each counterpart. Standard future contracts in exchanges do not have this property because they’re obliged to be multilateral, while OTC markets rely on contract customized pricing and thus this process cannot be transferred to an order-book.

## What if it did succeed, and OTC's became a unified LOB?

 A *‘CLOB’* results on credit risk not being able to be priced in, even when knowingly for all market participants, resulting in a serious hinder to the price formation process. If participants set risk parameters of some sort, they’d automatically remove the principle of FIFO (First in First Out principle applied to LOB's), since you want to be able to skip the defaulting counterpart as your other side of the trade, in other words, this defeats the purpose of a limit order book: price discovery, consequently, trust in the price traded by the agents, even tho there’s only one last price and the book assumes that credit is uniform for the price at that moment and at the same time is not uniform for the participant market agents.

### An example of a CLOB with visible credit risk
![rfq-diagram](https://i.imgur.com/0R2LZTd.png)

##### *(Risk expressed as [0,1] of default probability in percentage)*

The whole purpose of being able to negotiate evenly credit-wise with all your counterparts regardless of their behavior is the notion of value agreement. This does not hold when you are obligated to both prices the security itself and the possibility of your counterpart being risk-oriented based on a single uniform price. Even with hidden risk values/names, the price discovery price becomes distorted due to this asymmetric price formation process to the point where if anyone uses this price as reference, especially bid/ask, it’d be misleading depending on who is analyzing that quote, exposing intermediary and high-credit institutional traders to aggressive bidding of speculative low-credit traders that fill unrealistic prices in the hopes of finding a counterpart to your trades.

OTC traders understand that certain types of contracts will be not only negotiable in terms of customization because they can’t fill a single custom contract, they also understand their exposition to a distorted price formation process, results of the greediness of intermediary traders trying to achieve better prices using risky counterparts as their execution prices. This process also raises the risk of those indirectly exposed to those low-credit agents which increases the system risk as a whole and affects negatively all institutional traders, for those adopting the CLOB mechanism or not. This 'tail risk' is not an imminent threat because there are only a few examples of similar trading structures in real markets. When similar systems were implemented on European wholesale spot energy markets, they went far to ensure margin for this kind of operation that limits most of participants actions, and as a consequence, most were left out, since energy trading contracts is widely considered one of the most volatile contracts in the world and would require unpractical margins for centralized trading. [This is one of the reasons why a lot of European energy trading volume is still traded through OTC](https://ec.europa.eu/energy/sites/ener/files/documents/quarterly_report_on_european_electricity_markets_q2_2018.pdf) (Page 14, Figure 16), for example. [New solutions have been urgently called by both regulators and exchanges alike](https://www.fisglobal.com/solutions/institutional-and-wholesale/-/media/fisglobal/files/brochure/the-state-of-short-term-power-trading-in-europe.pdf), but as long this asymmetry persists on how the price is perceived by traders, it'll probably take some time until we get there.

### References:

> 1. Gregory, Jon (7 September 2011), Counterparty Credit Risk: The new challenge for global financial markets, John Wiley & Sons, p. 448
> 2. Lehalle and Laruelle, (2017). Market microstructure in practice: 2nd edition, World Scientific, p. 9

### Disclaimer:
>  European, American or Brazilian laws specific to trading behavior or practices were not considered. This is a theoretical approach to a hypothetical micro-structure model.

