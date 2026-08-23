# Soroverify

Independent, multi-verifier source verification for Soroban contracts.

Soroban doesn't store contract source on-chain. Soroverify closes that gap: given a deployed contract and its claimed source, it rebuilds the source in an isolated container and checks whether the result actually matches the deployed Wasm.

## Repositories

- **[soroverify-verifier](https://github.com/soroverify/soroverify-verifier)** — the rebuild-and-verify service.
- **[soroverify-consume](https://github.com/soroverify/soroverify-consume)** — SDK, embeddable badge widget, and reference integration.
- **[soroverify-watch](https://github.com/soroverify/soroverify-watch)** — continuous monitoring; detects when a previously verified contract's deployed code changes and publishes signed drift records.
- **[soroverify-action](https://github.com/soroverify/soroverify-action)** — a GitHub Action that submits a contract for verification directly from CI on release.

## Links

- [Documentation](https://hollujay-labs.gitbook.io/hollujay-labs-docs)
- [Live discussion with the SEP-58 maintainers](https://github.com/orgs/stellar/discussions/1923)

## Status

Pre-audit. See each repo's SECURITY.md for current scope.
