---
title: Auction and Market Designs
---


## Market and Auction Design and Structure

#### Alpha

We will keep the alpha part as is for now. We do not want to impose a new format on bidders as given
our small size might mean being ignored. The only change is the restriction of gas to 25MM. (The
rest goes to the beta market).

#### Beta

We will go with a discriminatory auction first. It is understood though that we adapt the auction
format depending on (i) feedback by potential bidders and (ii) actual behavior in the market.

We will restrict the residual claim only to full bids for now. To avoid too small token allocations
that are then practically of no use. Also note that in the case of a secondary market, this issue
might be less important.

The main reasons are:

- Simple and familiar format
- In principle compatible with a secondary market
- But first and foremost: Want to get feedback from bidders how they bid.

#### Contingencies

0. Depending on the step bidding, we increase the token size.
1. If we observe bidding on whole blocks only (or close to it), we can simplify the whole setup
   dramatically.
2. If we observe upward sloping demand curves, we might need to change the format completely.

### TODO Secondary market

- Market running after primary allocation took place
- Need to think whether we should provide the marketplace ourselves
  - In principle could be handled by external parties
  - But the interlocking of different markets (that the timing of spot market and secondary market
    is making sense\*\* is probably relevant and easier to orchestrate by us
- The main purpose of this market is to account for information differences over time - builders
  might realize they cannot fill a block; or they might need more space
- The base fee is not known at the time of the primary market; so there should be updates regarding
  the base fee happening with before-strike-time blocks being minted. This also affects the initial
  pricing we offer.