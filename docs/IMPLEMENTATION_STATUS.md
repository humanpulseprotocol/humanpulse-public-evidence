# Implementation status

**Evidence review date:** 30 October 2026  
**Private canonical implementation:** `humanpulse-core`, reviewed at `1616247031fbf5b1cb28a14633c3b5881279f3f6` (29 October 2026).  
**Claim:** code/test artifacts and documentation were present at that checkpoint; this publication does not contain third-party test certification.

| Component | Engineering evidence in private implementation | Maturity and limitation |
| --- | --- | --- |
| Claim Guard policy and hosted sessions | Code, persistence and tests for context/session flow | Current prototype; no asserted production partner service |
| Wallet authorization | Authorization/binding implementation and tests | Local engineering scope |
| Browser capture / active presence | Runtime and regression testing, including synthetic fixtures | Not independently calibrated against population-scale attacks |
| Bronze-ZK | Native VOPRF / proof demonstration components and local verification tests | Demo-only trust/material; not independently audited operational uniqueness |
| Nullifier and proof reservation | Context-scoped duplicate semantics and reserved-result processing | Local and integration validation; external deployment not implied |
| Solana proof-consumption | Anchor source and local test suites | Devnet Release Candidate preparation; **no public deployment of this candidate claimed** |
| PartnerResult and finalization | Signed-result boundary, outbox and database migrations | Demonstrated in code/test scope; live commercial partner integration not established |
| Capacity accounting and relayer | Database-backed capacity and settlement/reconciliation modules | Partner-funded commercial service **not declared live** |
| EUDI / HAIP / OpenID4VP | Adapter and presentation implementation work | Authoritative issuer, registry and external interoperability gates remain |
| Production mode | Architectural target | **Not enabled or independently security-audited** |
| Multichain and advanced research | Technical direction | **Not implemented as live services** |

## Distinctions that must be preserved

**Current prototype:** implemented modules and local validation, including synthetic or controlled tests.  
**Release candidate:** a build/deploy package being prepared and tested, without an asserted public deployment.  
**Production mode:** requires independently reviewed security, real trust providers, operational key governance, calibration and release authorization.  
**Roadmap and research:** proposed work and optional modules, never represented as existing production capability.

The project has documented historic demo materials. They should not be confused with current release-candidate components or future production assurances.
