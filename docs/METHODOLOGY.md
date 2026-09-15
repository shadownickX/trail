# Methodology and evidence boundaries

TRAIL turns a chain of public observations into a research view. This document defines what each observation means and, just as importantly, what it does not prove.

## Event definitions

### Qualifying sale

A transaction in which the tracked wallet disposes of the source token through a recognized trading path. A plain wallet-to-wallet token transfer is not classified as a sale.

### Qualifying next purchase

The first recognized purchase made by the same wallet after its qualifying source-token sale. A token received through an ordinary transfer, distribution, or unsupported route is not automatically classified as a purchase.

### Still holding

The wallet has a positive observable balance at the result block. This does not describe cost basis, control of other wallets, hedges, or offchain exposure.

## Relationship labels

### Direct transfer

At least one direct onchain asset transfer is observed between the selected buyer and destination deployer.

This proves that a transfer occurred. It does not, by itself, prove shared ownership or coordination.

### Shared funding source

Both addresses received funds from the same observable source within the configured search rules.

This can indicate common provenance, but exchanges, relayers, bridges, and widely used funding services can create legitimate overlaps.

### Same fee recipient

Two or more launches resolve to the same recorded fee recipient.

This is a launch-level relationship worth inspecting. It does not automatically establish that every deployer is the same person.

## Concentration

TRAIL separates:

- deployer-held supply;
- supply held by the selected linked-wallet group;
- total visible concentration of that selection.

These values must always include the block or timestamp used. They should not be presented as current after the observation has aged.

## Fees

Base trading fees and creator tax are separate fields. A combined percentage can be shown as a convenience only when both components and their sources remain visible.

## Coverage

Every result should disclose:

- source token and destination token;
- lookback window;
- block range;
- data providers or contracts queried;
- unsupported or failed sources;
- last refresh time;
- whether history was complete, partial, or unavailable.

## Interpretation rules

- A connection is an observation, not a verdict.
- No detected connection does not prove independence.
- A popular destination does not imply a profitable destination.
- Multiple rotating wallets can still be controlled by one actor.
- Historical deployer behavior can inform research but cannot guarantee future behavior.

## Example data

Numbers and addresses displayed in documentation graphics are illustrative unless a capture explicitly names its block, source, and timestamp.
