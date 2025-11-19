[README.md](https://github.com/user-attachments/files/23622084/README.md)
# Event Pass

## Project Description
The Event Pass contract provides a simple way to issue and manage event passes on the Stellar blockchain. It allows event organizers to issue passes to attendees, associating each address with a specific event name. This creates a tamper-proof record of event access that can be verified on-chain. The contract is designed for simplicity and efficiency, making it easy to track who has access to which events.

This contract is perfect for event organizers, conference managers, or anyone who needs to manage access control for events. By storing event passes on the blockchain, you create a verifiable and tamper-proof system that cannot be forged. Attendees can prove their access rights, and organizers can verify passes instantly without needing to contact a central database. This makes it ideal for conferences, concerts, workshops, or any event where access control is important.

**Key Benefits:**
- **Tamper-Proof**: Event passes cannot be forged or duplicated
- **Instant Verification**: Passes can be verified on-chain without database queries
- **Decentralized**: No single point of failure for access control
- **Transparent**: All issued passes are publicly verifiable
- **Cost-Effective**: Low-cost solution for event access management
- **Global Access**: Passes can be verified from anywhere

![Contract Explorer](img/contract-explorer.png)

**Contract Address:** `CAX6NLKPYRXZEOTSOC2DM76MO6UIYOCHEQEOLSQQNZJFZALBQTB6EWGT`

**View on Stellar Expert:** [https://stellar.expert/explorer/testnet/contract/CAX6NLKPYRXZEOTSOC2DM76MO6UIYOCHEQEOLSQQNZJFZALBQTB6EWGT](https://stellar.expert/explorer/testnet/contract/CAX6NLKPYRXZEOTSOC2DM76MO6UIYOCHEQEOLSQQNZJFZALBQTB6EWGT)

## Features
- Simple getter function to retrieve event pass information
- Simple setter function to issue event passes
- Basic storage model using address-to-event mapping
- Minimal, gas-efficient logic

## Building the Contract

To build use:
```bash
stellar contract build
```

## Deploy to Testnet
Run:

```bash
stellar contract deploy \
  --wasm target/wasm32v1-none/release/project-11.wasm \
  --source-account alice \
  --network testnet \
  --alias project-11
```


