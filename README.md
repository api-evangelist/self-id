# Self.ID

APIs.json 0.19 provider profile for Self.ID — a Ceramic-based decentralized identity framework.

## Overview

Self.ID is an open-source SDK and reference application for building self-sovereign identity
applications on the [Ceramic network](https://ceramic.network). It enables developers to manage
DID profiles, verifiable credentials, and identity records using Ethereum-based authentication
and composable, user-centric data storage.

**Homepage:** https://self.id  
**GitHub:** https://github.com/ceramicstudio/self.id  
**Documentation:** https://developers.ceramic.network/tools/self-id/overview/

## APIs Cataloged

| API | Description |
|-----|-------------|
| Self.ID Core API | Read public DID records (Node + browser) via `@self.id/core` |
| Self.ID Web API | Read/write DID records in browsers via `@self.id/web` + 3ID Connect |
| Self.ID React API | React hooks for DID auth and record interactions via `@self.id/react` |
| Self.ID Framework API | High-level React framework via `@self.id/framework` |
| Ceramic HTTP API | Underlying REST transport for streams and DID data on Ceramic nodes |

## Key Concepts

- **DID (Decentralized Identifier):** Cryptographic identifier for a user, not controlled by any
  central authority. Ceramic uses `did:3` and `did:pkh` methods.
- **Streams:** Hash-linked chains of events on Ceramic for storing mutable JSON data (profiles,
  credentials, etc.).
- **3ID Connect:** Browser wallet integration enabling Ethereum-based DID authentication.
- **Data Models:** Pre-configured schemas for `basicProfile`, `cryptoAccounts`, and `alsoKnownAs`.

## Ceramic Network Endpoints

| Network | URL |
|---------|-----|
| Mainnet gateway (read-only) | https://gateway.ceramic.network |
| Clay testnet (read/write) | https://ceramic-clay.3boxlabs.com |
| Clay testnet gateway (read-only) | https://gateway-clay.ceramic.network |
| Local node | http://localhost:7007 |

## Plans & Pricing

Self.ID is fully open-source (MIT/Apache 2). There are no subscription fees. Costs arise from
infrastructure (hosting a Ceramic node) and blockchain anchor transactions on Ethereum mainnet.
See [plans/plans.yml](plans/plans.yml) and [finops/finops.yml](finops/finops.yml) for details.

## Rate Limits

No formal rate limits are published. Community gateway nodes may apply undocumented throttling.
See [rate-limits/rate-limits.yml](rate-limits/rate-limits.yml) for known constraints.

## Maintainer

Cataloged by [API Evangelist](https://apievangelist.com).  
Original project maintained by [Ceramic Studio / 3Box Labs](https://ceramic.network).
