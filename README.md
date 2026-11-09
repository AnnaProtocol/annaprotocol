# ANNΛ Protocol — Project overview

**Artificial Neural Network for Accountability**

ANNA Protocol is an experimental infrastructure project for recording and verifying AI-related attestations using cryptographic commitments and blockchain contracts.

## Explore the public project

| Component | Source repository | Live application |
| --- | --- | --- |
| Official website and attestation lookup | [annaprotocol.com](https://github.com/AnnaProtocol/annaprotocol.com) | [annaprotocol.com](https://annaprotocol.com) |
| Wallet-connected dashboard | [dashboard.annaprotocol.online](https://github.com/AnnaProtocol/dashboard.annaprotocol.online) | [dashboard.annaprotocol.online](https://dashboard.annaprotocol.online) |
| Earlier static site | **This repository** | — |

## Architecture at a glance

```text
AI client / SDK
      |
      v
Attestation contracts (Polygon Amoy testnet)
      |                    |
      v                    v
Verification workflow   Identity / reputation
      |                    |
      +---------+----------+
                |
         Web dashboard
                |
        Public verification
```

This diagram describes the broader ANNA system; **this repository contains only a standalone `index.html`**, not the SDK, smart-contract sources, verifier service, or dashboard application source.

## Scope and verification

- The public demonstration uses the **Polygon Amoy testnet**, not Polygon mainnet.
- An on-chain record supports traceability of a commitment. It does **not** independently prove that an AI decision is correct.
- The dashboard repository contains a compiled frontend distribution; it is not the full React source project.
- This is a prototype/research system. Independent security assessment and verification-policy review are recommended before production use.

## Local preview

Open `index.html` in a browser, or serve the directory using `python -m http.server 8000` and visit http://localhost:8000.

## Project links

- [Official site](https://annaprotocol.com)
- [Public attestation verifier](https://annaprotocol.com/verify.html)
- [Dashboard](https://dashboard.annaprotocol.online)
- [ANNA Protocol organization](https://github.com/AnnaProtocol)

**Founder / developer:** Antonio Rufino.
