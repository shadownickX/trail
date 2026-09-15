# TRAIL product specification

## One-line promise

Paste a token. See what its sellers bought next, then inspect how those buyers connect to the next token's deployer.

## User moment

TRAIL is designed for the moment a trader notices wallets leaving a token and needs to decide what deserves attention next. Today that investigation is fragmented across transaction explorers, holder tables, deployer histories, and fee metadata. TRAIL keeps the sequence intact.

## Primary flow

1. The user enters a source-token contract address.
2. The user selects a lookback window.
3. TRAIL resolves qualifying sales during that window.
4. It follows each seller to the next qualifying purchase.
5. It groups destination tokens and calculates participation and purchase totals.
6. The user opens a destination token to inspect its launch participants.
7. TRAIL shows observations, provenance, coverage, and uncertainty.

## Core result model

### Rotation row

| Field | Meaning |
| --- | --- |
| Destination token | Token purchased after the source-token sale |
| Buyers after exit | Unique source-token sellers that later bought the destination |
| Linked buyers | Buyers with at least one selected observable relationship to the destination deployer |
| Combined buys | Sum of qualifying destination purchases by the rotating cohort |
| Last purchase | Most recent qualifying purchase time |
| Still holding | Buyers with a positive observable balance at the result block |
| Creator tax | Creator tax reported separately from the base fee |
| Coverage | Sources queried, block range, completeness, and failures |

### Expanded evidence card

- ordered source sale and destination purchase;
- buyer and deployer addresses;
- direct transfers between buyer and deployer;
- shared observed funding sources;
- fee-recipient reuse across launches;
- deployer's previous observed launches;
- deployer and selected-cohort supply concentration;
- current buyer continuation state;
- source timestamps and block references.

## Product principles

1. **Sequence before score.** Preserve the order of events.
2. **Purchases before transfers.** Receiving a token is not automatically a buy.
3. **Evidence before identity.** Label the observed relationship, not an inferred owner.
4. **Coverage before confidence.** Missing data must be visible.
5. **No universal SAFE badge.** Users should see why a result deserves attention.

## Out of scope for the first release

- executing trades;
- importing private keys;
- declaring token safety;
- proving wallet ownership;
- price prediction;
- guaranteed latency before measurement.
