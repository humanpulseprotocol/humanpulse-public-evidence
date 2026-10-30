# Protocol overview

## Problem and intended role

Digital rights distributed through wallets can be repeatedly claimed by the same person using multiple addresses. Wallet-based rate limits cannot by themselves establish whether different wallets are controlled by different humans. Standard identity workflows can impose unnecessary personal-data collection or partner exposure.

HumanPulse is designed to provide **context-scoped evidence of live, eligible human participation and proof consumption**, with controls that significantly increase the cost of some multi-wallet and replay attacks. It does not guarantee elimination of Sybil abuse, identity rental, synthetic-media attacks, civil-identity collisions or all sources of fraud.

## Claim Guard: design boundaries

1. **Context Policy.** Defines the particular right, eligibility requirements, assurance level and duplicate-consumption scope.
2. **Hosted Session and Wallet Authorization.** Binds a verification attempt to the session, context and authorized claim wallet.
3. **Capture and Evidence Verification.** Applies liveness/challenge-response and evidence checks at the assurance level supported by the selected implementation and trust source.
4. **Scoped Commitment / Nullifier.** Designed to detect prior consumption in the same context without introducing a publicly shared universal identity identifier.
5. **Proof Reservation and Finalization.** Designed to separate verification/claim reservation from final consumption and partner fulfillment.
6. **PartnerResult and Settlement.** Designed to provide a minimal verifiable result to an integrating application and register limited proof-consumption state on Solana.

The wallet is a claim reference, not the identity of the human. On-chain data minimization does not make public blockchain metadata anonymous. Further privacy review and testing remain required.

## Intended users and applications

- DAOs and eligible governance/community participation workflows.
- Airdrops, token launches and other context-bound distribution rights.
- Digital products requiring an application-specific one-person/one-right control.

These are intended use cases; no customer adoption or active commercial integration is implied.

## Current and proposed architecture

The implementation effort is Solana-first. Production-grade partner-funded verification capacity, hardened trust integrations, assurance tiers and multichain support require additional validation or development. Details are separated in [Implementation status](IMPLEMENTATION_STATUS.md) and [Roadmap and open gates](ROADMAP_AND_OPEN_GATES.md).
