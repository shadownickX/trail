# Data model

The core model is a directed, time-ordered evidence graph.

## Nodes

- wallet;
- source token;
- destination token;
- deployer;
- funding source;
- fee recipient;
- launch.

## Edges

- sold token;
- next qualifying purchase;
- direct transfer;
- funded by;
- deployed by;
- pays fees to;
- still holds, added, or exited.

Every derived edge carries source transaction or event references, observation time, block range, and coverage status. An edge records what was observed, not who legally controls an address.
