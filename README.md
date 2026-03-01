# Multichain Exploit PoC — MPC Key Infrastructure Compromise

## Overview
- **Date:** 2023-07-07
- **Loss:** ~$126M
- **Chain:** Multi-chain
- **Category:** Access Control Failures
- **Block:** 17636491

## Vulnerability
Multichain marketed MPC (Multi-Party Computation) key management but the CEO stored all key shards on a single cloud server. When the server was compromised, all bridge funds across multiple chains became accessible.

## Reproduction
```bash
git clone https://github.com/NomosLabs-Security/poc-multichain-2023
cd poc-multichain-2023
forge install foundry-rs/forge-std --no-git
forge test -vvvv
```

## References
- [Chainalysis Investigation](https://www.chainalysis.com/blog/multichain-exploit-july-2023/)
