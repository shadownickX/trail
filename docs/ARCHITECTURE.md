# Architecture

TRAIL preserves the route from raw chain activity to a reviewable observation.

1. **Chain ingestion** normalizes blocks, transactions, logs, and launch metadata.
2. **Event classification** distinguishes qualifying trades from ordinary transfers.
3. **Rotation sequencing** follows each seller forward to the next qualifying purchase.
4. **Relationship analysis** attaches deployer, funding, and fee-recipient observations.
5. **Storage** retains provenance, coverage, and deterministic query snapshots.
6. **API and UI** expose the route, evidence, uncertainty, and continuation state.

No presentation-layer score may discard the underlying evidence or hide missing coverage.
