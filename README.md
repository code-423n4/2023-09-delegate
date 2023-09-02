# ✨ So you want to run an audit

This `README.md` contains a set of checklists for our audit collaboration.

Your audit will use two repos: 
- **an _audit_ repo** (this one), which is used for scoping your audit and for providing information to wardens
- **a _findings_ repo**, where issues are submitted (shared with you after the audit) 

Ultimately, when we launch the audit, this repo will be made public and will contain the smart contracts to be reviewed and all the information needed for audit participants. The findings repo will be made public after the audit report is published and your team has mitigated the identified issues.

Some of the checklists in this doc are for **C4 (🐺)** and some of them are for **you as the audit sponsor (⭐️)**.

---

# Repo setup

## ⭐️ Sponsor: Add code to this repo

- [ ] Create a PR to this repo with the below changes:
- [ ] Provide a self-contained repository with working commands that will build (at least) all in-scope contracts, and commands that will run tests producing gas reports for the relevant contracts.
- [ ] Make sure your code is thoroughly commented using the [NatSpec format](https://docs.soliditylang.org/en/v0.5.10/natspec-format.html#natspec-format).
- [ ] Please have final versions of contracts and documentation added/updated in this repo **no less than 48 business hours prior to audit start time.**
- [ ] Be prepared for a 🚨code freeze🚨 for the duration of the audit — important because it establishes a level playing field. We want to ensure everyone's looking at the same code, no matter when they look during the audit. (Note: this includes your own repo, since a PR can leak alpha to our wardens!)


---

## ⭐️ Sponsor: Edit this README

Under "SPONSORS ADD INFO HERE" heading below, include the following:

- [ ] Modify the bottom of this `README.md` file to describe how your code is supposed to work with links to any relevent documentation and any other criteria/details that the C4 Wardens should keep in mind when reviewing. ([Here's a well-constructed example.](https://github.com/code-423n4/2022-08-foundation#readme))
  - [ ] When linking, please **provide all links as full absolute links** versus relative links
  - [ ] All information should be provided in markdown format (HTML does not render on Code4rena.com)
- [ ] Under the "Scope" heading, provide the name of each contract and:
  - [ ] source lines of code (excluding blank lines and comments) in each
  - [ ] external contracts called in each
  - [ ] libraries used in each
- [ ] Describe any novel or unique curve logic or mathematical models implemented in the contracts
- [ ] Does the token conform to the ERC-20 standard? In what specific ways does it differ?
- [ ] Describe anything else that adds any special logic that makes your approach unique
- [ ] Identify any areas of specific concern in reviewing the code
- [ ] Review the Gas award pool amount. This can be adjusted up or down, based on your preference - just flag it for Code4rena staff so we can update the pool totals across all comms channels.
- [ ] Ensure that all links and image/file paths in this README use absolute paths, not relative paths. 
- [ ] Optional / nice to have: pre-record a high-level overview of your protocol (not just specific smart contract functions). This saves wardens a lot of time wading through documentation.
- [ ] See also: [this checklist in Notion](https://code4rena.notion.site/Key-info-for-Code4rena-sponsors-f60764c4c4574bbf8e7a6dbd72cc49b4#0cafa01e6201462e9f78677a39e09746)
- [ ] Delete this checklist and all text above the line below when you're ready.

---

# Delegate audit details
- Total Prize Pool: $50,000 USDC
  - HM awards: ??? USDC
  - Analysis awards: ??? USDC
  - QA awards: ??? USDC
  - Bot Race awards: ??? USDC
  - Gas awards: ??? USDC
  - Judge awards: ??? USDC
  - Lookout awards: ??? USDC
  - Scout awards: ??? USDC
- Join [C4 Discord](https://discord.gg/code4rena) to register
- Submit findings [using the C4 form](https://code4rena.com/contests/2023-09-delegate/submit)
- [Read our guidelines for more details](https://docs.code4rena.com/roles/wardens)
- Starts September 5, 2023 20:00 UTC
- Ends September 10, 2023 20:00 UTC

## Automated Findings / Publicly Known Issues

Automated findings output for the audit can be found [here](https://github.com/code-423n4/2023-09-delegate/blob/main/bot-report.md) within 24 hours of audit opening.

*Note for C4 wardens: Anything included in the automated findings output is considered a publicly known issue and is ineligible for awards.*



[ ⭐️ SPONSORS ADD INFO HERE ]

# Overview

This contest covers two key pieces:
- v2 of the delegate registry
- v2 of the delegate marketplace

The delegate registry is a standalone singleton database that aggregates onchain programmable access control. Users can link cold wallets to hot wallets, or specify individual token rights to delegate to other wallets. This separation of asset utility from the asset owner is a powerful primitive that enables the delegate marketplace. The delegate marketplace lets users wrap delegation rights into ERC721 tokens that can then be traded or transferred in the same way as any other NFT. The primary usecase here is utility rentals with zero counterparty risk, zero liquidation risk, zero overcollateralization requirements, and an order of magnitude greater capital efficiency.

v1 of the delegate registry has been live across many EVM chains since September 2022. While v1 is not in scope, auditors are encouraged to review its usage patterns at [https://etherscan.io/address/0x00000000000076a84fef008cdabe6409d2fe638b](https://etherscan.io/address/0x00000000000076a84fef008cdabe6409d2fe638b). A frontend interface across all deployed chains and testnets can be used at [https://delegate.xyz](https://delegate.xyz). The v2 registry is similar to v1, although with expanded support for fungible token amounts, cleaner enumeration methods, multicall transaction batching, gas efficiency improvements, and the introduction of subdelegation rights. Documentation for v1 can be found at [https://docs.delegate.xyz](https://docs.delegate.xyz). 

The delegate marketplace consists of three core contracts: the DelegateToken, the PrincipalToken, and the CreateOfferer. Users will deposit a token, such as a bored ape NFT, into smart contract escrow using the DelegateToken.sol::create() function. They will receive back two ERC721s: a bored ape DelegateToken, and a bored ape PrincipalToken. The holder of the DelegateToken will receive delegate rights for the duration of the escrow. The holder of the PrincipalToken will have the right to redeem the bored ape from escrow at conclusion of the chosen timeframe. Users can choose to transfer or sell neither, one, or both of these. The CreateOfferer is a Seaport Contract Offerer that enables gasless listing of DelegateTokens which have not been created yet. If a buyer fulfills the gasless listing, then the desired token will be atomically escrowed and a DelegateToken created.

# Scope

| Contract | SLOC | Purpose | Libraries used |  
| ----------- | ----------- | ----------- | ----------- |
| [lib/delegate-registry/src/DelegateRegistry.sol](lib/delegate-registry/src/DelegateRegistry.sol) | 364 | v2 of the delegate registry | ??? |
| [lib/delegate-registry/src/libraries/RegistryHashes.sol](lib/delegate-registry/src/libraries/RegistryHashes.sol) | 135 | Helper library for registry hash calculation | ??? |
| [lib/delegate-registry/src/libraries/RegistryStorage.sol](lib/delegate-registry/src/libraries/RegistryStorage.sol) | 31 | Helper library for registry storage layout | ??? |
| [lib/delegate-registry/src/libraries/RegistryOps.sol](lib/delegate-registry/src/libraries/RegistryOps.sol) | 18 | Helper library for branchless boolean ops | ??? |
| [src/DelegateToken.sol](src/DelegateToken.sol) | 288 | Represent delegate rights as a transferrable ERC721 | ??? |
| [src/PrincipalToken.sol](src/PrincipalToken.sol) | 43 | Represent the rights to claim the deposited token as a transferrable ERC721 | ??? |
| [src/CreateOfferer.sol](src/CreateOfferer.sol) | 171 | Seaport Contract Offerer to enable gasless listings of DTs before they're created | ??? |
| [src/libraries/CreateOffererLib.sol](src/libraries/CreateOffererLib.sol) | 267 | Helper library for CreateOfferer | ??? |
| [src/libraries/DelegateTokenLib.sol](src/libraries/DelegateTokenLib.sol) | 90 | Helper library for DelegateToken | ??? |
| [src/libraries/DelegateTokenRegistryHelpers.sol](src/libraries/DelegateTokenRegistryHelpers.sol) | 219 | Helper library for Delegate Token registry hitchhiking | ??? |
| [src/libraries/DelegateTokenStorageHelpers.sol](src/libraries/DelegateTokenStorageHelpers.sol) | 125 | Helper library for Delegate Token registry hitchhiking | ??? |
| [src/libraries/DelegateTokenTransferHelpers.sol](src/libraries/DelegateTokenTransferHelpers.sol) | 73 | Helper library for Delegate Token ERC20/721/1155 transfers | ??? |

## Out of scope

The following contracts are out of scope:
- Any deployment or upgrade scripts are out of scope (but can be used to test the contracts in scope).
- Files in test/, contracts/test/ or src/test/ are out of scope (but can be used to test the contracts in scope).
- External libraries (@openzeppelin/*, @seaport/*)
- [src/MarketMetadata.sol](src/MarketMetadata.sol)
- [lib/delegate-registry/src/singlesig/Singlesig.sol](lib/delegate-registry/src/singlesig/Singlesig.sol)
- lib/delegate-registry/src/examples/*.sol

# Additional Context

*Describe any novel or unique curve logic or mathematical models implemented in the contracts*

*Sponsor, please confirm/edit the information below.*

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

# Tests

*Provide every step required to build the project from a fresh git clone, as well as steps to run the tests with a gas report.* 

*Note: Many wardens run Slither as a first pass for testing.  Please document any known errors with no workaround.* 
