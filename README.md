# NepalHomes — BSV Home Marketplace

A BSV-only, MLS-style residential listing marketplace. **Testnet prototype; not production-ready.**

- Property prices and publication fees are denominated exclusively in BSV.
- Publication fee: **0.001 BSV = 100,000 satoshis**.
- Intended flow: property form → payment request QR → independent transaction verification → signed OP_RETURN commitment → searchable listing index.
- Source model: user-provided 11-page Residential Listing Input Form. This is an independent adaptation, not an official MLS feed.
- Never publish seller signatures, private remarks, gate codes, private contact information, or private keys to the blockchain.

## Preview

Open `index.html` locally or enable GitHub Pages for the repository. This is an **interface demonstration**: no real payments or broadcasts occur in the browser preview.

## Backend

The previously prepared Phase 2 backend package includes Node.js source for listing schemas, testnet payment verification, and externally signed transaction broadcasting. That backend has **not yet been deployed or committed in this repository**. Its raw-transaction checks are not equivalent to confirmed settlement. Before accepting real funds, add authentication, encrypted storage, confirmation monitoring, rate limiting, and independent provider validation.

## Important

The repository is **public**. Do not commit `.env`, admin bearer tokens, wallet seeds, or property owners' personal data.
