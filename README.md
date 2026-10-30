# HumanPulse Protocol

**Public technical overview · Implementation evidence · Development roadmap**  
**Last reviewed:** 30 October 2026  
**Primary implementation:** Claim Guard on Solana  
**Status:** Current Claim Guard Prototype / Devnet Release Candidate preparation

> HumanPulse proves the presence of a unique living human at a specific moment in time — instantly, privately, and on-chain.

This is HumanPulse's protocol positioning and design objective. It must not be read as a claim that a fully audited, universally reliable, production-grade proof of unique humanity is available today.

## What HumanPulse is building

HumanPulse is developing privacy-first, context-bound **proof-consumption infrastructure**. Claim Guard is intended to help applications enforce one eligible human's use of a specified digital right within a defined context — for example an airdrop claim, a token distribution, or an eligible DAO participation event — while minimizing disclosure of personal information to relying parties and the blockchain.

The architecture separates **human-presence and eligibility evidence**, **context policy**, **wallet authorization**, **context-scoped duplicate prevention**, **signed partner results**, and **minimal Solana proof-consumption records**.

## Implementation snapshot

The privately maintained canonical implementation contains source code and tests for hosted sessions, capture and verification, Bronze-ZK demonstration components, proof reservations, partner finalization, capacity accounting, settlement/receipt reconciliation and Solana program logic. **These are engineering artifacts and local validation work, not proof of a public production deployment.**

The repository's current release-candidate README explicitly identifies a **demo issuer** and **demo-only single-party Groth16 setup**, and lists outstanding external trust, cryptographic governance, calibration, audit, key-custody and release gates.

## Start here

| Document | Purpose |
| --- | --- |
| [Protocol overview](docs/PROTOCOL_OVERVIEW.md) | Problem, approach, architecture and privacy boundaries |
| [Implementation status](docs/IMPLEMENTATION_STATUS.md) | What is built, what is being validated, and what is not live |
| [Engineering milestones](docs/ENGINEERING_MILESTONES.md) | Traceable private engineering checkpoints and scope |
| [Technical evidence](docs/EVIDENCE_AND_PROVENANCE.md) | Evidence basis, limitations and external validation requirements |
| [Roadmap and open gates](docs/ROADMAP_AND_OPEN_GATES.md) | Technical, operational and research boundaries |
| [Funding and collaboration](docs/FUNDING_AND_COLLABORATION.md) | Areas where external funding or specialist support would accelerate the project |
| [Security and disclosure](SECURITY.md) | Security reporting and code-disclosure policy |
| [Official project references](docs/OFFICIAL_LINKS.md) | Owner-approved central directory of project channels and materials |

## Scope of this repository

This is a **public documentation and technical-evidence repository**. It is deliberately separate from the private implementation repository. It does **not** contain production secrets, the private source tree, an executable service, historical private commits, biometric datasets or release-key material.

Public visibility of these materials is **not** a claim that the underlying implementation is licensed as open-source software. See [NOTICE](NOTICE.md).

---

© 2026 HumanPulse Protocol. All rights reserved, except where explicitly stated otherwise.
