# 🔐 NexID Vault

NexID Vault is a decentralized identity vault for signing and verifying governance documents using DIDKit and IPFS.

## ✅ Features

- DID-based key generation
- Verifiable signature of JSON documents
- IPFS anchoring
- Guardian-ready architecture

## 🧭 Quick Start

```
didkit key generate ed25519 > keys/guardian-001.jwk
didkit did key -k keys/guardian-001.jwk
didkit vc issue-credential \
  --key keys/guardian-001.jwk \
  --credential manifest.json \
  --proof-purpose assertionMethod \
  > signed/manifest.signed.json
```

## 📦 IPFS Upload

Use [Web3.Storage](https://web3.storage/) or [Pinata](https://pinata.cloud/) to upload signed files.

## 🔐 For Guardians

This vault is designed for Guardian Circle members to sign constitutions, proposals, and DAO decisions.


---

## 🧾 ৭. `docs/for-organizations.md`


# 🏛️ NexID Vault for Organizations

NexID Vault enables NGOs, DAOs, and civic institutions to:

- Generate decentralized identities (DIDs)
- Sign governance documents (constitutions, proposals)
- Verify authenticity using DIDKit
- Anchor documents to IPFS for permanence

## 🔗 Integration Options

- Use CLI or API to sign documents
- Store signed files in IPFS
- Verify signatures using public DID

## 📦 Use Cases

- Student Unions
- NGO Charters
- DAO Governance
- Legal Declarations
