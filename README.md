# Delegate audit details

- Total Prize Pool: $50,000 USDC
  - HM awards: $34,237.50 USDC
  - Analysis awards: $2,075 USDC
  - QA awards: $1037.50 USDC
  - Bot Race awards: $3,112.50 USDC
  - Gas awards: $1037.50 USDC
  - Judge awards: $5,000 USDC
  - Lookout awards: $3,000 USDC
  - Scout awards: $500 USDC
- Join [C4 Discord](https://discord.gg/code4rena) to register
- Submit findings [using the C4 form](https://code4rena.com/contests/2023-09-delegate/submit)
- [Read our guidelines for more details](https://docs.code4rena.com/roles/wardens)
- Starts September 5, 2023 20:00 UTC
- Ends September 11, 2023 20:00 UTC

## Automated Findings / Publicly Known Issues

Automated findings output for the audit can be found [here](https://github.com/code-423n4/2023-09-delegate/blob/main/bot-report.md) within 24 hours of audit opening.

*Note for C4 wardens: Anything included in the automated findings output is considered a publicly known issue and is ineligible for awards.*

# Overview

This contest covers two key pieces:

- v2 of the delegate registry
- v2 of the delegate marketplace

The delegate registry is a standalone singleton database that aggregates onchain programmable access control. Users can link cold wallets to hot wallets, or specify individual token rights to delegate to other wallets. This separation of asset utility from the asset owner is a powerful primitive that enables the delegate marketplace. The delegate marketplace lets users wrap delegation rights into ERC721 tokens that can then be traded or transferred in the same way as any other NFT. The primary use-case here is utility rentals with zero counterparty risk, zero liquidation risk, zero overcollateralization requirements, and an order of magnitude greater capital efficiency.

v1 of the delegate registry has been live across many EVM chains since September 2022. While v1 is not in scope, auditors are encouraged to review its usage patterns at [https://etherscan.io/address/0x00000000000076a84fef008cdabe6409d2fe638b](https://etherscan.io/address/0x00000000000076a84fef008cdabe6409d2fe638b). A frontend interface across all deployed chains and testnets can be used at [https://delegate.xyz](https://delegate.xyz). The v2 registry is similar to v1, although with expanded support for fungible token amounts, cleaner enumeration methods, multicall transaction batching, gas efficiency improvements, and the introduction of subdelegation rights. Documentation for v1 can be found at [https://docs.delegate.xyz](https://docs.delegate.xyz).

The delegate marketplace consists of three core contracts: the DelegateToken, the PrincipalToken, and the CreateOfferer. Users will deposit a token, such as a bored ape NFT, into smart contract escrow using the DelegateToken.sol::create() function. They will receive back two ERC721s: a bored ape DelegateToken, and a bored ape PrincipalToken. The holder of the DelegateToken will receive delegate rights for the duration of the escrow. The holder of the PrincipalToken will have the right to redeem the bored ape from escrow at conclusion of the chosen timeframe. Users can choose to transfer or sell neither, one, or both of these. The CreateOfferer is a Seaport Contract Offerer that enables gasless listing of DelegateTokens which have not been created yet. If a buyer fulfills the gasless listing, then the desired token will be atomically escrowed and a DelegateToken created.

# Scope

| Contract | SLOC | Purpose | Libraries used |  
| ----------- | ----------- | ----------- | ----------- |
| [lib/delegate-registry/src/DelegateRegistry.sol](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol) | 364 | v2 of the delegate registry | ??? |
| [lib/delegate-registry/src/libraries/RegistryHashes.sol](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol) | 135 | Helper library for registry hash calculation | ??? |
| [lib/delegate-registry/src/libraries/RegistryStorage.sol](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol) | 31 | Helper library for registry storage layout | ??? |
| [lib/delegate-registry/src/libraries/RegistryOps.sol](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol) | 18 | Helper library for branchless boolean ops | ??? |
| [src/DelegateToken.sol](https://github.com/code-423n4/2023-09-delegate/blob/main/src/DelegateToken.sol) | 288 | Represent delegate rights as a transferrable ERC721 | ??? |
| [src/PrincipalToken.sol](https://github.com/code-423n4/2023-09-delegate/blob/main/src/PrincipalToken.sol) | 43 | Represent the rights to claim the deposited token as a transferrable ERC721 | ??? |
| [src/CreateOfferer.sol](https://github.com/code-423n4/2023-09-delegate/blob/main/src/CreateOfferer.sol) | 171 | Seaport Contract Offerer to enable gasless listings of DTs before they're created | ??? |
| [src/libraries/CreateOffererLib.sol](https://github.com/code-423n4/2023-09-delegate/blob/main/src/libraries/CreateOffererLib.sol) | 267 | Helper library for CreateOfferer | ??? |
| [src/libraries/DelegateTokenLib.sol](https://github.com/code-423n4/2023-09-delegate/blob/main/src/libraries/DelegateTokenLib.sol) | 90 | Helper library for DelegateToken | ??? |
| [src/libraries/DelegateTokenRegistryHelpers.sol](https://github.com/code-423n4/2023-09-delegate/blob/main/src/libraries/DelegateTokenRegistryHelpers.sol) | 219 | Helper library for Delegate Token registry hitchhiking | ??? |
| [src/libraries/DelegateTokenStorageHelpers.sol](https://github.com/code-423n4/2023-09-delegate/blob/main/src/libraries/DelegateTokenStorageHelpers.sol) | 125 | Helper library for Delegate Token registry hitchhiking | ??? |
| [src/libraries/DelegateTokenTransferHelpers.sol](https://github.com/code-423n4/2023-09-delegate/blob/main/src/libraries/DelegateTokenTransferHelpers.sol) | 73 | Helper library for Delegate Token ERC20/721/1155 transfers | ??? |

## Out of scope

The following contracts are out of scope:

- Any deployment or upgrade scripts are out of scope (but can be used to test the contracts in scope).
- Files in test/, contracts/test/ or src/test/ are out of scope (but can be used to test the contracts in scope).
- External libraries (@openzeppelin/*, @seaport/*)
- [src/MarketMetadata.sol](https://github.com/code-423n4/2023-09-delegate/blob/main/src/MarketMetadata.sol)
- [lib/delegate-registry/src/singlesig/Singlesig.sol](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/singlesig/Singlesig.sol)
- lib/delegate-registry/src/examples/*.sol

## Scoping Details

```
- If you have a public code repo, please share it here:  
- How many contracts are in scope?:   12
- Total SLoC for these contracts?:  ~1500
- How many external imports are there?: 2 
- How many separate interfaces and struct definitions are there for the contracts within scope?:  ~10
- Does most of your code generally use composition or inheritance?:   Composition
- How many external calls?:   ~5
- What is the overall line coverage percentage provided by your tests?: 80%
- Is this an upgrade of an existing system?: True
- Check all that apply (e.g. timelock, NFT, AMM, ERC20, rollups, etc.): ERC-20 Token, Non ERC-20 Token
- Is there a need to understand a separate part of the codebase / get context in order to audit this part of the protocol?:  False 
- Please describe required context:   n/a
- Does it use an oracle?:  No
- Describe any novel or unique curve logic or mathematical models your code uses: None
- Is this either a fork of or an alternate implementation of another project?: False  
- Does it use a side-chain?: False
- Describe any specific areas you would like addressed: Please focus on registry correctness as that intersects with the marketplace
```

## Setup

Either clone with `--recurse`:

```bash
git clone --recurse https://github.com/code-423n4/2023-09-delegate.git
```

Use one of the following if `--recurse` was forgotten:

```bash
git submodule update --init --recursive
forge install
```

Be sure to run `foundryup`:

```bash
foundryup
```

## Tests

```bash
# Run marketplace tests
forge test
# Run registry tests
cd lib/delegate-registry && forge test && cd ../..
# Run registry gas benchmarks
cd lib/delegate-registry && forge test --match-contract GasBenchmark --gas-report > gasbenchmark10mil && forge test --match-contract HashBenchmark --gas-report > hashbenchmark10mil && cd ../..
```

## Slither

To run Slither, use the following command:

```bash
mv test _test
slither .
mv _test test
```
