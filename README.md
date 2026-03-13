# PermaDocs# PermaDocs

> A permanent, censorship-resistant document archive built on [Shelby Protocol](https://shelby.xyz) — store contracts, records, journalism, and personal documents that can never be deleted, altered, or censored.

---

## What is PermaDocs?

PermaDocs is a decentralized document archiving platform built on top of the Shelby Protocol. It is designed for individuals, journalists, activists, lawyers, and organizations who need to store critical documents with a permanent, tamper-proof guarantee.

Unlike traditional cloud storage where files can be deleted by the provider, government order, or account suspension, PermaDocs stores every document as an immutable blob on the Shelby network with its cryptographic commitment recorded on the Aptos blockchain. Once uploaded, a document exists permanently and can always be retrieved by its blob ID.

---

## The Problem

Critical documents are vulnerable on centralized platforms:

- Governments can issue takedown orders
- Cloud providers can suspend accounts without warning
- Companies can go bankrupt, taking your data with them
- Evidence and records can be quietly altered or removed

Journalists lose sources. Activists lose evidence. Individuals lose irreplaceable personal records. There is currently no simple, developer-friendly solution that combines permanent storage with cryptographic proof of integrity.

---

## Why Shelby?

Shelby's infrastructure solves this problem at the protocol level:

- **Immutable blobs** — Once written, documents cannot be altered or deleted
- **Cryptographic commitments** — Every document is committed to the Aptos blockchain, providing verifiable proof of existence and integrity
- **Erasure coding** — Documents are redundantly stored across multiple providers, eliminating single points of failure
- **Dedicated fiber network** — Fast and reliable retrieval, even for large files
- **Decentralized auditing** — Storage providers are continuously audited to ensure documents remain intact

---

## Use Cases

- **Journalism** — Archive investigation materials, sources, and evidence permanently
- **Legal** — Store contracts, agreements, and legal records with tamper-proof timestamps
- **Activism** — Preserve documentation of human rights violations beyond the reach of censorship
- **Personal** — Wills, property deeds, medical records, family archives
- **Academic** — Research data, papers, and datasets that must remain accessible long-term
- **Whistleblowing** — Safely preserve and share evidence without fear of deletion

---

## How It Works

1. User uploads a document (PDF, image, video, or any file format)
2. Shelby SDK erasure-codes the file and writes it to the storage network
3. A cryptographic commitment is recorded on the Aptos blockchain
4. User receives a permanent blob ID — the document is now retrievable forever
5. Anyone with the blob ID can verify the document's integrity against the on-chain commitment

---

## Roadmap

### Phase 1 — Core Archive
- [ ] Project setup with Shelby TypeScript SDK
- [ ] Document upload flow (PDF, images, any file type)
- [ ] Blob ID generation and permanent retrieval
- [ ] On-chain timestamp and integrity verification
- [ ] Basic document viewer UI

### Phase 2 — Verification & Trust
- [ ] Public proof-of-existence certificates
- [ ] QR code generation linking to on-chain commitment
- [ ] Document integrity checker (verify a file against its blob ID)
- [ ] Wallet connection (Aptos) for ownership records

### Phase 3 — Organization & Access
- [ ] Collections and folders
- [ ] Selective sharing via encrypted blob access
- [ ] Multi-signature document approval (for organizations)
- [ ] Expiry-free public archive mode

### Phase 4 — Ecosystem & Integrations
- [ ] API for third-party integrations (legal platforms, news organizations)
- [ ] Browser extension for one-click archiving of web pages
- [ ] Whistleblower-safe anonymous upload mode
- [ ] Mobile PWA

---

## Tech Stack

| Layer | Technology |
|---|---|
| Storage | Shelby Protocol |
| Blockchain | Aptos |
| SDK | `@shelby-protocol/sdk` |
| Frontend | TypeScript / React |
| Smart Contracts | Move |

---

## Getting Started

> ⚠️ Shelby is currently running on testnet. Early access required via [shelby.xyz](https://shelby.xyz).

```bash
# Install Shelby SDK
npm install @shelby-protocol/sdk

# Install Shelby CLI
npm install -g @shelby-protocol/cli
```

---

## Contributing

This project is in early development. Contributions, ideas, and feedback are welcome. Feel free to open an issue or submit a pull request.

---

## License

MIT

---

*Built during Shelby Early Access Testnet — powered by Shelby Protocol & Aptos*
