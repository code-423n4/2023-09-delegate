

```bash
# # # # # # # # # # # # # # # # # # # # # #
#                                         #
#             |\_/|                       #
#             | O O                       #
#             |   <>              _       #
#             |  _/\------____ ((| |))    #
#             |               `--' |      #
#         ____|_       ___|   |___.'      #
#        /_/_____/____/_______|           #
#    _   _                           _    #
#   | | | |                         | |   #
#   | |_| |  ___   _   _  _ __    __| |   #
#   |  _  | / _ \ | | | || '_ \  / _` |   #
#   | | | || (_) || |_| || | | || (_| |   #
#   \_| |_/ \___/  \__,_||_| |_| \__,_|   #
#                                         #
# # # # # # # # # # # # # # # # # # # # # #
```


## Summary

---

### Medium Risk Issues
|Id|Title|Instances|
|:--:|:------|:--:|
|[[M-01]](#m-01-transferred-erc721-can-be-stuck-permanently)| Transferred `ERC721` can be stuck permanently | 2 |
|[[M-02]](#m-02-unchecked-blocks-with-subtractions-may-underflow)| `unchecked` blocks with subtractions may underflow | 1 |
|[[M-03]](#m-03-some-functions-do-not-work-correctly-with-fee-on-transfer-tokens)| Some functions do not work correctly with fee-on-transfer tokens | 1 |

Total: 4 instances over 3 issues.

### Low Risk Issues
|Id|Title|Instances|
|:--:|:------|:--:|
|[[L-01]](#l-01-avoid-double-casting)| Avoid double casting | 3 |
|[[L-02]](#l-02-functions-calling-contracts-with-transfer-hooks-are-missing-reentrancy-guards)| Functions calling contracts with transfer hooks are missing reentrancy guards | 2 |
|[[L-03]](#l-03-large-transfers-may-not-work-with-some-erc20-tokens)| Large transfers may not work with some `ERC20` tokens | 2 |
|[[L-04]](#l-04-large-approvals-may-not-work-with-some-erc20-tokens)| Large approvals may not work with some `ERC20` tokens | 1 |
|[[L-05]](#l-05-approve-can-revert-if-the-current-approval-is-not-zero)| `approve` can revert if the current approval is not zero | 1 |
|[[L-06]](#l-06-nft-ownership-doesnt-support-hard-forks)| NFT ownership doesn't support hard forks | 1 |
|[[L-07]](#l-07-missing-disallowlist-for-erc721)| Missing disallowlist for `ERC721` | 1 |
|[[L-08]](#l-08-unchecked-blocks-with-additionsmultiplications-may-overflow)| `unchecked` blocks with additions/multiplications may overflow | 2 |
|[[L-09]](#l-09-some-functions-contain-the-same-exact-logic)| Some functions contain the same exact logic | 2 |
|[[L-10]](#l-10-use-of-transfer-instead-of-safetransfer)| Use of `transfer` instead of `safeTransfer` | 3 |
|[[L-11]](#l-11-external-calls-in-an-unbounded-loop-can-result-in-a-dos)| External calls in an unbounded loop can result in a DoS | 1 |
|[[L-12]](#l-12-using-zero-as-a-parameter)| Using zero as a parameter | 4 |

Total: 23 instances over 12 issues.

### Non Critical Issues
|Id|Title|Instances|
|:--:|:------|:--:|
|[[NC-01]](#nc-01-missing-events-in-sensitive-functions)| Missing events in sensitive functions | 2 |
|[[NC-02]](#nc-02-unused-named-return)| Unused named `return` | 23 |
|[[NC-03]](#nc-03-consider-using-erc721a-instead-of-erc721)| Consider using `ERC721A` instead of `ERC721` | 1 |
|[[NC-04]](#nc-04-enum-values-should-be-used-in-place-of-constant-array-indexes)| Enum values should be used in place of constant array indexes | 22 |
|[[NC-05]](#nc-05-variable-initialization-with-default-value)| Variable initialization with default value | 17 |
|[[NC-06]](#nc-06-duplicated-requireif-statements-should-be-refactored)| Duplicated `require/if` statements should be refactored | 2 |
|[[NC-07]](#nc-07-unbounded-loop-may-run-out-of-gas)| Unbounded loop may run out of gas | 7 |
|[[NC-08]](#nc-08-use-of-non-named-numeric-constants)| Use of non-named numeric constants | 17 |
|[[NC-09]](#nc-09-control-structures-do-not-comply-with-best-practices)| Control structures do not comply with best practices | 59 |
|[[NC-10]](#nc-10-use-a-single-file-for-system-wide-constants)| Use a single file for system wide constants | 4 |
|[[NC-11]](#nc-11-old-solidity-version)| Old Solidity version | 5 |
|[[NC-12]](#nc-12-use-of-floating-pragma)| Use of floating pragma | 4 |
|[[NC-13]](#nc-13-no-checks-for-empty-bytes)| No checks for empty bytes | 1 |
|[[NC-14]](#nc-14-contract-functions-should-use-an-interface)| Contract functions should use an `interface` | 48 |
|[[NC-15]](#nc-15-multiple-addressid-mappings-can-be-combined-into-a-single-mapping-of-an-addressid-to-a-struct-for-readability)| Multiple `address`/ID mappings can be combined into a single mapping of an `address`/ID to a `struct`, for readability | 1 |
|[[NC-16]](#nc-16-imports-should-be-organized-more-systematically)| Imports should be organized more systematically | 3 |
|[[NC-17]](#nc-17-event-is-missing-msgsender-parameter)| Event is missing `msg.sender` parameter | 3 |
|[[NC-18]](#nc-18-unresolved-todos-in-comments)| Unresolved `TODOs` in comments | 1 |
|[[NC-19]](#nc-19-use-of-polymorphism-is-discouraged-for-security-audits)| Use of polymorphism is discouraged for security audits | 4 |
|[[NC-20]](#nc-20-custom-error-without-details)| Custom `error` without details | 35 |
|[[NC-21]](#nc-21-constants-in-comparisons-should-appear-on-the-left-side)| Constants in comparisons should appear on the left side | 21 |
|[[NC-22]](#nc-22-consider-using-delete-instead-of-assigning-zerofalse-to-clear-values)| Consider using `delete` instead of assigning zero/false to clear values | 2 |
|[[NC-23]](#nc-23-use-a-ternary-statement-instead-of-ifelse-when-appropriate)| Use a ternary statement instead of `if`/`else` when appropriate | 2 |
|[[NC-24]](#nc-24-layout-order-does-not-comply-with-best-practices)| Layout order does not comply with best practices | 1 |
|[[NC-25]](#nc-25-function-visibility-order-does-not-comply-with-best-practices)| Function visibility order does not comply with best practices | 2 |
|[[NC-26]](#nc-26-long-functions-should-be-refactored-into-multiple-functions)| Long functions should be refactored into multiple functions | 1 |
|[[NC-27]](#nc-27-lines-are-too-long)| Lines are too long | 197 |
|[[NC-28]](#nc-28-missing-variable-names)| Missing variable names | 14 |
|[[NC-29]](#nc-29-typos-in-comments)| Typos in comments | 2 |
|[[NC-30]](#nc-30-contracts-should-have-full-test-coverage)| Contracts should have full test coverage | 1 |
|[[NC-31]](#nc-31-large-or-complicated-code-bases-should-implement-invariant-tests)| Large or complicated code bases should implement invariant tests | 1 |
|[[NC-32]](#nc-32-codebase-should-implement-formal-verification-testing)| Codebase should implement formal verification testing | 1 |
|[[NC-33]](#nc-33-inconsistent-spacing-in-comments)| Inconsistent spacing in comments | 9 |
|[[NC-34]](#nc-34-state-variables-should-include-comments)| State variables should include comments | 19 |
|[[NC-35]](#nc-35-complex-functions-should-have-explicit-comments)| Complex functions should have explicit comments | 1 |
|[[NC-36]](#nc-36-assembly-code-should-have-explicit-comments)| Assembly code should have explicit comments | 28 |
|[[NC-37]](#nc-37-missing-underscore-prefix-for-non-external-functions)| Missing underscore prefix for non-external functions | 83 |
|[[NC-38]](#nc-38-missing-underscore-prefix-for-non-external-variables)| Missing underscore prefix for non-external variables | 12 |
|[[NC-39]](#nc-39-invalid-natspec-comment-style)| Invalid NatSpec comment style | 1 |
|[[NC-40]](#nc-40-missing-natspec-from-contract-declarations)| Missing NatSpec from contract declarations | 5 |
|[[NC-41]](#nc-41-missing-natspec-title)| Missing NatSpec `@title` | 10 |
|[[NC-42]](#nc-42-missing-natspec-author)| Missing NatSpec `@author` | 12 |
|[[NC-43]](#nc-43-missing-natspec-from-function-definitions)| Missing NatSpec from function definitions | 2 |
|[[NC-44]](#nc-44-missing-natspec-param)| Missing NatSpec `@param` | 45 |
|[[NC-45]](#nc-45-incomplete-natspec-return)| Incomplete NatSpec `@return` | 23 |

Total: 755 instances over 45 issues.

### Gas Optimizations
|Id|Title|Instances|Gas Saved|
|:--:|:------|:--:|---:|
|[[G-01]](#g-01-multiple-mappings-that-share-an-id-can-be-combined-into-a-single-mapping-of-id--struct)| Multiple `mapping`s that share an ID can be combined into a single `mapping` of ID / `struct` | 1 | 20,084 |
|[[G-02]](#g-02-cache-state-variables-with-stack-variables)| Cache state variables with stack variables | 14 | 5,500 |
|[[G-03]](#g-03-avoid-contract-existence-checks-by-using-low-level-calls)| Avoid contract existence checks by using low level calls | 34 | 3,400 |
|[[G-04]](#g-04-use-at-least-solidity-version-0819-to-gain-some-gas-boost)| Use at least Solidity version `0.8.19` to gain some gas boost | 5 | - |
|[[G-05]](#g-05-use-of-memory-instead-of-calldata-for-immutable-arguments)| Use of `memory` instead of `calldata` for immutable arguments | 4 | 1,048 |
|[[G-06]](#g-06-using-bool-for-storage-incurs-overhead)| Using `bool` for storage incurs overhead | 1 | 17,100 |
|[[G-07]](#g-07-consider-activating-via-ir-for-deploying)| Consider activating `via-ir` for deploying | 1 | - |
|[[G-08]](#g-08-function-calls-should-be-cached-instead-of-re-calling-the-function)| Function calls should be cached instead of re-calling the function | 2 | - |
|[[G-09]](#g-09-functions-that-revert-when-called-by-normal-users-can-be-payable)| Functions that revert when called by normal users can be `payable` | 2 | 42 |
|[[G-10]](#g-10-array-length-is-not-cached)| Array `length` is not cached | 2 | 6 |
|[[G-11]](#g-11-usage-of-uintsints-smaller-than-32-bytes-256-bits-incurs-overhead)| Usage of `uints`/`ints` smaller than 32 bytes (256 bits) incurs overhead | 1 | 6 |
|[[G-12]](#g-12-using-pre-instead-of-post-incrementsdecrements)| Using pre instead of post increments/decrements | 2 | 10 |
|[[G-13]](#g-13--costs-less-gas-than)| `>=`/`<=` costs less gas than `>`/`<` | 14 | 42 |
|[[G-14]](#g-14-internalprivate-functions-only-called-once-can-be-inlined-to-save-gas)| `internal/private` functions only called once can be inlined to save gas | 7 | 140 |
|[[G-15]](#g-15-function-names-can-be-optimized)| Function names can be optimized | 4 | 88 |
|[[G-16]](#g-16-using-delete-instead-of-setting-mappingstruct-to-0-saves-gas)| Using `delete` instead of setting mapping/struct to 0 saves gas | 2 | 10 |
|[[G-17]](#g-17-use-a-more-recent-version-of-solidity)| Use a more recent version of Solidity | 5 | - |
|[[G-18]](#g-18-constructors-can-be-marked-payable)| Constructors can be marked `payable` | 4 | 84 |
|[[G-19]](#g-19-nesting-if-statements-that-use--saves-gas)| Nesting `if` statements that use `&&` saves gas | 4 | 120 |
|[[G-20]](#g-20-lack-of-unchecked-in-loops)| Lack of `unchecked` in loops | 7 | 420 |
|[[G-21]](#g-21-use-assembly-to-check-for-address0)| Use assembly to check for `address(0)` | 12 | 72 |
|[[G-22]](#g-22-use-assembly-to-write-hashes)| Use assembly to write hashes | 4 | 480 |
|[[G-23]](#g-23-use-assembly-to-write-address-storage-values)| Use assembly to write `address` storage values | 8 | 592 |
|[[G-24]](#g-24-use-assembly-to-emit-an-event)| Use assembly to emit an `event` | 11 | 418 |

Total: 150 instances over 24 issues with an estimate of **50,062 gas** saved.

## Medium Risk Issues

---

### [M-01] Transferred `ERC721` can be stuck permanently

If the recipient is not a EOA, `safeTransferFrom` ensures that the contract is able to safely receive the token. In the worst-case scenario, it may result in tokens frozen permanently, as the following code uses `transferFrom`, which [doesn't check](https://github.com/ethereum/EIPs/blob/78e2c297611f5e92b6a5112819ab71f74041ff25/EIPS/eip-721.md?plain=1#L103-L113) if the recipient can handle the NFT.

*There are 2 instances of this issue.*


```solidity
File: src/DelegateToken.sol

369: 		            IERC721(underlyingContract).transferFrom(address(this), msg.sender, erc721UnderlyingTokenId);

393: 		            IERC721(info.tokenContract).transferFrom(address(this), info.receiver, info.tokenId);
```
[[369](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L369), [393](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L393)]


---

### [M-02] `unchecked` blocks with subtractions may underflow

There aren't any checks to avoid an underflow which can happen inside an `unchecked` block, so the following subtractions may underflow silently.

*There is 1 instance of this issue.*


```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

// @audit uint256(IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_AMOUNT))) - decreaseAmount
122: 		                uint256(IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_AMOUNT))) - decreaseAmount;
```
[[122](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L122)]


---

### [M-03] Some functions do not work correctly with fee-on-transfer tokens

Some tokens take a transfer fee (e.g. `STA`, `PAXG`), some do not currently charge a fee but may do so in the future (e.g. `USDT`, `USDC`).

Should a fee-on-transfer token be added as an asset and deposited, it could be abused, as the accounting is wrong. In the current implementation the following function calls do not work well with fee-on-transfer tokens as the amount variable is the pre-fee amount, including the fee, whereas the final balance do not include the fee anymore.

*There is 1 instance of this issue.*


```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

58: 		        SafeERC20.safeTransferFrom(IERC20(underlyingContract), msg.sender, address(this), pullAmount);
```
[[58](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L58)]


#### **Recommended Mitigation Steps**

- Consider comparing before and after balance to get the actual transferred amount.
- Alternatively, disallow tokens with fee-on-transfer mechanics to be added as valid tokens.

---

## Low Risk Issues

---

### [L-01] Avoid double casting

Consider refactoring the following code, as double casting may introduce unexpected truncations and/or rounding issues.

Furthermore, double type casting can make the code less readable and harder to maintain, increasing the likelihood of errors and misunderstandings during development and debugging.

*There are 3 instances of this issue.*


```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

// @audit uint256(uint160)
39: 		        delegateTokenInfo[delegateTokenId][PACKED_INFO_POSITION] = (uint256(uint160(approved)) << 96) | expiry;

// @audit uint256(uint160)
47: 		        delegateTokenInfo[delegateTokenId][PACKED_INFO_POSITION] = (uint256(uint160(approved)) << 96) | expiry;
```
[[39](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L39), [47](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L47)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

// @audit uint256(uint160)
154: 		        uint256 sc = uint256(uint160(0x0000000000000000000000000000000000000000));
```
[[154](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L154)]


---

### [L-02] Functions calling contracts with transfer hooks are missing reentrancy guards

Even if the function follows the best practice of check-effects-interaction, not using a reentrancy guard when there may be transfer hooks will open the users of this protocol up to read-only reentrancies with no way to protect against it, except by block-listing the whole protocol.

*There are 2 instances of this issue.*


```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

58: 		        SafeERC20.safeTransferFrom(IERC20(underlyingContract), msg.sender, address(this), pullAmount);

71: 		        IERC1155(underlyingContract).safeTransferFrom(msg.sender, address(this), underlyingTokenId, pullAmount, "");
```
[[58](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L58), [71](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L71)]


---

### [L-03] Large transfers may not work with some `ERC20` tokens

Some `IERC20` implementations (e.g `UNI`, `COMP`) may fail if the valued `transferred` is larger than `uint96`. [Source](https://github.com/d-xo/weird-erc20/blob/main/src/Uint96.sol).

*There are 2 instances of this issue.*


```solidity
File: src/DelegateToken.sol

375: 		            SafeERC20.safeTransfer(IERC20(underlyingContract), msg.sender, erc20UnderlyingAmount);

399: 		            SafeERC20.safeTransfer(IERC20(info.tokenContract), info.receiver, info.amount);
```
[[375](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L375), [399](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L399)]


---

### [L-04] Large approvals may not work with some `ERC20` tokens

Not all `IERC20` implementations are totally compliant, and some (e.g `UNI`, `COMP`) may fail if the valued passed to `approve` is larger than `uint96`. If the approval amount is `type(uint256).max`, which may cause issues with systems that expect the value passed to approve to be reflected in the allowances mapping.

*There is 1 instance of this issue.*


```solidity
File: src/CreateOfferer.sol

121: 		            if (!IERC20(erc20Order.info.tokenContract).approve(address(delegateToken), erc20Order.amount)) {
```
[[121](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L121)]


---

### [L-05] `approve` can revert if the current approval is not zero

Some tokens like USDT check for the current approval, and they revert if it's not zero. While Tether is known to do this, it applies to other tokens as well, which are trying to protect against [this](https://docs.google.com/document/d/1YLPtQxZu1UAvO9cZ1O2RPXBbT0mooh4DYKjA_jp-RLM/edit) attack vector.

*There is 1 instance of this issue.*


```solidity
File: src/CreateOfferer.sol

121: 		            if (!IERC20(erc20Order.info.tokenContract).approve(address(delegateToken), erc20Order.amount)) {
```
[[121](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L121)]


#### **Recommended Mitigation Steps**

Consider always calling `token.safeApprove(addr, 0)` before changing the approval, or better yet, use `safeIncreaseAllowance`/`safeDecreaseAllowance`.

---

### [L-06] NFT ownership doesn't support hard forks

To ensure clarity regarding the ownership of the NFT on a specific chain, it is recommended to add `require(block.chainid == 1, "Invalid Chain")` or the desired chain ID in the functions below.

Alternatively, consider including the chain ID in the URI itself. By doing so, any confusion regarding the chain responsible for owning the NFT will be eliminated.

*There is 1 instance of this issue.*


```solidity
File: src/PrincipalToken.sol

54: 		    function tokenURI(uint256 id) public view override returns (string memory) {
```
[[54](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L54)]


---

### [L-07] Missing disallowlist for `ERC721`

Lately, there has been a rise in cases where NFTs are being stolen. These stolen NFTs are then added to platforms, allowing them to be easily converted into liquidity.

Some popular marketplaces, such as Opensea, have already taken steps to combat this issue by introducing a disallowlist feature. This means that if an NFT is reported as stolen, it won't be listed or sold on their platform.

This may increase the project centralization, but it can help solve this problem, if this issue is a concern.

*There is 1 instance of this issue.*


```solidity
File: src/PrincipalToken.sol

11: 		contract PrincipalToken is ERC721("PrincipalToken", "PT") {
```
[[11](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L11)]


---

### [L-08] `unchecked` blocks with additions/multiplications may overflow

There aren't any checks to avoid an overflow which can happen inside an `unchecked` block, so the following expressions may overflow silently.

*There are 2 instances of this issue.*


```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

156: 		            availableAmount = loadAmount(delegateRegistry, RegistryHashes.erc20Hash(address(this), "flashloan", info.delegateHolder, info.tokenContract))
157: 		                + loadAmount(delegateRegistry, RegistryHashes.erc20Hash(address(this), "", info.delegateHolder, info.tokenContract));

165: 		            availableAmount = loadAmount(delegateRegistry, RegistryHashes.erc1155Hash(address(this), "flashloan", info.delegateHolder, info.tokenId, info.tokenContract))
166: 		                + loadAmount(delegateRegistry, RegistryHashes.erc1155Hash(address(this), "", info.delegateHolder, info.tokenId, info.tokenContract));
```
[[156-157](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L156-L157), [165-166](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L165-L166)]


---

### [L-09] Some functions contain the same exact logic

These functions might be a problem if the logic changes before the contract is deployed, as the developer must remember to syncronize the logic between all the function instances.

Consider using a single function instead of duplicating the code, for example by using a `library`, or through inheritance.

*There are 2 instances of this issue.*


```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

// @audit duplicated logic in lib/delegate-registry/src/DelegateRegistry.sol -> _writeDelegation, lib/delegate-registry/src/DelegateRegistry.sol -> _writeDelegation
344: 		    function _writeDelegation(bytes32 location, uint256 position, bytes32 data) internal {

// @audit duplicated logic in lib/delegate-registry/src/DelegateRegistry.sol -> _loadDelegationBytes32, lib/delegate-registry/src/DelegateRegistry.sol -> _loadDelegationUint
430: 		    function _loadDelegationBytes32(bytes32 location, uint256 position) internal view returns (bytes32 data) {
```
[[344](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L344), [430](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L430)]


---

### [L-10] Use of `transfer` instead of `safeTransfer`

It is good to add a `require` statement that checks the return value of token transfers, or to use something like OpenZeppelin's `safeTransfer`/`safeTransferFrom`, even if one is sure that the given token reverts in case of a failure.

This reduces the risk to zero even if these contracts are upgreadable, and it also helps with security reviews, as the auditor will not have to check this specific edge case.

*There are 3 instances of this issue.*


```solidity
File: src/DelegateToken.sol

369: 		            IERC721(underlyingContract).transferFrom(address(this), msg.sender, erc721UnderlyingTokenId);

393: 		            IERC721(info.tokenContract).transferFrom(address(this), info.receiver, info.tokenId);
```
[[369](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L369), [393](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L393)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

41: 		        IERC721(underlyingContract).transferFrom(msg.sender, address(this), underlyingTokenId);
```
[[41](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L41)]


---

### [L-11] External calls in an unbounded loop can result in a DoS

Consider limiting the number of iterations in loops that make external calls, as just a single one of them failing will result in a revert.

*There is 1 instance of this issue.*


```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

// @audit delegatecall (37)
35: 		            for (uint256 i = 0; i < data.length; ++i) {

```
[[35](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L35)]


---

### [L-12] Using zero as a parameter

Taking zero as a valid argument without checks can lead to severe security issues in some cases.

If using a zero argument is mandatory, consider using descriptive constants or an enum instead of passing zero directly on function calls, as that might be error-prone, to fully describe the caller's intention.

*There are 4 instances of this issue.*

```solidity
File: src/DelegateToken.sol

372: 		            StorageHelpers.writeUnderlyingAmount(delegateTokenInfo, delegateTokenId, 0); // Deletes amount

378: 		            StorageHelpers.writeUnderlyingAmount(delegateTokenInfo, delegateTokenId, 0); // Deletes amount
```
[[372](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L372), [378](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L378)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

145: 		            _writeDelegation(location, Storage.POSITIONS_AMOUNT, uint256(0));

279: 		                    delegations_[i] = Delegation({type_: DelegationType.NONE, to: address(0), from: address(0), rights: "", amount: 0, contract_: address(0), tokenId: 0});
```
[[145](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L145), [279](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L279)]


---

## Non Critical Issues

---

### [NC-01] Missing events in sensitive functions

Events should be emitted when sensitive changes are made to the contracts, but some functions lack them.

*There are 2 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/libraries/CreateOffererLib.sol

199: 		    function updateTransientState(
200: 		        CreateOffererStructs.TransientState storage transientState,
201: 		        address fulfiller,
202: 		        SpentItem calldata minimumReceived,
203: 		        SpentItem calldata maximumSpent,
204: 		        CreateOffererStructs.Context memory decodedContext
205: 		    ) internal {
206: 		        IDelegateRegistry.DelegationType tokenType = RegistryHashes.decodeType(bytes32(minimumReceived.identifier));
207: 		        if (tokenType == IDelegateRegistry.DelegationType.ERC721) {
208: 		            transientState.erc721Order = CreateOffererStructs.ERC721Order({
209: 		                tokenId: maximumSpent.identifier,
210: 		                info: CreateOffererStructs.Order({
211: 		                    rights: decodedContext.rights,
212: 		                    expiryLength: decodedContext.expiryLength,
213: 		                    signerSalt: decodedContext.signerSalt,
214: 		                    tokenContract: maximumSpent.token,
215: 		                    expiryType: decodedContext.expiryType,
216: 		                    targetToken: decodedContext.targetToken
217: 		                })
218: 		            });
219: 		        } else if (tokenType == IDelegateRegistry.DelegationType.ERC20) {
220: 		            transientState.erc20Order = CreateOffererStructs.ERC20Order({
221: 		                amount: maximumSpent.amount,
222: 		                info: CreateOffererStructs.Order({
223: 		                    rights: decodedContext.rights,
224: 		                    expiryLength: decodedContext.expiryLength,
225: 		                    signerSalt: decodedContext.signerSalt,
226: 		                    tokenContract: maximumSpent.token,
227: 		                    expiryType: decodedContext.expiryType,
228: 		                    targetToken: decodedContext.targetToken
229: 		                })
230: 		            });
231: 		        } else if (tokenType == IDelegateRegistry.DelegationType.ERC1155) {
232: 		            transientState.erc1155Order = CreateOffererStructs.ERC1155Order({
233: 		                amount: maximumSpent.amount,
234: 		                tokenId: maximumSpent.identifier,
235: 		                info: CreateOffererStructs.Order({
236: 		                    rights: decodedContext.rights,
237: 		                    expiryLength: decodedContext.expiryLength,
238: 		                    signerSalt: decodedContext.signerSalt,
239: 		                    tokenContract: maximumSpent.token,
240: 		                    expiryType: decodedContext.expiryType,
241: 		                    targetToken: decodedContext.targetToken
242: 		                })
243: 		            });
244: 		        } else {
245: 		            revert CreateOffererErrors.InvalidTokenType(tokenType);
246: 		        }
247: 		        transientState.receivers.fulfiller = fulfiller;
248: 		    }
```
[[199-248](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L199-L248)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

369: 		    function _updateFrom(bytes32 location, address from) internal {
370: 		        uint256 firstPacked = Storage.POSITIONS_FIRST_PACKED;
371: 		        uint256 cleanAddress = Storage.CLEAN_ADDRESS;
372: 		        uint256 cleanUpper12Bytes = type(uint256).max << 160;
373: 		        assembly {
374: 		            let slot := and(sload(add(location, firstPacked)), cleanUpper12Bytes)
375: 		            sstore(add(location, firstPacked), or(slot, and(from, cleanAddress)))
376: 		        }
377: 		    }
```
[[369-377](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L369-L377)]

</details>

---

### [NC-02] Unused named `return`

Declaring named returns, but not using them, is confusing to the reader. Consider either completely removing them (by declaring just the type without a name), or remove the return statement and do a variable assignment.

This would improve the readability of the code, and it may also help reduce regressions during future code refactors.

*There are 23 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/DelegateToken.sol

265: 		    function getDelegateInfo(uint256 delegateTokenId) external view returns (Structs.DelegateInfo memory delegateInfo) {
```
[[265](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L265)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

16: 		    function loadTokenHolder(address delegateRegistry, bytes32 registryHash) internal view returns (address delegateTokenHolder) {

18: 		            return RegistryStorage.unpackAddress(
19: 		                IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_SECOND_PACKED))
20: 		            );
```
[[16](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L16)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

300: 		    function readSlot(bytes32 location) external view returns (bytes32 contents) {

430: 		    function _loadDelegationBytes32(bytes32 location, uint256 position) internal view returns (bytes32 data) {

437: 		    function _loadDelegationUint(bytes32 location, uint256 position) internal view returns (uint256 data) {
```
[[300](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L300), [430](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L430), [437](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L437)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryHashes.sol

41: 		    function decodeType(bytes32 inputHash) internal pure returns (IDelegateRegistry.DelegationType decodedType) {

54: 		    function location(bytes32 inputHash) internal pure returns (bytes32 computedLocation) {

73: 		    function allHash(address from, bytes32 rights, address to) internal pure returns (bytes32 hash) {

95: 		    function allLocation(address from, bytes32 rights, address to) internal pure returns (bytes32 computedLocation) {

120: 		    function contractHash(address from, bytes32 rights, address to, address contract_) internal pure returns (bytes32 hash) {

143: 		    function contractLocation(address from, bytes32 rights, address to, address contract_) internal pure returns (bytes32 computedLocation) {

170: 		    function erc721Hash(address from, bytes32 rights, address to, uint256 tokenId, address contract_) internal pure returns (bytes32 hash) {

195: 		    function erc721Location(address from, bytes32 rights, address to, uint256 tokenId, address contract_) internal pure returns (bytes32 computedLocation) {

222: 		    function erc20Hash(address from, bytes32 rights, address to, address contract_) internal pure returns (bytes32 hash) {

245: 		    function erc20Location(address from, bytes32 rights, address to, address contract_) internal pure returns (bytes32 computedLocation) {

272: 		    function erc1155Hash(address from, bytes32 rights, address to, uint256 tokenId, address contract_) internal pure returns (bytes32 hash) {

297: 		    function erc1155Location(address from, bytes32 rights, address to, uint256 tokenId, address contract_) internal pure returns (bytes32 computedLocation) {
```
[[41](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L41), [54](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L54), [73](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L73), [95](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L95), [120](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L120), [143](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L143), [170](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L170), [195](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L195), [222](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L222), [245](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L245), [272](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L272), [297](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L297)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryOps.sol

6: 		    function max(uint256 x, uint256 y) internal pure returns (uint256 z) {

19: 		    function and(bool x, bool y) internal pure returns (bool z) {

26: 		    function or(bool x, bool y) internal pure returns (bool z) {
```
[[6](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L6), [19](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L19), [26](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L26)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryStorage.sol

34: 		    function packAddresses(address from, address to, address contract_) internal pure returns (bytes32 firstPacked, bytes32 secondPacked) {

50: 		    function unpackAddresses(bytes32 firstPacked, bytes32 secondPacked) internal pure returns (address from, address to, address contract_) {

64: 		    function unpackAddress(bytes32 packedSlot) internal pure returns (address unpacked) {
```
[[34](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L34), [50](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L50), [64](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L64)]

</details>

---

### [NC-03] Consider using `ERC721A` instead of `ERC721`

[ERC721A](https://www.erc721a.org/) is an implementation of IERC721 with significant gas savings for minting multiple NFTs in a single transaction.

*There is 1 instance of this issue.*


```solidity
File: src/PrincipalToken.sol

11: 		contract PrincipalToken is ERC721("PrincipalToken", "PT") {
```
[[11](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L11)]


---

### [NC-04] Enum values should be used in place of constant array indexes

Consider using an enum instead of hardcoding an index access to make the code easier to understand.

*There are 22 instances of this issue.*


```solidity
File: src/CreateOfferer.sol

61: 		        Helpers.updateTransientState(transientState, fulfiller, minimumReceived[0], maximumSpent[0], decodedContext);

61: 		        Helpers.updateTransientState(transientState, fulfiller, minimumReceived[0], maximumSpent[0], decodedContext);

78: 		        Helpers.verifyCreate(delegateToken, offer[0].identifier, transientState.receivers, consideration[0], context);

78: 		        Helpers.verifyCreate(delegateToken, offer[0].identifier, transientState.receivers, consideration[0], context);
```
[[61](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L61), [61](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L61), [78](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L78), [78](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L78)]



```solidity
File: src/libraries/CreateOffererLib.sol

352: 		        if (minimumReceived[0].itemType != ItemType.ERC721 || minimumReceived[0].token != address(this) || minimumReceived[0].amount != 1) {

352: 		        if (minimumReceived[0].itemType != ItemType.ERC721 || minimumReceived[0].token != address(this) || minimumReceived[0].amount != 1) {

352: 		        if (minimumReceived[0].itemType != ItemType.ERC721 || minimumReceived[0].token != address(this) || minimumReceived[0].amount != 1) {

353: 		            revert CreateOffererErrors.MinimumReceivedInvalid(minimumReceived[0]);

355: 		        if (maximumSpent[0].itemType != ItemType.ERC721 && maximumSpent[0].itemType != ItemType.ERC20 && maximumSpent[0].itemType != ItemType.ERC1155) {

355: 		        if (maximumSpent[0].itemType != ItemType.ERC721 && maximumSpent[0].itemType != ItemType.ERC20 && maximumSpent[0].itemType != ItemType.ERC1155) {

355: 		        if (maximumSpent[0].itemType != ItemType.ERC721 && maximumSpent[0].itemType != ItemType.ERC20 && maximumSpent[0].itemType != ItemType.ERC1155) {

356: 		            revert CreateOffererErrors.MaximumSpentInvalid(maximumSpent[0]);

359: 		        offer[0] = SpentItem({itemType: minimumReceived[0].itemType, token: minimumReceived[0].token, identifier: minimumReceived[0].identifier, amount: minimumReceived[0].amount});

359: 		        offer[0] = SpentItem({itemType: minimumReceived[0].itemType, token: minimumReceived[0].token, identifier: minimumReceived[0].identifier, amount: minimumReceived[0].amount});

359: 		        offer[0] = SpentItem({itemType: minimumReceived[0].itemType, token: minimumReceived[0].token, identifier: minimumReceived[0].identifier, amount: minimumReceived[0].amount});

359: 		        offer[0] = SpentItem({itemType: minimumReceived[0].itemType, token: minimumReceived[0].token, identifier: minimumReceived[0].identifier, amount: minimumReceived[0].amount});

359: 		        offer[0] = SpentItem({itemType: minimumReceived[0].itemType, token: minimumReceived[0].token, identifier: minimumReceived[0].identifier, amount: minimumReceived[0].amount});

361: 		        consideration[0] = ReceivedItem({

362: 		            itemType: maximumSpent[0].itemType,

363: 		            token: maximumSpent[0].token,

364: 		            identifier: maximumSpent[0].identifier,

365: 		            amount: maximumSpent[0].amount,
```
[[352](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L352), [352](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L352), [352](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L352), [353](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L353), [355](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L355), [355](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L355), [355](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L355), [356](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L356), [359](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L359), [359](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L359), [359](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L359), [359](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L359), [359](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L359), [361](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L361), [362](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L362), [363](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L363), [364](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L364), [365](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L365)]


---

### [NC-05] Variable initialization with default value

It's not necessary to initialize a variable with its default value, and it's actually worse in gas terms as it adds an overhead.

*There are 17 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/DelegateToken.sol

175: 		        bytes32 newRegistryHash = 0;

305: 		        bytes32 newRegistryHash = 0;
```
[[175](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L175), [305](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L305)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

153: 		        uint256 availableAmount = 0;

163: 		        uint256 availableAmount = 0;
```
[[153](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L153), [163](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L163)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

15: 		    uint256 internal constant ID_AVAILABLE = 0;

22: 		    uint256 internal constant REGISTRY_HASH_POSITION = 0;
```
[[15](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L15), [22](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L22)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

35: 		            for (uint256 i = 0; i < data.length; ++i) {

275: 		            for (uint256 i = 0; i < hashes.length; ++i) {

312: 		            for (uint256 i = 0; i < length; ++i) {

381: 		        uint256 count = 0;

386: 		            for (uint256 i = 0; i < hashesLength; ++i) {

393: 		            for (uint256 i = 0; i < count; ++i) {

412: 		        uint256 count = 0;

417: 		            for (uint256 i = 0; i < hashesLength; ++i) {

423: 		            for (uint256 i = 0; i < count; ++i) {
```
[[35](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L35), [275](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L275), [312](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L312), [381](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L381), [386](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L386), [393](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L393), [412](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L412), [417](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L417), [423](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L423)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryHashes.sol

31: 		    uint256 internal constant DELEGATION_SLOT = 0;
```
[[31](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L31)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryStorage.sol

10: 		    uint256 internal constant POSITIONS_FIRST_PACKED = 0; //  | 4 bytes empty | first 8 bytes of contract address | 20 bytes of from address |
```
[[10](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L10)]

</details>

---

### [NC-06] Duplicated `require/if` statements should be refactored

These statements should be refactored to a separate function, as there are multiple parts of the codebase that use the same logic, to improve the code readability and reduce code duplication.

*There are 2 instances of this issue.*


```solidity
File: src/CreateOfferer.sol

// @audit this if condition is duplicated on line 182
58: 		        if (context.length != 160) revert Errors.InvalidContextLength();
```
[[58](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L58)]



```solidity
File: src/DelegateToken.sol

// @audit this if condition is duplicated on line 107
100: 		        if (delegateTokenHolder == address(0)) revert Errors.DelegateTokenHolderZero();
```
[[100](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L100)]


---

### [NC-07] Unbounded loop may run out of gas

Consider limiting the number of iterations in loops with an explicit revert reason to avoid iterating an array that is too large.

The function would eventually revert if out of gas anyway, but by limiting it the user avoids wasting too much gas, as the loop doesn't execute if an excessive value is provided.

*There are 7 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

35: 		            for (uint256 i = 0; i < data.length; ++i) {
36: 		                //slither-disable-next-line calls-loop,delegatecall-loop
37: 		                (success, results[i]) = address(this).delegatecall(data[i]);
38: 		                if (!success) revert MulticallFailed();
39: 		            }

275: 		            for (uint256 i = 0; i < hashes.length; ++i) {
276: 		                bytes32 location = Hashes.location(hashes[i]);
277: 		                address from = _loadFrom(location);
278: 		                if (_invalidFrom(from)) {
279: 		                    delegations_[i] = Delegation({type_: DelegationType.NONE, to: address(0), from: address(0), rights: "", amount: 0, contract_: address(0), tokenId: 0});
280: 		                } else {
281: 		                    (, address to, address contract_) = _loadDelegationAddresses(location);
282: 		                    delegations_[i] = Delegation({
283: 		                        type_: Hashes.decodeType(hashes[i]),
284: 		                        to: to,
285: 		                        from: from,
286: 		                        rights: _loadDelegationBytes32(location, Storage.POSITIONS_RIGHTS),
287: 		                        amount: _loadDelegationUint(location, Storage.POSITIONS_AMOUNT),
288: 		                        contract_: contract_,
289: 		                        tokenId: _loadDelegationUint(location, Storage.POSITIONS_TOKEN_ID)
290: 		                    });
291: 		                }
292: 		            }

312: 		            for (uint256 i = 0; i < length; ++i) {
313: 		                tempLocation = locations[i];
314: 		                assembly {
315: 		                    tempValue := sload(tempLocation)
316: 		                }
317: 		                contents[i] = tempValue;
318: 		            }

386: 		            for (uint256 i = 0; i < hashesLength; ++i) {
387: 		                hash = hashes[i];
388: 		                if (_invalidFrom(_loadFrom(Hashes.location(hash)))) continue;
389: 		                filteredHashes[count++] = hash;
390: 		            }

393: 		            for (uint256 i = 0; i < count; ++i) {
394: 		                hash = filteredHashes[i];
395: 		                location = Hashes.location(hash);
396: 		                (address from, address to, address contract_) = _loadDelegationAddresses(location);
397: 		                delegations_[i] = Delegation({
398: 		                    type_: Hashes.decodeType(hash),
399: 		                    to: to,
400: 		                    from: from,
401: 		                    rights: _loadDelegationBytes32(location, Storage.POSITIONS_RIGHTS),
402: 		                    amount: _loadDelegationUint(location, Storage.POSITIONS_AMOUNT),
403: 		                    contract_: contract_,
404: 		                    tokenId: _loadDelegationUint(location, Storage.POSITIONS_TOKEN_ID)
405: 		                });
406: 		            }

417: 		            for (uint256 i = 0; i < hashesLength; ++i) {
418: 		                hash = hashes[i];
419: 		                if (_invalidFrom(_loadFrom(Hashes.location(hash)))) continue;
420: 		                filteredHashes[count++] = hash;
421: 		            }

423: 		            for (uint256 i = 0; i < count; ++i) {
424: 		                validHashes[i] = filteredHashes[i];
425: 		            }
```
[[35-39](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L35-L39), [275-292](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L275-L292), [312-318](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L312-L318), [386-390](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L386-L390), [393-406](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L393-L406), [417-421](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L417-L421), [423-425](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L423-L425)]

</details>

---

### [NC-08] Use of non-named numeric constants

Constants should be defined instead of using magic numbers.

*There are 17 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/CreateOfferer.sol

58: 		        if (context.length != 160) revert Errors.InvalidContextLength();

182: 		        if (context.length != 160) revert Errors.InvalidContextLength();
```
[[58](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L58), [182](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L182)]



```solidity
File: src/DelegateToken.sol

66: 		        return interfaceId == 0x2a55205a // ERC165 Interface ID for ERC2981

67: 		            || interfaceId == 0x01ffc9a7 // ERC165 Interface ID for ERC165

68: 		            || interfaceId == 0x80ac58cd // ERC165 Interface ID for ERC721

69: 		            || interfaceId == 0x5b5e139f // ERC165 Interface ID for ERC721Metadata

70: 		            || interfaceId == 0x4e2312e0; // ERC165 Interface ID for ERC1155 Token receiver
```
[[66](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L66), [67](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L67), [68](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L68), [69](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L69), [70](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L70)]



```solidity
File: src/libraries/CreateOffererLib.sol

297: 		        if (context.length != 160) revert CreateOffererErrors.InvalidContextLength();

399: 		        return (hashWithoutType << 8) | uint256(tokenType);
```
[[297](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L297), [399](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L399)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

39: 		        delegateTokenInfo[delegateTokenId][PACKED_INFO_POSITION] = (uint256(uint160(approved)) << 96) | expiry;

46: 		        address approved = address(uint160(delegateTokenInfo[delegateTokenId][PACKED_INFO_POSITION] >> 96));

47: 		        delegateTokenInfo[delegateTokenId][PACKED_INFO_POSITION] = (uint256(uint160(approved)) << 96) | expiry;

128: 		        return address(uint160(delegateTokenInfo[delegateTokenId][PACKED_INFO_POSITION] >> 96));
```
[[39](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L39), [46](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L46), [47](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L47), [128](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L128)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

330: 		        return Ops.or(interfaceId == type(IDelegateRegistry).interfaceId, interfaceId == 0x01ffc9a7);

372: 		        uint256 cleanUpper12Bytes = type(uint256).max << 160;
```
[[330](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L330), [372](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L372)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryStorage.sol

20: 		    uint256 internal constant CLEAN_FIRST8_BYTES_ADDRESS = 0xffffffffffffffff << 96;

23: 		    uint256 internal constant CLEAN_PACKED8_BYTES_ADDRESS = 0xffffffffffffffff << 160;
```
[[20](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L20), [23](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L23)]

</details>

---

### [NC-09] Control structures do not comply with best practices

This is a [best practice](https://docs.soliditylang.org/en/latest/style-guide.html#control-structures) that should be followed. 

*There are 59 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/CreateOfferer.sol

30: 		        if (parameters.delegateToken == address(0)) revert Errors.DelegateTokenIsZero();

32: 		        if (parameters.principalToken == address(0)) revert Errors.PrincipalTokenIsZero();

58: 		        if (context.length != 160) revert Errors.InvalidContextLength();

90: 		        if (from != address(this)) revert Errors.FromNotCreateOfferer(from);

182: 		        if (context.length != 160) revert Errors.InvalidContextLength();
```
[[30](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L30), [32](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L32), [58](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L58), [90](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L90), [182](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L182)]



```solidity
File: src/DelegateToken.sol

53: 		        if (parameters.delegateRegistry == address(0)) revert Errors.DelegateRegistryZero();

54: 		        if (parameters.principalToken == address(0)) revert Errors.PrincipalTokenZero();

55: 		        if (parameters.marketMetadata == address(0)) revert Errors.MarketMetadataZero();

84: 		        if (address(this) == operator) return IERC721Receiver.onERC721Received.selector;

100: 		        if (delegateTokenHolder == address(0)) revert Errors.DelegateTokenHolderZero();

107: 		        if (delegateTokenHolder == address(0)) revert Errors.DelegateTokenHolderZero();

162: 		        if (to == address(0)) revert Errors.ToIsZero();

166: 		        if (from != delegateTokenHolder) revert Errors.FromNotDelegateTokenHolder();

273: 		        if (delegateInfo.tokenType == IDelegateRegistry.DelegationType.ERC20) delegateInfo.tokenId = 0;

275: 		        if (delegateInfo.tokenType == IDelegateRegistry.DelegationType.ERC721) delegateInfo.amount = 0;

299: 		        if (delegateInfo.delegateHolder == address(0)) revert Errors.ToIsZero();

329: 		        if (newExpiry <= previousExpiry) revert Errors.ExpiryTooSmall();
```
[[53](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L53), [54](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L54), [55](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L55), [84](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L84), [100](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L100), [107](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L107), [162](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L162), [166](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L166), [273](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L273), [275](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L275), [299](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L299), [329](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L329)]



```solidity
File: src/PrincipalToken.sol

21: 		        if (setDelegateToken == address(0)) revert DelegateTokenZero();

23: 		        if (setMarketMetadata == address(0)) revert MarketMetadataZero();

28: 		        if (msg.sender == delegateToken) return;
```
[[21](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L21), [23](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L23), [28](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L28)]



```solidity
File: src/libraries/CreateOffererLib.sol

146: 		        if (setSeaport == address(0)) revert CreateOffererErrors.SeaportIsZero();

158: 		        if (cacheStage.lock != CreateOffererEnums.Lock.unlocked) revert CreateOffererErrors.Locked();

159: 		        if (cacheStage.flag != currentStage) revert CreateOffererErrors.WrongStage(currentStage, cacheStage.flag);

170: 		        if (caller != seaport) revert CreateOffererErrors.CallerNotSeaport(caller);

185: 		        if (nonce.value != contractNonce) revert CreateOffererErrors.InvalidContractNonce(nonce.value, contractNonce);

297: 		        if (context.length != 160) revert CreateOffererErrors.InvalidContextLength();

300: 		        if (

351: 		        if (!(minimumReceived.length == 1 && maximumSpent.length == 1)) revert CreateOffererErrors.NoBatchWrapping();
```
[[146](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L146), [158](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L158), [159](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L159), [170](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L170), [185](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L185), [297](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L297), [300](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L300), [351](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L351)]



```solidity
File: src/libraries/DelegateTokenLib.sol

92: 		        if (IDelegateFlashloan(info.receiver).onFlashloan{value: msg.value}(msg.sender, info) == IDelegateFlashloan.onFlashloan.selector) return;

97: 		        if (to.code.length == 0 || IERC721Receiver(to).onERC721Received(msg.sender, from, delegateTokenId, data) == IERC721Receiver.onERC721Received.selector) return;

102: 		        if (to.code.length == 0 || IERC721Receiver(to).onERC721Received(msg.sender, from, delegateTokenId, "") == IERC721Receiver.onERC721Received.selector) return;

109: 		        if (expiry > block.timestamp) return;
```
[[92](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L92), [97](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L97), [102](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L102), [109](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L109)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

145: 		        if (

159: 		        if (info.amount > availableAmount) revert Errors.ERC20FlashAmountUnavailable();

184: 		        if (

204: 		        if (

241: 		        if (

251: 		        if (

262: 		        if (

299: 		        if (

318: 		        if (
```
[[145](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L145), [159](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L159), [184](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L184), [204](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L204), [241](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L241), [251](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L251), [262](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L262), [299](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L299), [318](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L318)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

45: 		        if (expiry > MAX_EXPIRY) revert Errors.ExpiryTooLarge();

98: 		        if (principalBurnAuthorization.flag == BURN_AUTHORIZED) return;

106: 		        if (principalMintAuthorization.flag == MINT_AUTHORIZED) return;

113: 		        if (msg.sender == principalToken) return;

118: 		        if (delegateTokenInfo[delegateTokenId][REGISTRY_HASH_POSITION] == ID_AVAILABLE) return;

123: 		        if (msg.sender == account || accountOperator[account][msg.sender]) return;

149: 		        if (msg.sender == account || accountOperator[account][msg.sender] || msg.sender == readApproved(delegateTokenInfo, delegateTokenId)) return;
```
[[45](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L45), [98](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L98), [106](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L106), [113](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L113), [118](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L118), [123](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L123), [149](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L149)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

62: 		        if (pullAmount == 0) revert Errors.WrongAmountForType(IDelegateRegistry.DelegationType.ERC1155, pullAmount);

86: 		        if (!checkERC1155Pulled(erc1155PullAuthorization, operator)) revert Errors.ERC1155PullNotRequested(operator);
```
[[62](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L62), [86](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L86)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

38: 		                if (!success) revert MulticallFailed();

52: 		                if (rights != "") _writeDelegation(location, Storage.POSITIONS_RIGHTS, rights);

71: 		                if (rights != "") _writeDelegation(location, Storage.POSITIONS_RIGHTS, rights);

91: 		                if (rights != "") _writeDelegation(location, Storage.POSITIONS_RIGHTS, rights);

111: 		                if (rights != "") _writeDelegation(location, Storage.POSITIONS_RIGHTS, rights);

136: 		                if (rights != "") _writeDelegation(location, Storage.POSITIONS_RIGHTS, rights);

168: 		            if (!Ops.or(rights == "", valid)) valid = _validateFrom(Hashes.allLocation(from, rights, to), from);

388: 		                if (_invalidFrom(_loadFrom(Hashes.location(hash)))) continue;

419: 		                if (_invalidFrom(_loadFrom(Hashes.location(hash)))) continue;
```
[[38](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L38), [52](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L52), [71](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L71), [91](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L91), [111](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L111), [136](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L136), [168](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L168), [388](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L388), [419](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L419)]

</details>

---

### [NC-10] Use a single file for system wide constants

Consider grouping all the system constants under a single file. This finding shows only the first constant for each file, for brevity.

*There are 4 instances of this issue.*


```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

9: 		    uint256 internal constant MAX_EXPIRY = type(uint96).max;
```
[[9](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L9)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

12: 		    uint256 internal constant ERC1155_NOT_PULLED = 5;
```
[[12](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L12)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryHashes.sol

23: 		    uint256 internal constant EXTRACT_LAST_BYTE = 0xff;
```
[[23](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L23)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryStorage.sol

6: 		    address internal constant DELEGATION_EMPTY = address(0);
```
[[6](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L6)]


---

### [NC-11] Old Solidity version

Use a more recent version of Solidity: the latest version is 0.8.21, but it's safer to use at least the version 0.8.19 to get the latest bugfixes and features when deploying on L2.

*There are 5 instances of this issue.*


```solidity
File: src/libraries/CreateOffererLib.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L2)]



```solidity
File: src/libraries/DelegateTokenLib.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L2)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L2)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L2)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L2)]


---

### [NC-12] Use of floating pragma

Locking the pragma helps avoid accidental deploys with an outdated compiler version that may introduce bugs and unexpected vulnerabilities.

Floating pragma is meant to be used for libraries and contracts that have external users and need backward compatibility.

*There are 4 instances of this issue.*


```solidity
File: src/CreateOfferer.sol

2: 		pragma solidity ^0.8.21;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L2)]



```solidity
File: src/DelegateToken.sol

2: 		pragma solidity ^0.8.21;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L2)]



```solidity
File: src/PrincipalToken.sol

2: 		pragma solidity ^0.8.21;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L2)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

2: 		pragma solidity ^0.8.21;
```
[[2](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L2)]


---

### [NC-13] No checks for empty bytes

Like the zero-address check, an empty bytes assignment might be undesiderable, but the following functions don't have it.

*There is 1 instance of this issue.*


```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

// @audit location
369: 		    function _updateFrom(bytes32 location, address from) internal {
```
[[369](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L369)]


---

### [NC-14] Contract functions should use an `interface`

All `external`/`public` functions should extend an `interface`. This is useful to make sure that the whole API is extracted.

*There are 48 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/CreateOfferer.sol

52: 		    function generateOrder(address fulfiller, SpentItem[] calldata minimumReceived, SpentItem[] calldata maximumSpent, bytes calldata context)

71: 		    function ratifyOrder(SpentItem[] calldata offer, ReceivedItem[] calldata consideration, bytes calldata context, bytes32[] calldata, uint256 contractNonce)

89: 		    function transferFrom(address from, address targetTokenReceiver, uint256 createOrderHashAsTokenId) external checkStage(Enums.Stage.transfer, Enums.Stage.ratify) {

176: 		    function previewOrder(address caller, address, SpentItem[] calldata minimumReceived, SpentItem[] calldata maximumSpent, bytes calldata context)

195: 		    function calculateERC721OrderHashAndId(address targetTokenReceiver, address conduit, Structs.ERC721Order calldata erc721Order)

213: 		    function calculateERC20OrderHashAndId(address targetTokenReceiver, address conduit, Structs.ERC20Order calldata erc20Order)

231: 		    function calculateERC1155OrderHashAndId(address targetTokenReceiver, address conduit, Structs.ERC1155Order calldata erc1155Order)

241: 		    function getSeaportMetadata() external pure returns (string memory, Schema[] memory) {
```
[[52](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L52), [71](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L71), [89](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L89), [176](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L176), [195](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L195), [213](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L213), [231](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L231), [241](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L241)]



```solidity
File: src/DelegateToken.sol

65: 		    function supportsInterface(bytes4 interfaceId) external pure returns (bool) {

78: 		    function onERC1155BatchReceived(address, address, uint256[] calldata, uint256[] calldata, bytes calldata) external pure returns (bytes4) {

83: 		    function onERC721Received(address operator, address, uint256, bytes calldata) external view returns (bytes4) {

89: 		    function onERC1155Received(address operator, address, uint256, uint256, bytes calldata) external returns (bytes4) {

99: 		    function balanceOf(address delegateTokenHolder) external view returns (uint256) {

105: 		    function ownerOf(uint256 delegateTokenId) external view returns (address delegateTokenHolder) {

111: 		    function getApproved(uint256 delegateTokenId) external view returns (address) {

117: 		    function isApprovedForAll(address account, address operator) external view returns (bool) {

122: 		    function safeTransferFrom(address from, address to, uint256 delegateTokenId, bytes calldata data) external {

128: 		    function safeTransferFrom(address from, address to, uint256 delegateTokenId) external {

134: 		    function approve(address spender, uint256 delegateTokenId) external {

144: 		    function setApprovalForAll(address operator, bool approved) external {

161: 		    function transferFrom(address from, address to, uint256 delegateTokenId) public {

217: 		    function name() external pure returns (string memory) {

222: 		    function symbol() external pure returns (string memory) {

227: 		    function tokenURI(uint256 delegateTokenId) external view returns (string memory) {

239: 		    function isApprovedOrOwner(address spender, uint256 delegateTokenId) external view returns (bool) {

247: 		    function baseURI() external view returns (string memory) {

252: 		    function contractURI() external view returns (string memory) {

256: 		    function royaltyInfo(uint256 tokenId, uint256 salePrice) external view returns (address receiver, uint256 royaltyAmount) {

265: 		    function getDelegateInfo(uint256 delegateTokenId) external view returns (Structs.DelegateInfo memory delegateInfo) {

280: 		    function getDelegateId(address caller, uint256 salt) external view returns (uint256 delegateTokenId) {

286: 		    function burnAuthorizedCallback() external view {

291: 		    function mintAuthorizedCallback() external view {

296: 		    function create(Structs.DelegateInfo calldata delegateInfo, uint256 salt) external nonReentrant returns (uint256 delegateTokenId) {

325: 		    function extend(uint256 delegateTokenId, uint256 newExpiry) external {

339: 		    function rescind(uint256 delegateTokenId) external {

353: 		    function withdraw(uint256 delegateTokenId) external nonReentrant {

389: 		    function flashloan(Structs.FlashInfo calldata info) external payable nonReentrant {
```
[[65](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L65), [78](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L78), [83](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L83), [89](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L89), [99](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L99), [105](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L105), [111](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L111), [117](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L117), [122](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L122), [128](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L128), [134](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L134), [144](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L144), [161](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L161), [217](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L217), [222](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L222), [227](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L227), [239](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L239), [247](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L247), [252](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L252), [256](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L256), [265](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L265), [280](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L280), [286](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L286), [291](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L291), [296](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L296), [325](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L325), [339](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L339), [353](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L353), [389](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L389)]



```solidity
File: src/PrincipalToken.sol

33: 		    function mint(address to, uint256 id) external {

40: 		    function burn(address spender, uint256 id) external {

50: 		    function isApprovedOrOwner(address account, uint256 id) external view returns (bool) {
```
[[33](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L33), [40](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L40), [50](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L50)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

151: 		    function sweep() external {

257: 		    function getOutgoingDelegations(address from) external view returns (Delegation[] memory delegations_) {

262: 		    function getIncomingDelegationHashes(address to) external view returns (bytes32[] memory delegationHashes) {

267: 		    function getOutgoingDelegationHashes(address from) external view returns (bytes32[] memory delegationHashes) {

272: 		    function getDelegationsFromHashes(bytes32[] calldata hashes) external view returns (Delegation[] memory delegations_) {

300: 		    function readSlot(bytes32 location) external view returns (bytes32 contents) {

306: 		    function readSlots(bytes32[] calldata locations) external view returns (bytes32[] memory contents) {

329: 		    function supportsInterface(bytes4 interfaceId) external pure returns (bool) {
```
[[151](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L151), [257](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L257), [262](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L262), [267](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L267), [272](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L272), [300](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L300), [306](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L306), [329](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L329)]

</details>

---

### [NC-15] Multiple `address`/ID mappings can be combined into a single mapping of an `address`/ID to a `struct`, for readability

Well-organized data structures make code reviews easier, which may lead to fewer bugs. Consider combining related mappings into mappings to structs, so it's clear what data is related.

*There is 1 instance of this issue.*


```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

// @audit consider merging outgoingDelegationHashes, incomingDelegationHashes
21: 		    mapping(address from => bytes32[] delegationHashes) internal outgoingDelegationHashes;

24: 		    mapping(address to => bytes32[] delegationHashes) internal incomingDelegationHashes;
```
[[21](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L21)]


---

### [NC-16] Imports should be organized more systematically

The contract's interface should be imported first, followed by each of the interfaces it uses, followed by all other files. The examples below do not follow this layout.

*There are 3 instances of this issue.*


```solidity
File: src/CreateOfferer.sol

11: 		import {ContractOffererInterface, SpentItem, ReceivedItem, Schema} from "seaport/contracts/interfaces/ContractOffererInterface.sol";
```
[[11](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L11)]



```solidity
File: src/DelegateToken.sol

8: 		import {ReentrancyGuard} from "openzeppelin/security/ReentrancyGuard.sol";
```
[[8](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L8)]



```solidity
File: src/PrincipalToken.sol

6: 		import {ERC721} from "openzeppelin-contracts/contracts/token/ERC721/ERC721.sol";
```
[[6](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L6)]


---

### [NC-17] Event is missing `msg.sender` parameter

The following functions are missing some parameters when emitting an event: when dealing with a source address which uses the value of `msg.sender`, the `msg.sender` value should be specified in every event.

Otherwise, a contract or web page listening to events cannot react to connected users: basically, those events cannot be used properly.

*There are 3 instances of this issue.*


```solidity
File: src/DelegateToken.sol

304: 		        emit Transfer(address(0), delegateInfo.delegateHolder, delegateTokenId);

332: 		            emit ExpiryExtended(delegateTokenId, previousExpiry, newExpiry);

362: 		        emit Transfer(delegateTokenHolder, address(0), delegateTokenId);
```
[[304](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L304), [332](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L332), [362](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L362)]


---

### [NC-18] Unresolved `TODOs` in comments

Some features might not be properly implemented, as there are commented `TODOs`. Review the comments to ensure that everything is implemented, and remove them before deploying.

*There is 1 instance of this issue.*


```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

152: 		        // TODO: Replace this with correct address at deployment time
```
[[152](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L152)]


---

### [NC-19] Use of polymorphism is discouraged for security audits

A duplicated function name in the same contract might have problems with automated auditing tools, so it should be avoided. Consider always using a different name for functions to improve the readability of the code.

*There are 4 instances of this issue.*


```solidity
File: src/DelegateToken.sol

// @audit found also on line 122
128: 		    function safeTransferFrom(address from, address to, uint256 delegateTokenId) external {
```
[[128](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L128)]



```solidity
File: src/libraries/DelegateTokenLib.sol

// @audit found also on line 96
101: 		    function revertOnInvalidERC721ReceiverCallback(address from, address to, uint256 delegateTokenId) internal {
```
[[101](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L101)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

// @audit found also on line 170
178: 		    function revertNotMinted(bytes32 registryHash, uint256 delegateTokenId) internal pure {
```
[[178](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L178)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

// @audit found also on line 344
351: 		    function _writeDelegation(bytes32 location, uint256 position, uint256 data) internal {
```
[[351](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L351)]


---

### [NC-20] Custom `error` without details

Consider adding some parameters to the error to indicate which user or values caused the failure.

*There are 35 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/PrincipalToken.sol

15: 		    error DelegateTokenZero();

16: 		    error MarketMetadataZero();

17: 		    error CallerNotDelegateToken();
```
[[15](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L15), [16](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L16), [17](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L17)]



```solidity
File: src/libraries/CreateOffererLib.sol

11: 		    error DelegateTokenIsZero();

12: 		    error PrincipalTokenIsZero();

14: 		    error NoBatchWrapping();

16: 		    error SeaportIsZero();

17: 		    error Locked();

28: 		    error DelegateInfoInvariant();

29: 		    error InvalidContextLength();
```
[[11](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L11), [12](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L12), [14](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L14), [16](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L16), [17](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L17), [28](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L28), [29](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L29)]



```solidity
File: src/libraries/DelegateTokenLib.sol

43: 		    error DelegateRegistryZero();

44: 		    error PrincipalTokenZero();

45: 		    error DelegateTokenHolderZero();

46: 		    error MarketMetadataZero();

47: 		    error ToIsZero();

49: 		    error NotERC721Receiver();

50: 		    error InvalidERC721TransferOperator();

52: 		    error BatchERC1155TransferUnsupported();

54: 		    error InsufficientAllowanceOrInvalidToken();

55: 		    error CallerNotOwnerOrInvalidToken();

60: 		    error FromNotDelegateTokenHolder();

62: 		    error HashMismatch();

68: 		    error ExpiryInPast();

69: 		    error ExpiryTooLarge();

70: 		    error ExpiryTooSmall();

76: 		    error ERC721FlashUnavailable();

77: 		    error ERC20FlashAmountUnavailable();

78: 		    error ERC1155FlashAmountUnavailable();

80: 		    error BurnNotAuthorized();

81: 		    error MintNotAuthorized();

82: 		    error CallerNotPrincipalToken();

83: 		    error BurnAuthorized();

84: 		    error MintAuthorized();

86: 		    error ERC1155Pulled();

87: 		    error ERC1155NotPulled();
```
[[43](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L43), [44](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L44), [45](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L45), [46](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L46), [47](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L47), [49](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L49), [50](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L50), [52](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L52), [54](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L54), [55](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L55), [60](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L60), [62](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L62), [68](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L68), [69](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L69), [70](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L70), [76](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L76), [77](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L77), [78](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L78), [80](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L80), [81](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L81), [82](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L82), [83](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L83), [84](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L84), [86](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L86), [87](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L87)]

</details>

---

### [NC-21] Constants in comparisons should appear on the left side

This is useful to avoid doing some [typo bugs](https://www.moserware.com/2008/01/constants-on-left-are-better-but-this.html).

*There are 21 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/CreateOfferer.sol

58: 		        if (context.length != 160) revert Errors.InvalidContextLength();

138: 		            if (IERC20(erc20Order.info.tokenContract).allowance(address(this), address(delegateToken)) != 0) {

182: 		        if (context.length != 160) revert Errors.InvalidContextLength();
```
[[58](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L58), [138](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L138), [182](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L182)]



```solidity
File: src/DelegateToken.sol

66: 		        return interfaceId == 0x2a55205a // ERC165 Interface ID for ERC2981

67: 		            || interfaceId == 0x01ffc9a7 // ERC165 Interface ID for ERC165

68: 		            || interfaceId == 0x80ac58cd // ERC165 Interface ID for ERC721

69: 		            || interfaceId == 0x5b5e139f // ERC165 Interface ID for ERC721Metadata

70: 		            || interfaceId == 0x4e2312e0; // ERC165 Interface ID for ERC1155 Token receiver
```
[[66](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L66), [67](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L67), [68](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L68), [69](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L69), [70](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L70)]



```solidity
File: src/libraries/CreateOffererLib.sol

297: 		        if (context.length != 160) revert CreateOffererErrors.InvalidContextLength();

351: 		        if (!(minimumReceived.length == 1 && maximumSpent.length == 1)) revert CreateOffererErrors.NoBatchWrapping();

351: 		        if (!(minimumReceived.length == 1 && maximumSpent.length == 1)) revert CreateOffererErrors.NoBatchWrapping();

352: 		        if (minimumReceived[0].itemType != ItemType.ERC721 || minimumReceived[0].token != address(this) || minimumReceived[0].amount != 1) {
```
[[297](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L297), [351](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L351), [351](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L351), [352](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L352)]



```solidity
File: src/libraries/DelegateTokenLib.sol

97: 		        if (to.code.length == 0 || IERC721Receiver(to).onERC721Received(msg.sender, from, delegateTokenId, data) == IERC721Receiver.onERC721Received.selector) return;

102: 		        if (to.code.length == 0 || IERC721Receiver(to).onERC721Received(msg.sender, from, delegateTokenId, "") == IERC721Receiver.onERC721Received.selector) return;
```
[[97](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L97), [102](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L102)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

32: 		        if (underlyingAmount != 0) {

46: 		        if (underlyingTokenId != 0) {

49: 		        if (underlyingAmount == 0) {

62: 		        if (pullAmount == 0) revert Errors.WrongAmountForType(IDelegateRegistry.DelegationType.ERC1155, pullAmount);
```
[[32](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L32), [46](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L46), [49](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L49), [62](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L62)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

106: 		        if (amount != 0) {

130: 		        if (amount != 0) {

330: 		        return Ops.or(interfaceId == type(IDelegateRegistry).interfaceId, interfaceId == 0x01ffc9a7);
```
[[106](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L106), [130](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L130), [330](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L330)]

</details>

---

### [NC-22] Consider using `delete` instead of assigning zero/false to clear values

The `delete` keyword more closely matches the semantics of what is being done, and draws more attention to the changing of state, which may lead to a more thorough audit of its associated logic.

*There are 2 instances of this issue.*


```solidity
File: src/DelegateToken.sol

273: 		        if (delegateInfo.tokenType == IDelegateRegistry.DelegationType.ERC20) delegateInfo.tokenId = 0;

275: 		        if (delegateInfo.tokenType == IDelegateRegistry.DelegationType.ERC721) delegateInfo.amount = 0;
```
[[273](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L273), [275](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L275)]


---

### [NC-23] Use a ternary statement instead of `if`/`else` when appropriate

The `if`/`else` statement can be written in a shorthand way using the ternary operator, as it increases readability and reduces the number of lines of code.

*There are 2 instances of this issue.*


```solidity
File: src/DelegateToken.sol

273: 		        if (delegateInfo.tokenType == IDelegateRegistry.DelegationType.ERC20) delegateInfo.tokenId = 0;
274: 		        else delegateInfo.tokenId = RegistryHelpers.loadTokenId(delegateRegistry, registryHash);

275: 		        if (delegateInfo.tokenType == IDelegateRegistry.DelegationType.ERC721) delegateInfo.amount = 0;
276: 		        else delegateInfo.amount = StorageHelpers.readUnderlyingAmount(delegateTokenInfo, delegateTokenId);
```
[[273-274](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L273-L274), [275-276](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L275-L276)]


---

### [NC-24] Layout order does not comply with best practices

This is a [best practice](https://docs.soliditylang.org/en/latest/style-guide.html#order-of-layout) that should be followed.

Inside each contract, library or interface, use the following order:

1. Type declarations
2. State variables
3. Events
4. Errors
5. Modifiers
6. Functions

*There is 1 instance of this issue.*


```solidity
File: src/libraries/CreateOffererLib.sol

// @audit function constructor found on line 145
156: 		    modifier checkStage(CreateOffererEnums.Stage currentStage, CreateOffererEnums.Stage nextStage) {
```
[[156](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L156)]


---

### [NC-25] Function visibility order does not comply with best practices

This is a [best practice](https://docs.soliditylang.org/en/latest/style-guide.html#order-of-functions) that should be followed.

Functions should be grouped according to their visibility and ordered:

1. constructor
2. receive function (if exists)
3. fallback function (if exists)
4. external
5. public
6. internal
7. private

Within a grouping, place the view and pure functions last.

*There are 2 instances of this issue.*


```solidity
File: src/PrincipalToken.sol

// @audit _checkDelegateTokenCaller on line 27, which is internal
50: 		    function isApprovedOrOwner(address account, uint256 id) external view returns (bool) {

// @audit _checkDelegateTokenCaller on line 27, which is internal
54: 		    function tokenURI(uint256 id) public view override returns (string memory) {
```
[[50](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L50), [54](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L54)]


---

### [NC-26] Long functions should be refactored into multiple functions

Consider splitting long functions into multiple, smaller functions to improve the code readability.

*There is 1 instance of this issue.*


```solidity
File: src/CreateOfferer.sol

89: 		    function transferFrom(address from, address targetTokenReceiver, uint256 createOrderHashAsTokenId) external checkStage(Enums.Stage.transfer, Enums.Stage.ratify) {
```
[[89](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L89)]


---

### [NC-27] Lines are too long

Maximum suggested line length is 120 characters according to the [documentation](https://docs.soliditylang.org/en/latest/style-guide.html#maximum-line-length).

*There are 197 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/CreateOfferer.sol

11: 		import {ContractOffererInterface, SpentItem, ReceivedItem, Schema} from "seaport/contracts/interfaces/ContractOffererInterface.sol";

35: 		            Structs.Order({rights: 0, expiryLength: 1, signerSalt: 1, tokenContract: address(42), expiryType: Enums.ExpiryType.absolute, targetToken: Enums.TargetToken.principal});

52: 		    function generateOrder(address fulfiller, SpentItem[] calldata minimumReceived, SpentItem[] calldata maximumSpent, bytes calldata context)

71: 		    function ratifyOrder(SpentItem[] calldata offer, ReceivedItem[] calldata consideration, bytes calldata context, bytes32[] calldata, uint256 contractNonce)

86: 		     * @param createOrderHashAsTokenId The hash that secures the intended targetToken receiver being the beneficiary of a specific delegate / principal token

89: 		    function transferFrom(address from, address targetTokenReceiver, uint256 createOrderHashAsTokenId) external checkStage(Enums.Stage.transfer, Enums.Stage.ratify) {

95: 		            if (!(erc721Order.info.targetToken == Enums.TargetToken.delegate || erc721Order.info.targetToken == Enums.TargetToken.principal)) {

104: 		                    principalHolder: erc721Order.info.targetToken == Enums.TargetToken.principal ? targetTokenReceiver : transientState.receivers.fulfiller,

106: 		                    delegateHolder: erc721Order.info.targetToken == Enums.TargetToken.delegate ? targetTokenReceiver : transientState.receivers.fulfiller,

117: 		            if (!(erc20Order.info.targetToken == Enums.TargetToken.delegate || erc20Order.info.targetToken == Enums.TargetToken.principal)) {

128: 		                    principalHolder: erc20Order.info.targetToken == Enums.TargetToken.principal ? targetTokenReceiver : transientState.receivers.fulfiller,

130: 		                    delegateHolder: erc20Order.info.targetToken == Enums.TargetToken.delegate ? targetTokenReceiver : transientState.receivers.fulfiller,

143: 		            if (!(erc1155Order.info.targetToken == Enums.TargetToken.delegate || erc1155Order.info.targetToken == Enums.TargetToken.principal)) {

152: 		                    principalHolder: erc1155Order.info.targetToken == Enums.TargetToken.principal ? targetTokenReceiver : transientState.receivers.fulfiller,

154: 		                    delegateHolder: erc1155Order.info.targetToken == Enums.TargetToken.delegate ? targetTokenReceiver : transientState.receivers.fulfiller,

176: 		    function previewOrder(address caller, address, SpentItem[] calldata minimumReceived, SpentItem[] calldata maximumSpent, bytes calldata context)

195: 		    function calculateERC721OrderHashAndId(address targetTokenReceiver, address conduit, Structs.ERC721Order calldata erc721Order)

201: 		            Helpers.calculateOrderHashAndId(delegateToken, targetTokenReceiver, conduit, abi.encode(erc721Order), IDelegateRegistry.DelegationType.ERC721);

213: 		    function calculateERC20OrderHashAndId(address targetTokenReceiver, address conduit, Structs.ERC20Order calldata erc20Order)

219: 		            Helpers.calculateOrderHashAndId(delegateToken, targetTokenReceiver, conduit, abi.encode(erc20Order), IDelegateRegistry.DelegationType.ERC20);

231: 		    function calculateERC1155OrderHashAndId(address targetTokenReceiver, address conduit, Structs.ERC1155Order calldata erc1155Order)

237: 		            Helpers.calculateOrderHashAndId(delegateToken, targetTokenReceiver, conduit, abi.encode(erc1155Order), IDelegateRegistry.DelegationType.ERC1155);
```
[[11](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L11), [35](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L35), [52](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L52), [71](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L71), [86](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L86), [89](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L89), [95](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L95), [104](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L104), [106](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L106), [117](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L117), [128](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L128), [130](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L130), [143](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L143), [152](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L152), [154](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L154), [176](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L176), [195](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L195), [201](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L201), [213](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L213), [219](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L219), [231](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L231), [237](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L237)]



```solidity
File: src/DelegateToken.sol

10: 		import {IDelegateRegistry, DelegateTokenErrors as Errors, DelegateTokenStructs as Structs, DelegateTokenHelpers as Helpers} from "src/libraries/DelegateTokenLib.sol";

12: 		import {DelegateTokenRegistryHelpers as RegistryHelpers, RegistryHashes} from "src/libraries/DelegateTokenRegistryHelpers.sol";

13: 		import {DelegateTokenTransferHelpers as TransferHelpers, SafeERC20, IERC721, IERC20, IERC1155} from "src/libraries/DelegateTokenTransferHelpers.sol";

78: 		    function onERC1155BatchReceived(address, address, uint256[] calldata, uint256[] calldata, bytes calldata) external pure returns (bytes4) {

106: 		        delegateTokenHolder = RegistryHelpers.loadTokenHolder(delegateRegistry, StorageHelpers.readRegistryHash(delegateTokenInfo, delegateTokenId));

165: 		        (address delegateTokenHolder, address underlyingContract) = RegistryHelpers.loadTokenHolderAndContract(delegateRegistry, registryHash);

178: 		            newRegistryHash = RegistryHashes.erc721Hash(address(this), underlyingRights, to, underlyingTokenId, underlyingContract);

180: 		            RegistryHelpers.transferERC721(delegateRegistry, registryHash, from, newRegistryHash, to, underlyingRights, underlyingContract, underlyingTokenId);

196: 		            newRegistryHash = RegistryHashes.erc1155Hash(address(this), underlyingRights, to, underlyingTokenId, underlyingContract);

243: 		        return spender == delegateTokenHolder || accountOperator[delegateTokenHolder][spender] || StorageHelpers.readApproved(delegateTokenInfo, delegateTokenId) == spender;

256: 		    function royaltyInfo(uint256 tokenId, uint256 salePrice) external view returns (address receiver, uint256 royaltyAmount) {

269: 		        (delegateInfo.delegateHolder, delegateInfo.tokenContract) = RegistryHelpers.loadTokenHolderAndContract(delegateRegistry, registryHash);

296: 		    function create(Structs.DelegateInfo calldata delegateInfo, uint256 salt) external nonReentrant returns (uint256 delegateTokenId) {

307: 		            newRegistryHash = RegistryHashes.erc721Hash(address(this), delegateInfo.rights, delegateInfo.delegateHolder, delegateInfo.tokenId, delegateInfo.tokenContract);

312: 		            newRegistryHash = RegistryHashes.erc20Hash(address(this), delegateInfo.rights, delegateInfo.delegateHolder, delegateInfo.tokenContract);

317: 		            newRegistryHash = RegistryHashes.erc1155Hash(address(this), delegateInfo.rights, delegateInfo.delegateHolder, delegateInfo.tokenId, delegateInfo.tokenContract);

321: 		        StorageHelpers.mintPrincipal(principalToken, principalMintAuthorization, delegateInfo.principalHolder, delegateTokenId);

358: 		        (address delegateTokenHolder, address underlyingContract) = RegistryHelpers.loadTokenHolderAndContract(delegateRegistry, registryHash);

359: 		        StorageHelpers.revertInvalidWithdrawalConditions(delegateTokenInfo, accountOperator, delegateTokenId, delegateTokenHolder);

367: 		            RegistryHelpers.revokeERC721(delegateRegistry, registryHash, delegateTokenHolder, underlyingContract, erc721UnderlyingTokenId, underlyingRights);

373: 		            RegistryHelpers.decrementERC20(delegateRegistry, registryHash, delegateTokenHolder, underlyingContract, erc20UnderlyingAmount, underlyingRights);

381: 		                delegateRegistry, registryHash, delegateTokenHolder, underlyingContract, erc11551UnderlyingTokenId, erc1155UnderlyingAmount, underlyingRights

384: 		            IERC1155(underlyingContract).safeTransferFrom(address(this), msg.sender, erc11551UnderlyingTokenId, erc1155UnderlyingAmount, "");
```
[[10](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L10), [12](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L12), [13](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L13), [78](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L78), [106](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L106), [165](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L165), [178](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L178), [180](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L180), [196](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L196), [243](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L243), [256](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L256), [269](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L269), [296](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L296), [307](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L307), [312](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L312), [317](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L317), [321](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L321), [358](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L358), [359](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L359), [367](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L367), [373](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L373), [381](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L381), [384](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L384)]



```solidity
File: src/libraries/CreateOffererLib.sol

257: 		    function createAndValidateDelegateTokenId(address delegateToken, uint256 createOrderHash, IDelegateTokenStructs.DelegateInfo memory delegateInfo) internal {

269: 		     * @param conduit The address of the conduit that should conduct the create on transferFrom on seaport calling CreateOfferer

274: 		    function calculateOrderHashAndId(address delegateToken, address targetTokenReceiver, address conduit, bytes memory orderInfo, IDelegateRegistry.DelegationType delegationType)

280: 		        delegateTokenId = IDelegateToken(delegateToken).getDelegateId(address(this), createOrderHash); // This should revert if already existed

284: 		     * @notice Verifies the properties of a delegateToken against the first element of a seaport ContractOfferer ratify order calldata

287: 		     * @param consideration The consideration specified in the ratify order call data (used as input data of the underlying used to create the delegate token)

288: 		     * @param context Should contain an unpacked encoding of the Context struct which provides additional order data for comparison

292: 		    function verifyCreate(address delegateToken, uint256 identifier, CreateOffererStructs.Receivers storage receivers, ReceivedItem calldata consideration, bytes calldata context)

305: 		                        principalHolder: decodedContext.targetToken == CreateOffererEnums.TargetToken.principal ? receivers.targetTokenReceiver : receivers.fulfiller,

306: 		                        delegateHolder: decodedContext.targetToken == CreateOffererEnums.TargetToken.delegate ? receivers.targetTokenReceiver : receivers.fulfiller,

314: 		            ) != keccak256(abi.encode(IDelegateToken(delegateToken).getDelegateInfo(DelegateTokenHelpers.delegateIdNoRevert(address(this), identifier))))

326: 		    function calculateExpiry(CreateOffererEnums.ExpiryType expiryType, uint256 expiryLength) internal view returns (uint256) {

352: 		        if (minimumReceived[0].itemType != ItemType.ERC721 || minimumReceived[0].token != address(this) || minimumReceived[0].amount != 1) {

355: 		        if (maximumSpent[0].itemType != ItemType.ERC721 && maximumSpent[0].itemType != ItemType.ERC20 && maximumSpent[0].itemType != ItemType.ERC1155) {

359: 		        offer[0] = SpentItem({itemType: minimumReceived[0].itemType, token: minimumReceived[0].token, identifier: minimumReceived[0].identifier, amount: minimumReceived[0].amount});

378: 		    function validateCreateOrderHash(address targetTokenReceiver, uint256 createOrderHash, bytes memory encodedOrder, IDelegateRegistry.DelegationType tokenType) internal view {

379: 		        uint256 actualCreateOrderHash = CreateOffererHelpers.calculateOrderHash(targetTokenReceiver, msg.sender, encodedOrder, tokenType);

393: 		    function calculateOrderHash(address targetTokenReceiver, address conduit, bytes memory createOrderInfo, IDelegateRegistry.DelegationType tokenType)
```
[[257](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L257), [269](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L269), [274](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L274), [280](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L280), [284](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L284), [287](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L287), [288](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L288), [292](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L292), [305](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L305), [306](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L306), [314](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L314), [326](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L326), [352](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L352), [355](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L355), [359](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L359), [378](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L378), [379](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L379), [393](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L393)]



```solidity
File: src/libraries/DelegateTokenLib.sol

92: 		        if (IDelegateFlashloan(info.receiver).onFlashloan{value: msg.value}(msg.sender, info) == IDelegateFlashloan.onFlashloan.selector) return;

96: 		    function revertOnInvalidERC721ReceiverCallback(address from, address to, uint256 delegateTokenId, bytes calldata data) internal {

97: 		        if (to.code.length == 0 || IERC721Receiver(to).onERC721Received(msg.sender, from, delegateTokenId, data) == IERC721Receiver.onERC721Received.selector) return;

102: 		        if (to.code.length == 0 || IERC721Receiver(to).onERC721Received(msg.sender, from, delegateTokenId, "") == IERC721Receiver.onERC721Received.selector) return;
```
[[92](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L92), [96](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L96), [97](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L97), [102](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L102)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

6: 		import {IDelegateRegistry, DelegateTokenErrors as Errors, DelegateTokenStructs as Structs} from "src/libraries/DelegateTokenLib.sol";

16: 		    function loadTokenHolder(address delegateRegistry, bytes32 registryHash) internal view returns (address delegateTokenHolder) {

19: 		                IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_SECOND_PACKED))

29: 		     * @dev Two slots need to be loaded in the registry given the packed configuration, this function should only be used when you don't need "to" or "from"

32: 		    function loadContract(address delegateRegistry, bytes32 registryHash) internal view returns (address underlyingContract) {

52: 		    function loadTokenHolderAndContract(address delegateRegistry, bytes32 registryHash) internal view returns (address delegateTokenHolder, address underlyingContract) {

72: 		                IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_FIRST_PACKED))

84: 		            return uint256(IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_AMOUNT)));

96: 		            return IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_RIGHTS));

108: 		            return uint256(IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_TOKEN_ID)));

119: 		    function calculateDecreasedAmount(address delegateRegistry, bytes32 registryHash, uint256 decreaseAmount) internal view returns (uint256) {

122: 		                uint256(IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_AMOUNT))) - decreaseAmount;

133: 		    function calculateIncreasedAmount(address delegateRegistry, bytes32 registryHash, uint256 increaseAmount) internal view returns (uint256) {

136: 		                uint256(IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_AMOUNT))) + increaseAmount;

146: 		            loadFrom(delegateRegistry, RegistryHashes.erc721Hash(address(this), "", info.delegateHolder, info.tokenId, info.tokenContract)) == address(this)

147: 		                || loadFrom(delegateRegistry, RegistryHashes.erc721Hash(address(this), "flashloan", info.delegateHolder, info.tokenId, info.tokenContract)) == address(this)

155: 		            // We sum the delegation amounts for "flashloan" and "" rights since liquid delegate doesn't allow double spends for different rights

156: 		            availableAmount = loadAmount(delegateRegistry, RegistryHashes.erc20Hash(address(this), "flashloan", info.delegateHolder, info.tokenContract))

165: 		            availableAmount = loadAmount(delegateRegistry, RegistryHashes.erc1155Hash(address(this), "flashloan", info.delegateHolder, info.tokenId, info.tokenContract))

166: 		                + loadAmount(delegateRegistry, RegistryHashes.erc1155Hash(address(this), "", info.delegateHolder, info.tokenId, info.tokenContract));

185: 		            IDelegateRegistry(delegateRegistry).delegateERC721(from, underlyingContract, underlyingTokenId, underlyingRights, false) == registryHash

186: 		                && IDelegateRegistry(delegateRegistry).delegateERC721(to, underlyingContract, underlyingTokenId, underlyingRights, true) == newRegistryHash

230: 		        if (IDelegateRegistry(delegateRegistry).delegateERC1155(from, underlyingContract, underlyingTokenId, underlyingRights, amount) != registryHash) {

234: 		        if (IDelegateRegistry(delegateRegistry).delegateERC1155(to, underlyingContract, underlyingTokenId, underlyingRights, amount) != newRegistryHash) {

240: 		    function delegateERC721(address delegateRegistry, bytes32 newRegistryHash, Structs.DelegateInfo calldata delegateInfo) internal {

242: 		            IDelegateRegistry(delegateRegistry).delegateERC721(delegateInfo.delegateHolder, delegateInfo.tokenContract, delegateInfo.tokenId, delegateInfo.rights, true)

250: 		    function incrementERC20(address delegateRegistry, bytes32 newRegistryHash, Structs.DelegateInfo calldata delegateInfo) internal {

253: 		                delegateInfo.delegateHolder, delegateInfo.tokenContract, delegateInfo.rights, calculateIncreasedAmount(delegateRegistry, newRegistryHash, delegateInfo.amount)

261: 		    function incrementERC1155(address delegateRegistry, bytes32 newRegistryHash, Structs.DelegateInfo calldata delegateInfo) internal {

283: 		        if (IDelegateRegistry(delegateRegistry).delegateERC721(delegateTokenHolder, underlyingContract, underlyingTokenId, underlyingRights, false) == registryHash) {

301: 		                delegateTokenHolder, underlyingContract, underlyingRights, calculateDecreasedAmount(delegateRegistry, registryHash, underlyingAmount)

320: 		                delegateTokenHolder, underlyingContract, underlyingTokenId, underlyingRights, calculateDecreasedAmount(delegateRegistry, registryHash, underlyingAmount)
```
[[6](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L6), [16](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L16), [19](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L19), [29](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L29), [32](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L32), [52](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L52), [72](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L72), [84](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L84), [96](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L96), [108](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L108), [119](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L119), [122](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L122), [133](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L133), [136](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L136), [146](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L146), [147](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L147), [155](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L155), [156](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L156), [165](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L165), [166](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L166), [185](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L185), [186](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L186), [230](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L230), [234](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L234), [240](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L240), [242](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L242), [250](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L250), [253](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L253), [261](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L261), [283](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L283), [301](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L301), [320](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L320)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

36: 		    /// @dev should preserve the expiry in the lower 96 bits in storage, and update the upper 160 bits with approved address

37: 		    function writeApproved(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId, address approved) internal {

44: 		    function writeExpiry(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId, uint256 expiry) internal {

50: 		    function writeRegistryHash(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId, bytes32 registryHash) internal {

54: 		    function writeUnderlyingAmount(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId, uint256 underlyingAmount) internal {

58: 		    function incrementBalance(mapping(address delegateTokenHolder => uint256 balance) storage balances, address delegateTokenHolder) internal {

64: 		    function decrementBalance(mapping(address delegateTokenHolder => uint256 balance) storage balances, address delegateTokenHolder) internal {

72: 		    function burnPrincipal(address principalToken, Structs.Uint256 storage principalBurnAuthorization, uint256 delegateTokenId) internal {

84: 		    function mintPrincipal(address principalToken, Structs.Uint256 storage principalMintAuthorization, address principalRecipient, uint256 delegateTokenId) internal {

96: 		    function checkBurnAuthorized(address principalToken, Structs.Uint256 storage principalBurnAuthorization) internal view {

104: 		    function checkMintAuthorized(address principalToken, Structs.Uint256 storage principalMintAuthorization) internal view {

117: 		    function revertAlreadyExisted(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId) internal view {

122: 		    function revertNotOperator(mapping(address account => mapping(address operator => bool enabled)) storage accountOperator, address account) internal view {

127: 		    function readApproved(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId) internal view returns (address) {

131: 		    function readExpiry(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId) internal view returns (uint256) {

135: 		    function readRegistryHash(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId) internal view returns (bytes32) {

139: 		    function readUnderlyingAmount(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId) internal view returns (uint256) {

149: 		        if (msg.sender == account || accountOperator[account][msg.sender] || msg.sender == readApproved(delegateTokenInfo, delegateTokenId)) return;

153: 		    /// @dev should only revert if expiry has not expired AND caller is not the delegateTokenHolder AND not approved for the delegateTokenId AND not an operator for

163: 		            if (delegateTokenHolder == msg.sender || msg.sender == readApproved(delegateTokenInfo, delegateTokenId) || accountOperator[delegateTokenHolder][msg.sender]) {

170: 		    function revertNotMinted(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId) internal view {

177: 		    /// @dev does not read from storage, make sure the registryHash of the corresponding delegateTokenId is passed to have the intended effect
```
[[36](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L36), [37](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L37), [44](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L44), [50](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L50), [54](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L54), [58](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L58), [64](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L64), [72](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L72), [84](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L84), [96](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L96), [104](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L104), [117](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L117), [122](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L122), [127](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L127), [131](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L131), [135](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L135), [139](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L139), [149](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L149), [153](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L153), [163](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L163), [170](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L170), [177](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L177)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

4: 		import {IDelegateRegistry, DelegateTokenErrors as Errors, DelegateTokenStructs as Structs} from "src/libraries/DelegateTokenLib.sol";

15: 		    function checkAndPullByType(Structs.Uint256 storage erc1155Pulled, Structs.DelegateInfo calldata delegateInfo) internal {

31: 		    function checkERC721BeforePull(uint256 underlyingAmount, address underlyingContract, uint256 underlyingTokenId) internal view {

45: 		    function checkERC20BeforePull(uint256 underlyingAmount, address underlyingContract, uint256 underlyingTokenId) internal view {

70: 		    function pullERC1155AfterCheck(Structs.Uint256 storage erc1155Pulled, uint256 pullAmount, address underlyingContract, uint256 underlyingTokenId) internal {
```
[[4](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L4), [15](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L15), [31](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L31), [45](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L45), [70](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L70)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

63: 		    function delegateContract(address to, address contract_, bytes32 rights, bool enable) external payable override returns (bytes32 hash) {

82: 		    function delegateERC721(address to, address contract_, uint256 tokenId, bytes32 rights, bool enable) external payable override returns (bytes32 hash) {

102: 		    function delegateERC20(address to, address contract_, bytes32 rights, uint256 amount) external payable override returns (bytes32 hash) {

126: 		    function delegateERC1155(address to, address contract_, uint256 tokenId, bytes32 rights, uint256 amount) external payable override returns (bytes32 hash) {

153: 		        // This hardcoded address is a CREATE2 factory counterfactual smart contract wallet that will always accept native token transfers

178: 		    function checkDelegateForContract(address to, address from, address contract_, bytes32 rights) external view override returns (bool valid) {

180: 		            valid = _validateFrom(Hashes.allLocation(from, "", to), from) || _validateFrom(Hashes.contractLocation(from, "", to, contract_), from);

182: 		                valid = _validateFrom(Hashes.allLocation(from, rights, to), from) || _validateFrom(Hashes.contractLocation(from, rights, to, contract_), from);

193: 		    function checkDelegateForERC721(address to, address from, address contract_, uint256 tokenId, bytes32 rights) external view override returns (bool valid) {

195: 		            valid = _validateFrom(Hashes.allLocation(from, "", to), from) || _validateFrom(Hashes.contractLocation(from, "", to, contract_), from)

198: 		                valid = _validateFrom(Hashes.allLocation(from, rights, to), from) || _validateFrom(Hashes.contractLocation(from, rights, to, contract_), from)

210: 		    function checkDelegateForERC20(address to, address from, address contract_, bytes32 rights) external view override returns (uint256 amount) {

212: 		            amount = (_validateFrom(Hashes.allLocation(from, "", to), from) || _validateFrom(Hashes.contractLocation(from, "", to, contract_), from))

216: 		                uint256 rightsBalance = (_validateFrom(Hashes.allLocation(from, rights, to), from) || _validateFrom(Hashes.contractLocation(from, rights, to, contract_), from))

229: 		    function checkDelegateForERC1155(address to, address from, address contract_, uint256 tokenId, bytes32 rights) external view override returns (uint256 amount) {

231: 		            amount = (_validateFrom(Hashes.allLocation(from, "", to), from) || _validateFrom(Hashes.contractLocation(from, "", to, contract_), from))

235: 		                uint256 rightsBalance = (_validateFrom(Hashes.allLocation(from, rights, to), from) || _validateFrom(Hashes.contractLocation(from, rights, to, contract_), from))

279: 		                    delegations_[i] = Delegation({type_: DelegationType.NONE, to: address(0), from: address(0), rights: "", amount: 0, contract_: address(0), tokenId: 0});

379: 		    /// @dev Helper function that takes an array of delegation hashes and returns an array of Delegation structs with their onchain information

380: 		    function _getValidDelegationsFromHashes(bytes32[] storage hashes) internal view returns (Delegation[] memory delegations_) {

411: 		    function _getValidDelegationHashesFromHashes(bytes32[] storage hashes) internal view returns (bytes32[] memory validHashes) {

459: 		    function _loadDelegationAddresses(bytes32 location) internal view returns (address from, address to, address contract_) {
```
[[63](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L63), [82](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L82), [102](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L102), [126](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L126), [153](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L153), [178](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L178), [180](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L180), [182](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L182), [193](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L193), [195](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L195), [198](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L198), [210](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L210), [212](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L212), [216](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L216), [229](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L229), [231](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L231), [235](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L235), [279](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L279), [379](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L379), [380](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L380), [411](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L411), [459](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L459)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryHashes.sol

17: 		 * To avoid collisions between the hashes with respect to type, the hash is shifted left by one byte and the last byte is then encoded with a unique number for the

24: 		    /// @dev uint256 constant for the delegate registry delegation type enumeration, related unit test should fail if these mismatch

38: 		     * @dev may lead to a revert with Conversion into non-existent enum type after the function is called if inputHash was encoded with type outside the DelegationType

52: 		     * @dev Follows the solidity storage location encoding for a mapping(bytes32 => fixedArray) at the position of the delegationSlot

69: 		     * @dev returned hash should be equivalent to keccak256(abi.encodePacked(rights, from, to)) followed by a shift left by 1 byte and writing the delegation type to the

71: 		     * @dev will not revert if from or to are > uint160, any input larger than uint160 for from and to will be cleaned to their last 20 bytes

81: 		            hash := or(shl(8, keccak256(ptr, 72)), ALL_TYPE) // Runs keccak over the packed encoding, shifts left by one byte, then writes the type to the last

91: 		     * @return computedLocation is the storage location of the all delegation with those parameters in the delegations mapping

93: 		     * @dev will not revert if from or to are > uint160, any input larger than uint160 for from and to will be cleaned to their last 20 bytes

103: 		            mstore(0, or(shl(8, keccak256(ptr, 72)), ALL_TYPE)) // Runs keccak over the packed encoding, shifts left by one byte, then writes the type to the

117: 		     * @dev returned hash should be equivalent to keccak256(abi.encodePacked(rights, from, to, contract_)) with the last byte overwritten with CONTRACT_TYPE

118: 		     * @dev will not revert if from, to, or contract_ are > uint160, any input larger than uint160 for from, to, or contract_ will be cleaned to their last 20 bytes

120: 		    function contractHash(address from, bytes32 rights, address to, address contract_) internal pure returns (bytes32 hash) {

129: 		            hash := or(shl(8, keccak256(ptr, 92)), CONTRACT_TYPE) // Runs keccak over the packed encoding, shifts left by one byte, then writes the type to the last byte

139: 		     * @return computedLocation is the storage location of the contract delegation with those parameters in the delegations mapping

141: 		     * @dev will not revert if from, to, or contract_ are > uint160, any input larger than uint160 for from, to, or contract_ will be cleaned to their last 20 bytes

143: 		    function contractLocation(address from, bytes32 rights, address to, address contract_) internal pure returns (bytes32 computedLocation) {

152: 		            mstore(0, or(shl(8, keccak256(ptr, 92)), CONTRACT_TYPE)) // Runs keccak over the packed encoding, shifts left by one byte, then writes the type to the

167: 		     * @dev returned hash should be equivalent to keccak256(abi.encodePacked(rights, from, to, contract_, tokenId)) with the last byte overwritten with ERC721_TYPE

168: 		     * @dev will not revert if from, to, or contract_ are > uint160, any input larger than uint160 for from, to, or contract_ will be cleaned to their last 20 bytes

170: 		    function erc721Hash(address from, bytes32 rights, address to, uint256 tokenId, address contract_) internal pure returns (bytes32 hash) {

180: 		            hash := or(shl(8, keccak256(ptr, 124)), ERC721_TYPE) // Runs keccak over the packed encoding, shifts left by one byte, then writes the type to the last byte

191: 		     * @return computedLocation is the storage location of the erc721 delegation with those parameters in the delegations mapping

193: 		     * @dev will not revert if from, to, or contract_ are > uint160, any input larger than uint160 for from, to, or contract_ will be cleaned to their last 20 bytes

195: 		    function erc721Location(address from, bytes32 rights, address to, uint256 tokenId, address contract_) internal pure returns (bytes32 computedLocation) {

205: 		            mstore(0, or(shl(8, keccak256(ptr, 124)), ERC721_TYPE)) // Runs keccak over the packed encoding, shifts left by one byte, then writes the type to the

219: 		     * @dev returned hash should be equivalent to keccak256(abi.encodePacked(rights, from, to, contract_)) with the last byte overwritten with ERC20_TYPE

220: 		     * @dev will not revert if from, to, or contract_ are > uint160, any input larger than uint160 for from, to, or contract_ will be cleaned to their last 20 bytes

231: 		            hash := or(shl(8, keccak256(ptr, 92)), ERC20_TYPE) // Runs keccak over the packed encoding, shifts left by one byte, then writes the type to the last byte

241: 		     * @return computedLocation is the storage location of the erc20 delegation with those parameters in the delegations mapping

243: 		     * @dev will not revert if from, to, or contract_ are > uint160, any input larger than uint160 for from, to, or contract_ will be cleaned to their last 20 bytes

245: 		    function erc20Location(address from, bytes32 rights, address to, address contract_) internal pure returns (bytes32 computedLocation) {

254: 		            mstore(0, or(shl(8, keccak256(ptr, 92)), ERC20_TYPE)) // Runs keccak over the packed encoding, shifts left by one byte, then writes the type to the

269: 		     * @dev returned hash should be equivalent to keccak256(abi.encodePacked(rights, from, to, contract_, tokenId)) with the last byte overwritten with ERC1155_TYPE

270: 		     * @dev will not revert if from, to, or contract_ are > uint160, any input larger than uint160 for from, to, or contract_ will be cleaned to their last 20 bytes

272: 		    function erc1155Hash(address from, bytes32 rights, address to, uint256 tokenId, address contract_) internal pure returns (bytes32 hash) {

282: 		            hash := or(shl(8, keccak256(ptr, 124)), ERC1155_TYPE) // Runs keccak over the packed encoding, shifts left by one byte, then writes the type to the last byte

293: 		     * @return computedLocation is the storage location of the erc1155 delegation with those parameters in the delegations mapping

295: 		     * @dev will not revert if from, to, or contract_ are > uint160, any input larger than uint160 for from, to, or contract_ will be cleaned to their last 20 bytes

297: 		    function erc1155Location(address from, bytes32 rights, address to, uint256 tokenId, address contract_) internal pure returns (bytes32 computedLocation) {

307: 		            mstore(0, or(shl(8, keccak256(ptr, 124)), ERC1155_TYPE)) // Runs keccak over the packed encoding, shifts left by one byte, then writes the type to the
```
[[17](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L17), [24](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L24), [38](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L38), [52](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L52), [69](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L69), [71](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L71), [81](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L81), [91](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L91), [93](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L93), [103](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L103), [117](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L117), [118](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L118), [120](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L120), [129](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L129), [139](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L139), [141](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L141), [143](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L143), [152](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L152), [167](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L167), [168](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L168), [170](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L170), [180](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L180), [191](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L191), [193](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L193), [195](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L195), [205](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L205), [219](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L219), [220](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L220), [231](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L231), [241](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L241), [243](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L243), [245](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L245), [254](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L254), [269](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L269), [270](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L270), [272](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L272), [282](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L282), [293](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L293), [295](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L295), [297](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L297), [307](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L307)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryStorage.sol

5: 		    /// @dev Standardizes from storage flags to prevent double-writes in the delegation in/outbox if the same delegation is revoked and rewritten

10: 		    uint256 internal constant POSITIONS_FIRST_PACKED = 0; //  | 4 bytes empty | first 8 bytes of contract address | 20 bytes of from address |

11: 		    uint256 internal constant POSITIONS_SECOND_PACKED = 1; // |        last 12 bytes of contract address          | 20 bytes of to address   |

32: 		     * @dev Will not revert if from, to, and contract_ are > uint160, any inputs with dirty bits outside the last 20 bytes will be cleaned

34: 		    function packAddresses(address from, address to, address contract_) internal pure returns (bytes32 firstPacked, bytes32 secondPacked) {

42: 		     * @notice Helper function that unpacks from, to, and contract_ address inside the firstPacked secondPacked storage configuration

48: 		     * @dev Will not revert if from, to, and contract_ are > uint160, any inputs with dirty bits outside the last 20 bytes will be cleaned

50: 		    function unpackAddresses(bytes32 firstPacked, bytes32 secondPacked) internal pure returns (address from, address to, address contract_) {
```
[[5](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L5), [10](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L10), [11](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L11), [32](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L32), [34](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L34), [42](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L42), [48](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L48), [50](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L50)]

</details>

---

### [NC-28] Missing variable names

Consider adding a comment with the variable name even if it's not used, to improve the code readability.

*There are 14 instances of this issue.*


```solidity
File: src/CreateOfferer.sol

71: 		    function ratifyOrder(SpentItem[] calldata offer, ReceivedItem[] calldata consideration, bytes calldata context, bytes32[] calldata, uint256 contractNonce)

176: 		    function previewOrder(address caller, address, SpentItem[] calldata minimumReceived, SpentItem[] calldata maximumSpent, bytes calldata context)
```
[[71](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L71), [176](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L176)]



```solidity
File: src/DelegateToken.sol

78: 		    function onERC1155BatchReceived(address, address, uint256[] calldata, uint256[] calldata, bytes calldata) external pure returns (bytes4) {

78: 		    function onERC1155BatchReceived(address, address, uint256[] calldata, uint256[] calldata, bytes calldata) external pure returns (bytes4) {

78: 		    function onERC1155BatchReceived(address, address, uint256[] calldata, uint256[] calldata, bytes calldata) external pure returns (bytes4) {

78: 		    function onERC1155BatchReceived(address, address, uint256[] calldata, uint256[] calldata, bytes calldata) external pure returns (bytes4) {

78: 		    function onERC1155BatchReceived(address, address, uint256[] calldata, uint256[] calldata, bytes calldata) external pure returns (bytes4) {

83: 		    function onERC721Received(address operator, address, uint256, bytes calldata) external view returns (bytes4) {

83: 		    function onERC721Received(address operator, address, uint256, bytes calldata) external view returns (bytes4) {

83: 		    function onERC721Received(address operator, address, uint256, bytes calldata) external view returns (bytes4) {

89: 		    function onERC1155Received(address operator, address, uint256, uint256, bytes calldata) external returns (bytes4) {

89: 		    function onERC1155Received(address operator, address, uint256, uint256, bytes calldata) external returns (bytes4) {

89: 		    function onERC1155Received(address operator, address, uint256, uint256, bytes calldata) external returns (bytes4) {

89: 		    function onERC1155Received(address operator, address, uint256, uint256, bytes calldata) external returns (bytes4) {
```
[[78](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L78), [78](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L78), [78](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L78), [78](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L78), [78](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L78), [83](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L83), [83](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L83), [83](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L83), [89](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L89), [89](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L89), [89](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L89), [89](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L89)]


---

### [NC-29] Typos in comments

Avoid typos, and proper nouns should be capitalized.

*There are 2 instances of this issue.*


```solidity
File: src/libraries/CreateOffererLib.sol

// @audit ths
154: 		     * @param nextStage The stage to be entered after ths stage being marked by the modifier
```
[[154](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L154)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

// @audit mireynolds
13: 		 * @custom:coauthor mireynolds
```
[[13](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L13)]


---

### [NC-30] Contracts should have full test coverage

A 100% test coverage is not foolproof, but it helps immensely in reducing the amount of bugs that may occur.



---

### [NC-31] Large or complicated code bases should implement invariant tests

This includes: large code bases, or code with lots of inline-assembly, complicated math, or complicated interactions between multiple contracts.

Invariant fuzzers such as Echidna require the test writer to come up with invariants which should not be violated under any circumstances, and the fuzzer tests various inputs and function calls to ensure that the invariants always hold.

Even code with 100% code coverage can still have bugs due to the order of the operations a user performs, and invariant fuzzers may help significantly.



---

### [NC-32] Codebase should implement formal verification testing

Formal verification is the act of proving or disproving the correctness of intended algorithms underlying a system with respect to a certain formal specification/property/invariant, using formal methods of mathematics.

Some tools that are currently available to perform these tests on smart contracts are [SMTChecker](https://docs.soliditylang.org/en/latest/smtchecker.html) and [Certora Prover](https://www.certora.com/).



---

### [NC-33] Inconsistent spacing in comments

Some lines use `// x` and some use `//x`. The instances below point out the usages that don't follow the majority, within each file.

*There are 9 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/CreateOfferer.sol

88: 		    //slither-disable-next-line erc20-interface
```
[[88](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L88)]



```solidity
File: src/DelegateToken.sol

340: 		        //slither-disable-next-line timestamp
```
[[340](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L340)]



```solidity
File: src/libraries/CreateOffererLib.sol

299: 		        //slither-disable-start timestamp

316: 		        //slither-disable-end timestamp
```
[[299](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L299), [316](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L316)]



```solidity
File: src/libraries/DelegateTokenLib.sol

108: 		        //slither-disable-next-line timestamp
```
[[108](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L108)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

35: 		            //slither-disable-next-line unused-return

55: 		            //slither-disable-next-line unused-return
```
[[35](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L35), [55](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L55)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

161: 		        //slither-disable-next-line timestamp
```
[[161](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L161)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

36: 		                //slither-disable-next-line calls-loop,delegatecall-loop
```
[[36](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L36)]


</details>

---

### [NC-34] State variables should include comments

Consider adding some comments on critical state variables to explain what they are supposed to do: this will help for future code reviews.

*There are 19 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/CreateOfferer.sol

24: 		    address public immutable delegateToken;

25: 		    address public immutable principalToken;

26: 		    Structs.TransientState internal transientState;

27: 		    Structs.Nonce internal nonce;
```
[[24](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L24), [25](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L25), [26](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L26), [27](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L27)]



```solidity
File: src/DelegateToken.sol

26: 		    address public immutable marketMetadata;

43: 		    Structs.Uint256 internal principalBurnAuthorization = Structs.Uint256(StorageHelpers.BURN_NOT_AUTHORIZED);
```
[[26](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L26), [43](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L43)]



```solidity
File: src/PrincipalToken.sol

12: 		    address public immutable delegateToken;

13: 		    address public immutable marketMetadata;
```
[[12](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L12), [13](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L13)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

16: 		    uint256 internal constant ID_USED = 1;

32: 		    uint256 internal constant MINT_AUTHORIZED = 2;

33: 		    uint256 internal constant BURN_NOT_AUTHORIZED = 3;

34: 		    uint256 internal constant BURN_AUTHORIZED = 4;
```
[[16](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L16), [32](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L32), [33](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L33), [34](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L34)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

13: 		    uint256 internal constant ERC1155_PULLED = 6;
```
[[13](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L13)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryHashes.sol

26: 		    uint256 internal constant CONTRACT_TYPE = 2;

27: 		    uint256 internal constant ERC721_TYPE = 3;

28: 		    uint256 internal constant ERC20_TYPE = 4;
```
[[26](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L26), [27](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L27), [28](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L28)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryStorage.sol

7: 		    address internal constant DELEGATION_REVOKED = address(1);

13: 		    uint256 internal constant POSITIONS_TOKEN_ID = 3;

14: 		    uint256 internal constant POSITIONS_AMOUNT = 4;
```
[[7](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L7), [13](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L13), [14](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L14)]

</details>

---

### [NC-35] Complex functions should have explicit comments

Large and/or complex functions should have more comments to better explain the purpose of each logic step.

*There is 1 instance of this issue.*


```solidity
File: src/CreateOfferer.sol

89: 		    function transferFrom(address from, address targetTokenReceiver, uint256 createOrderHashAsTokenId) external checkStage(Enums.Stage.transfer, Enums.Stage.ratify) {
```
[[89](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L89)]


---

### [NC-36] Assembly code should have explicit comments

Low-level languages like assembly should require extensive documentation and comments to clarify the purpose of each instruction.

*There are 28 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

170: 		        assembly ("memory-safe") {

185: 		        assembly ("memory-safe") {

202: 		        assembly ("memory-safe") {

222: 		        assembly ("memory-safe") {

241: 		        assembly ("memory-safe") {

314: 		                assembly {

362: 		        assembly {

373: 		        assembly {

431: 		        assembly {

438: 		        assembly {

447: 		        assembly {

464: 		        assembly {
```
[[170](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L170), [185](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L185), [202](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L202), [222](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L222), [241](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L241), [314](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L314), [362](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L362), [373](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L373), [431](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L431), [438](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L438), [447](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L447), [464](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L464)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryHashes.sol

42: 		        assembly {

74: 		        assembly ("memory-safe") {

96: 		        assembly ("memory-safe") {

121: 		        assembly ("memory-safe") {

144: 		        assembly ("memory-safe") {

171: 		        assembly ("memory-safe") {

196: 		        assembly ("memory-safe") {

223: 		        assembly ("memory-safe") {

246: 		        assembly ("memory-safe") {

273: 		        assembly ("memory-safe") {

298: 		        assembly ("memory-safe") {
```
[[42](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L42), [74](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L74), [96](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L96), [121](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L121), [144](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L144), [171](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L171), [196](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L196), [223](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L223), [246](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L246), [273](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L273), [298](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L298)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryOps.sol

7: 		        assembly {

20: 		        assembly {

27: 		        assembly {
```
[[7](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L7), [20](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L20), [27](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L27)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryStorage.sol

35: 		        assembly {

51: 		        assembly {
```
[[35](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L35), [51](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L51)]

</details>

---

### [NC-37] Missing underscore prefix for non-external functions

This convention is suggested for non-external functions (private or internal). [Documentation](https://docs.soliditylang.org/en/latest/style-guide.html#underscore-prefix-for-non-external-functions-and-variables)

*There are 83 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/libraries/CreateOffererLib.sol

184: 		    function processNonce(CreateOffererStructs.Nonce storage nonce, uint256 contractNonce) internal {

199: 		    function updateTransientState(

257: 		    function createAndValidateDelegateTokenId(address delegateToken, uint256 createOrderHash, IDelegateTokenStructs.DelegateInfo memory delegateInfo) internal {

274: 		    function calculateOrderHashAndId(address delegateToken, address targetTokenReceiver, address conduit, bytes memory orderInfo, IDelegateRegistry.DelegationType delegationType)

292: 		    function verifyCreate(address delegateToken, uint256 identifier, CreateOffererStructs.Receivers storage receivers, ReceivedItem calldata consideration, bytes calldata context)

326: 		    function calculateExpiry(CreateOffererEnums.ExpiryType expiryType, uint256 expiryLength) internal view returns (uint256) {

346: 		    function processSpentItems(SpentItem[] calldata minimumReceived, SpentItem[] calldata maximumSpent)

378: 		    function validateCreateOrderHash(address targetTokenReceiver, uint256 createOrderHash, bytes memory encodedOrder, IDelegateRegistry.DelegationType tokenType) internal view {

393: 		    function calculateOrderHash(address targetTokenReceiver, address conduit, bytes memory createOrderInfo, IDelegateRegistry.DelegationType tokenType)
```
[[184](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L184), [199](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L199), [257](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L257), [274](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L274), [292](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L292), [326](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L326), [346](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L346), [378](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L378), [393](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L393)]



```solidity
File: src/libraries/DelegateTokenLib.sol

91: 		    function revertOnCallingInvalidFlashloan(DelegateTokenStructs.FlashInfo calldata info) internal {

96: 		    function revertOnInvalidERC721ReceiverCallback(address from, address to, uint256 delegateTokenId, bytes calldata data) internal {

101: 		    function revertOnInvalidERC721ReceiverCallback(address from, address to, uint256 delegateTokenId) internal {

107: 		    function revertOldExpiry(uint256 expiry) internal view {

113: 		    function delegateIdNoRevert(address caller, uint256 salt) internal pure returns (uint256) {
```
[[91](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L91), [96](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L96), [101](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L101), [107](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L107), [113](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L113)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

16: 		    function loadTokenHolder(address delegateRegistry, bytes32 registryHash) internal view returns (address delegateTokenHolder) {

32: 		    function loadContract(address delegateRegistry, bytes32 registryHash) internal view returns (address underlyingContract) {

52: 		    function loadTokenHolderAndContract(address delegateRegistry, bytes32 registryHash) internal view returns (address delegateTokenHolder, address underlyingContract) {

69: 		    function loadFrom(address delegateRegistry, bytes32 registryHash) internal view returns (address) {

82: 		    function loadAmount(address delegateRegistry, bytes32 registryHash) internal view returns (uint256) {

94: 		    function loadRights(address delegateRegistry, bytes32 registryHash) internal view returns (bytes32) {

106: 		    function loadTokenId(address delegateRegistry, bytes32 registryHash) internal view returns (uint256) {

119: 		    function calculateDecreasedAmount(address delegateRegistry, bytes32 registryHash, uint256 decreaseAmount) internal view returns (uint256) {

133: 		    function calculateIncreasedAmount(address delegateRegistry, bytes32 registryHash, uint256 increaseAmount) internal view returns (uint256) {

140: 		    function revertERC721FlashUnavailable(address delegateRegistry, Structs.FlashInfo calldata info) internal view {

152: 		    function revertERC20FlashAmountUnavailable(address delegateRegistry, Structs.FlashInfo calldata info) internal view {

162: 		    function revertERC1155FlashAmountUnavailable(address delegateRegistry, Structs.FlashInfo calldata info) internal view {

174: 		    function transferERC721(

194: 		    function transferERC20(

218: 		    function transferERC1155(

240: 		    function delegateERC721(address delegateRegistry, bytes32 newRegistryHash, Structs.DelegateInfo calldata delegateInfo) internal {

250: 		    function incrementERC20(address delegateRegistry, bytes32 newRegistryHash, Structs.DelegateInfo calldata delegateInfo) internal {

261: 		    function incrementERC1155(address delegateRegistry, bytes32 newRegistryHash, Structs.DelegateInfo calldata delegateInfo) internal {

275: 		    function revokeERC721(

291: 		    function decrementERC20(

309: 		    function decrementERC1155(
```
[[16](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L16), [32](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L32), [52](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L52), [69](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L69), [82](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L82), [94](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L94), [106](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L106), [119](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L119), [133](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L133), [140](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L140), [152](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L152), [162](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L162), [174](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L174), [194](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L194), [218](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L218), [240](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L240), [250](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L250), [261](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L261), [275](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L275), [291](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L291), [309](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L309)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

37: 		    function writeApproved(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId, address approved) internal {

44: 		    function writeExpiry(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId, uint256 expiry) internal {

50: 		    function writeRegistryHash(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId, bytes32 registryHash) internal {

54: 		    function writeUnderlyingAmount(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId, uint256 underlyingAmount) internal {

58: 		    function incrementBalance(mapping(address delegateTokenHolder => uint256 balance) storage balances, address delegateTokenHolder) internal {

64: 		    function decrementBalance(mapping(address delegateTokenHolder => uint256 balance) storage balances, address delegateTokenHolder) internal {

72: 		    function burnPrincipal(address principalToken, Structs.Uint256 storage principalBurnAuthorization, uint256 delegateTokenId) internal {

84: 		    function mintPrincipal(address principalToken, Structs.Uint256 storage principalMintAuthorization, address principalRecipient, uint256 delegateTokenId) internal {

96: 		    function checkBurnAuthorized(address principalToken, Structs.Uint256 storage principalBurnAuthorization) internal view {

104: 		    function checkMintAuthorized(address principalToken, Structs.Uint256 storage principalMintAuthorization) internal view {

112: 		    function principalIsCaller(address principalToken) internal view {

117: 		    function revertAlreadyExisted(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId) internal view {

122: 		    function revertNotOperator(mapping(address account => mapping(address operator => bool enabled)) storage accountOperator, address account) internal view {

127: 		    function readApproved(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId) internal view returns (address) {

131: 		    function readExpiry(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId) internal view returns (uint256) {

135: 		    function readRegistryHash(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId) internal view returns (bytes32) {

139: 		    function readUnderlyingAmount(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId) internal view returns (uint256) {

143: 		    function revertNotApprovedOrOperator(

155: 		    function revertInvalidWithdrawalConditions(

170: 		    function revertNotMinted(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId) internal view {

178: 		    function revertNotMinted(bytes32 registryHash, uint256 delegateTokenId) internal pure {
```
[[37](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L37), [44](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L44), [50](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L50), [54](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L54), [58](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L58), [64](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L64), [72](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L72), [84](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L84), [96](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L96), [104](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L104), [112](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L112), [117](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L117), [122](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L122), [127](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L127), [131](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L131), [135](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L135), [139](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L139), [143](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L143), [155](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L155), [170](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L170), [178](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L178)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

15: 		    function checkAndPullByType(Structs.Uint256 storage erc1155Pulled, Structs.DelegateInfo calldata delegateInfo) internal {

31: 		    function checkERC721BeforePull(uint256 underlyingAmount, address underlyingContract, uint256 underlyingTokenId) internal view {

40: 		    function pullERC721AfterCheck(address underlyingContract, uint256 underlyingTokenId) internal {

45: 		    function checkERC20BeforePull(uint256 underlyingAmount, address underlyingContract, uint256 underlyingTokenId) internal view {

57: 		    function pullERC20AfterCheck(address underlyingContract, uint256 pullAmount) internal {

61: 		    function checkERC1155BeforePull(Structs.Uint256 storage erc1155Pulled, uint256 pullAmount) internal {

70: 		    function pullERC1155AfterCheck(Structs.Uint256 storage erc1155Pulled, uint256 pullAmount, address underlyingContract, uint256 underlyingTokenId) internal {

77: 		    function checkERC1155Pulled(Structs.Uint256 storage erc1155Pulled, address operator) internal returns (bool) {

85: 		    function revertInvalidERC1155PullCheck(Structs.Uint256 storage erc1155PullAuthorization, address operator) internal {
```
[[15](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L15), [31](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L31), [40](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L40), [45](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L45), [57](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L57), [61](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L61), [70](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L70), [77](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L77), [85](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L85)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryHashes.sol

41: 		    function decodeType(bytes32 inputHash) internal pure returns (IDelegateRegistry.DelegationType decodedType) {

54: 		    function location(bytes32 inputHash) internal pure returns (bytes32 computedLocation) {

73: 		    function allHash(address from, bytes32 rights, address to) internal pure returns (bytes32 hash) {

95: 		    function allLocation(address from, bytes32 rights, address to) internal pure returns (bytes32 computedLocation) {

120: 		    function contractHash(address from, bytes32 rights, address to, address contract_) internal pure returns (bytes32 hash) {

143: 		    function contractLocation(address from, bytes32 rights, address to, address contract_) internal pure returns (bytes32 computedLocation) {

170: 		    function erc721Hash(address from, bytes32 rights, address to, uint256 tokenId, address contract_) internal pure returns (bytes32 hash) {

195: 		    function erc721Location(address from, bytes32 rights, address to, uint256 tokenId, address contract_) internal pure returns (bytes32 computedLocation) {

222: 		    function erc20Hash(address from, bytes32 rights, address to, address contract_) internal pure returns (bytes32 hash) {

245: 		    function erc20Location(address from, bytes32 rights, address to, address contract_) internal pure returns (bytes32 computedLocation) {

272: 		    function erc1155Hash(address from, bytes32 rights, address to, uint256 tokenId, address contract_) internal pure returns (bytes32 hash) {

297: 		    function erc1155Location(address from, bytes32 rights, address to, uint256 tokenId, address contract_) internal pure returns (bytes32 computedLocation) {
```
[[41](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L41), [54](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L54), [73](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L73), [95](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L95), [120](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L120), [143](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L143), [170](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L170), [195](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L195), [222](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L222), [245](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L245), [272](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L272), [297](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L297)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryOps.sol

6: 		    function max(uint256 x, uint256 y) internal pure returns (uint256 z) {

19: 		    function and(bool x, bool y) internal pure returns (bool z) {

26: 		    function or(bool x, bool y) internal pure returns (bool z) {
```
[[6](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L6), [19](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L19), [26](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L26)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryStorage.sol

34: 		    function packAddresses(address from, address to, address contract_) internal pure returns (bytes32 firstPacked, bytes32 secondPacked) {

50: 		    function unpackAddresses(bytes32 firstPacked, bytes32 secondPacked) internal pure returns (address from, address to, address contract_) {

64: 		    function unpackAddress(bytes32 packedSlot) internal pure returns (address unpacked) {
```
[[34](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L34), [50](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L50), [64](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L64)]

</details>

---

### [NC-38] Missing underscore prefix for non-external variables

This convention is suggested for non-external state variables (private or internal). [Documentation](https://docs.soliditylang.org/en/latest/style-guide.html#underscore-prefix-for-non-external-functions-and-variables)

*There are 12 instances of this issue.*


```solidity
File: src/CreateOfferer.sol

26: 		    Structs.TransientState internal transientState;

27: 		    Structs.Nonce internal nonce;
```
[[26](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L26), [27](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L27)]



```solidity
File: src/DelegateToken.sol

33: 		    mapping(uint256 delegateTokenId => uint256[3] info) internal delegateTokenInfo;

36: 		    mapping(address delegateTokenHolder => uint256 balance) internal balances;

39: 		    mapping(address account => mapping(address operator => bool enabled)) internal accountOperator;

42: 		    Structs.Uint256 internal principalMintAuthorization = Structs.Uint256(StorageHelpers.MINT_NOT_AUTHORIZED);

43: 		    Structs.Uint256 internal principalBurnAuthorization = Structs.Uint256(StorageHelpers.BURN_NOT_AUTHORIZED);

46: 		    Structs.Uint256 internal erc1155PullAuthorization = Structs.Uint256(TransferHelpers.ERC1155_NOT_PULLED);
```
[[33](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L33), [36](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L36), [39](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L39), [42](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L42), [43](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L43), [46](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L46)]



```solidity
File: src/libraries/CreateOffererLib.sol

139: 		    CreateOffererStructs.Stage private stage;
```
[[139](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L139)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

18: 		    mapping(bytes32 delegationHash => bytes32[5] delegationStorage) internal delegations;

21: 		    mapping(address from => bytes32[] delegationHashes) internal outgoingDelegationHashes;

24: 		    mapping(address to => bytes32[] delegationHashes) internal incomingDelegationHashes;
```
[[18](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L18), [21](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L21), [24](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L24)]


---

### [NC-39] Invalid NatSpec comment style

NatSpec [must](https://docs.soliditylang.org/en/latest/natspec-format.html#documentation-example) begin with `///`, or use the `/* ... */` syntax.

*There is 1 instance of this issue.*


```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

101: 		    // @inheritdoc IDelegateRegistry
```
[[101](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L101)]


---

### [NC-40] Missing NatSpec from contract declarations

Some contracts miss a `@dev/@notice` NatSpec, which should be a [best practice](https://docs.soliditylang.org/en/latest/natspec-format.html) to add as a documentation.

*There are 5 instances of this issue.*


```solidity
File: src/libraries/CreateOffererLib.sol

10: 		library CreateOffererErrors {

33: 		library CreateOffererEnums {

64: 		library CreateOffererStructs {
```
[[10](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L10), [33](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L33), [64](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L64)]



```solidity
File: src/libraries/DelegateTokenLib.sol

8: 		library DelegateTokenStructs {

42: 		library DelegateTokenErrors {
```
[[8](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L8), [42](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L42)]


---

### [NC-41] Missing NatSpec `@title`

Some contract definitions have an incomplete NatSpec: add a `@title` notation to describe the contract to improve the code documentation.

*There are 10 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/CreateOfferer.sol

22: 		/// @dev Experimental way to create delegate tokens with seaport and existing seaport conduit approvals
```
[[22](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L22)]



```solidity
File: src/DelegateToken.sol

15: 		contract DelegateToken is ReentrancyGuard, IDelegateToken {
```
[[15](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L15)]



```solidity
File: src/PrincipalToken.sol

9: 		/// @notice A simple NFT that doesn't store any user data, being tightly linked to the stateful Delegate Token.
```
[[9](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L9)]



```solidity
File: src/libraries/CreateOffererLib.sol

10: 		library CreateOffererErrors {
```
[[10](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L10)]



```solidity
File: src/libraries/DelegateTokenLib.sol

8: 		library DelegateTokenStructs {
```
[[8](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L8)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

8: 		library DelegateTokenRegistryHelpers {
```
[[8](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L8)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

7: 		library DelegateTokenStorageHelpers {
```
[[7](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L7)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

10: 		library DelegateTokenTransferHelpers {
```
[[10](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L10)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryOps.sol

4: 		library RegistryOps {
```
[[4](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L4)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryStorage.sol

4: 		library RegistryStorage {
```
[[4](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L4)]

</details>

---

### [NC-42] Missing NatSpec `@author`

Some contract definitions have an incomplete NatSpec: add a `@author` notation to improve the code documentation.

*There are 12 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/CreateOfferer.sol

22: 		/// @dev Experimental way to create delegate tokens with seaport and existing seaport conduit approvals
```
[[22](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L22)]



```solidity
File: src/DelegateToken.sol

15: 		contract DelegateToken is ReentrancyGuard, IDelegateToken {
```
[[15](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L15)]



```solidity
File: src/PrincipalToken.sol

9: 		/// @notice A simple NFT that doesn't store any user data, being tightly linked to the stateful Delegate Token.
```
[[9](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L9)]



```solidity
File: src/libraries/CreateOffererLib.sol

10: 		library CreateOffererErrors {
```
[[10](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L10)]



```solidity
File: src/libraries/DelegateTokenLib.sol

8: 		library DelegateTokenStructs {
```
[[8](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L8)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

8: 		library DelegateTokenRegistryHelpers {
```
[[8](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L8)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

7: 		library DelegateTokenStorageHelpers {
```
[[7](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L7)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

10: 		library DelegateTokenTransferHelpers {
```
[[10](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L10)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

13: 		 * @custom:coauthor mireynolds
```
[[13](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L13)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryHashes.sol

6: 		/**
```
[[6](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryHashes.sol#L6)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryOps.sol

4: 		library RegistryOps {
```
[[4](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L4)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryStorage.sol

4: 		library RegistryStorage {
```
[[4](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryStorage.sol#L4)]

</details>

---

### [NC-43] Missing NatSpec from function definitions

Some functions miss a NatSpec, which should be a [best practice](https://docs.soliditylang.org/en/latest/natspec-format.html) to add as a documentation.

Even if Natspec for internal and private function is not parsed (but this may change in the future, according to the official docs), it still helps while reviewing the codebase.

*There are 2 instances of this issue.*


```solidity
File: src/libraries/DelegateTokenLib.sol

91: 		    function revertOnCallingInvalidFlashloan(DelegateTokenStructs.FlashInfo calldata info) internal {
```
[[91](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L91)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

15: 		    function checkAndPullByType(Structs.Uint256 storage erc1155Pulled, Structs.DelegateInfo calldata delegateInfo) internal {
```
[[15](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L15)]


---

### [NC-44] Missing NatSpec `@param`

Some functions have an incomplete NatSpec: add a `@param` notation to describe the function parameters to improve the code documentation.

*There are 45 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/CreateOfferer.sol

// @audit missing fulfiller
44: 		    /**
45: 		     * @notice Implementation of seaport contract offerer generateOrder
46: 		     * @param minimumReceived The "ghost" create offerer token to be ordered
47: 		     * @param maximumSpent The underlying token required during the liquid delegate create process
48: 		     * @param context The upper bits of context should be encoded with the CreateOffererStruct
49: 		     * @return offer Returns minimumReceived
50: 		     * @return consideration Returns maximumSpent but with the beneficiary specified as this contract
51: 		     */
52: 		    function generateOrder(address fulfiller, SpentItem[] calldata minimumReceived, SpentItem[] calldata maximumSpent, bytes calldata context)

64: 		    /**
65: 		     * @notice Implementation of seaport contract offerer generateOrder
66: 		     * @param offer The delegateToken created during transfer
67: 		     * @param consideration The underlying used for create during transfer
68: 		     * @param context The upper bits of context should be encoded with the CreateOffererStruct
69: 		     * @param contractNonce Should match with the nonce tracked by this contract
70: 		     */
71: 		    function ratifyOrder(SpentItem[] calldata offer, ReceivedItem[] calldata consideration, bytes calldata context, bytes32[] calldata, uint256 contractNonce)

// @audit missing context
168: 		    /**
169: 		     * @notice Implementation of seaport contract offerer previewOrder
170: 		     * @param caller Must be the seaport address
171: 		     * @param minimumReceived The "ghost" create offerer token to be ordered
172: 		     * @param maximumSpent The underlying token required during the liquid delegate create process
173: 		     * @return offer Returns minimumReceived
174: 		     * @return consideration Returns maximumSpent but with the beneficiary specified as this contract
175: 		     */
176: 		    function previewOrder(address caller, address, SpentItem[] calldata minimumReceived, SpentItem[] calldata maximumSpent, bytes calldata context)
```
[[44-52](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L44-L52), [64-71](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L64-L71), [168-176](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L168-L176)]



```solidity
File: src/DelegateToken.sol

// @audit missing interfaceId
61: 		    /*//////////////////////////////////////////////////////////////
62: 		    /                    Supported Interfaces                      /
63: 		    //////////////////////////////////////////////////////////////*/
64: 		
65: 		    function supportsInterface(bytes4 interfaceId) external pure returns (bool) {
```
[[61-65](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L61-L65)]



```solidity
File: src/PrincipalToken.sol

// @audit missing to, id
32: 		    /// @notice Mints a PT if and only if the DT contract calls and has authorized
33: 		    function mint(address to, uint256 id) external {

// @audit missing spender, id
39: 		    /// @notice Burns a PT if the DT contract authorizes and the spender isApprovedOrOwner and DT owner authorizes
40: 		    function burn(address spender, uint256 id) external {
```
[[32-33](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L32-L33), [39-40](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L39-L40)]



```solidity
File: src/libraries/CreateOffererLib.sol

// @audit missing fulfiller
191: 		    /**
192: 		     * @notice Updates a TransientState struct in storage with order data
193: 		     * @param transientState The storage pointer to the TransientState struct to be updated
194: 		     * @param minimumReceived Used to decode the token id of the CreateOfferer "ghost" token offer
195: 		     * @param maximumSpent Contains the information of the underlying token to be used in create
196: 		     * @param decodedContext Is the Context struct decoded and provides additional data need for the Order structs
197: 		     * @dev Only one of the transient order data types will be updated
198: 		     */
199: 		    function updateTransientState(

// @audit missing receivers
283: 		    /**
284: 		     * @notice Verifies the properties of a delegateToken against the first element of a seaport ContractOfferer ratify order calldata
285: 		     * @param delegateToken Should be the address of the DelegateToken contract
286: 		     * @param identifier The offer identifier
287: 		     * @param consideration The consideration specified in the ratify order call data (used as input data of the underlying used to create the delegate token)
288: 		     * @param context Should contain an unpacked encoding of the Context struct which provides additional order data for comparison
289: 		     * @dev Should revert if the delegateToken with tokenId in the offer does not match with the expected result
290: 		     * @dev Should revert if context is the wrong length
291: 		     */
292: 		    function verifyCreate(address delegateToken, uint256 identifier, CreateOffererStructs.Receivers storage receivers, ReceivedItem calldata consideration, bytes calldata context)
```
[[191-199](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L191-L199), [283-292](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L283-L292)]



```solidity
File: src/libraries/DelegateTokenLib.sol

// @audit missing expiry
106: 		    /// @dev won't revert if expiry is too large (i.e. > type(uint96).max)
107: 		    function revertOldExpiry(uint256 expiry) internal view {
```
[[106-107](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L106-L107)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

// @audit missing delegateRegistry, registryHash, from, newRegistryHash, to, underlyingRights, underlyingContract, underlyingTokenId
173: 		    /// @dev Will not revert if from didn't have a delegation in the first place
174: 		    function transferERC721(

// @audit missing delegateRegistry, registryHash, from, newRegistryHash, to, underlyingAmount, underlyingRights, underlyingContract
191: 		    /// @dev Will not revert if from didn't have a delegation in the first place
192: 		    /// @dev Will not revert an underflow value if from's existing delegation amount > underlyingAmount
193: 		    /// @dev Will not revert an overflow value if to's existing delegation + underlyingAmount > type(uint256).max
194: 		    function transferERC20(

// @audit missing delegateRegistry, registryHash, from, newRegistryHash, to, underlyingAmount, underlyingRights, underlyingContract, underlyingTokenId
215: 		    /// @dev Will not revert if from didn't have a delegation in the first place
216: 		    /// @dev Will not revert an underflow value if from's existing delegation amount > underlyingAmount
217: 		    /// @dev Will not revert an overflowed value if to's existing delegation + underlyingAmount > type(uint256).max
218: 		    function transferERC1155(

// @audit missing delegateRegistry, newRegistryHash, delegateInfo
239: 		    /// @dev Will not revert if delegateHolder had a delegation in the first place
240: 		    function delegateERC721(address delegateRegistry, bytes32 newRegistryHash, Structs.DelegateInfo calldata delegateInfo) internal {

// @audit missing delegateRegistry, newRegistryHash, delegateInfo
248: 		    /// @dev Will not revert if delegateHolder had a delegation in the first place
249: 		    /// @dev Will not revert an overflow value if delegateHolder's existing delegation + amount > type(uint256).max
250: 		    function incrementERC20(address delegateRegistry, bytes32 newRegistryHash, Structs.DelegateInfo calldata delegateInfo) internal {

// @audit missing delegateRegistry, newRegistryHash, delegateInfo
259: 		    /// @dev Will not revert if delegateHolder had a delegation in the first place
260: 		    /// @dev Will not revert an overflow value if delegateHolder's existing delegation + amount > type(uint256).max
261: 		    function incrementERC1155(address delegateRegistry, bytes32 newRegistryHash, Structs.DelegateInfo calldata delegateInfo) internal {

// @audit missing delegateRegistry, registryHash, delegateTokenHolder, underlyingContract, underlyingTokenId, underlyingRights
274: 		    /// @dev Will not revert if delegateHolder never had a delegation in the first place
275: 		    function revokeERC721(

// @audit missing delegateRegistry, registryHash, delegateTokenHolder, underlyingContract, underlyingAmount, underlyingRights
289: 		    /// @dev Will not revert if delegateHolder never had a delegation in the first place
290: 		    /// @dev Will not revert an underflow value if delegateHolder's existing delegation - underlyingAmount < 0
291: 		    function decrementERC20(

// @audit missing delegateRegistry, registryHash, delegateTokenHolder, underlyingContract, underlyingTokenId, underlyingAmount, underlyingRights
307: 		    /// @dev Will not revert if delegateHolder never had a delegation in the first place
308: 		    /// @dev Will not revert an underflow value if delegateHolder's existing delegation - underlyingAmount < 0
309: 		    function decrementERC1155(
```
[[173-174](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L173-L174), [191-194](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L191-L194), [215-218](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L215-L218), [239-240](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L239-L240), [248-250](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L248-L250), [259-261](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L259-L261), [274-275](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L274-L275), [289-291](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L289-L291), [307-309](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L307-L309)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

// @audit missing delegateTokenInfo, delegateTokenId, approved
36: 		    /// @dev should preserve the expiry in the lower 96 bits in storage, and update the upper 160 bits with approved address
37: 		    function writeApproved(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId, address approved) internal {

// @audit missing delegateTokenInfo, delegateTokenId, expiry
42: 		    /// @dev should preserve approved in the upper 160 bits, and update the lower 96 bits with expiry
43: 		    /// @dev should revert if expiry exceeds 96 bits
44: 		    function writeExpiry(mapping(uint256 delegateTokenId => uint256[3] info) storage delegateTokenInfo, uint256 delegateTokenId, uint256 expiry) internal {

// @audit missing principalToken, principalBurnAuthorization, delegateTokenId
70: 		    /// @notice helper function for burning a principal token
71: 		    /// @dev must revert if burnAuthorized is not set to BURN_NOT_AUTHORIZED flag
72: 		    function burnPrincipal(address principalToken, Structs.Uint256 storage principalBurnAuthorization, uint256 delegateTokenId) internal {

// @audit missing principalToken, principalMintAuthorization, principalRecipient, delegateTokenId
82: 		    /// @notice helper function for minting a principal token
83: 		    /// @dev must revert if mintAuthorized has already been set to MINT_AUTHORIZED flag
84: 		    function mintPrincipal(address principalToken, Structs.Uint256 storage principalMintAuthorization, address principalRecipient, uint256 delegateTokenId) internal {

// @audit missing principalToken, principalBurnAuthorization
94: 		    /// @dev must revert if delegate token did not call burn on the Principal Token for the delegateTokenId
95: 		    /// @dev must revert if principal token is not the caller
96: 		    function checkBurnAuthorized(address principalToken, Structs.Uint256 storage principalBurnAuthorization) internal view {

// @audit missing principalToken, principalMintAuthorization
102: 		    /// @dev must revert if delegate token did not call burn on the Principal Token for the delegateTokenId
103: 		    /// @dev must revert if principal token is not the caller
104: 		    function checkMintAuthorized(address principalToken, Structs.Uint256 storage principalMintAuthorization) internal view {

// @audit missing principalToken
110: 		    /// @notice helper function to revert if caller is not Principal Token
111: 		    /// @dev must revert if msg.sender is not the principal token
112: 		    function principalIsCaller(address principalToken) internal view {

// @audit missing delegateTokenInfo, accountOperator, delegateTokenId, delegateTokenHolder
153: 		    /// @dev should only revert if expiry has not expired AND caller is not the delegateTokenHolder AND not approved for the delegateTokenId AND not an operator for
154: 		    /// delegateTokenHolder
155: 		    function revertInvalidWithdrawalConditions(

// @audit missing registryHash, delegateTokenId
177: 		    /// @dev does not read from storage, make sure the registryHash of the corresponding delegateTokenId is passed to have the intended effect
178: 		    function revertNotMinted(bytes32 registryHash, uint256 delegateTokenId) internal pure {
```
[[36-37](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L36-L37), [42-44](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L42-L44), [70-72](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L70-L72), [82-84](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L82-L84), [94-96](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L94-L96), [102-104](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L102-L104), [110-112](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L110-L112), [153-155](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L153-L155), [177-178](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L177-L178)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

// @audit missing underlyingAmount, underlyingContract, underlyingTokenId
30: 		    /// @dev Should revert for a typical 20 / 1155, and pass for a typical 721
31: 		    function checkERC721BeforePull(uint256 underlyingAmount, address underlyingContract, uint256 underlyingTokenId) internal view {

// @audit missing underlyingAmount, underlyingContract, underlyingTokenId
44: 		    /// @dev Should revert for a typical 721 / 1155 and pass for a typical 20
45: 		    function checkERC20BeforePull(uint256 underlyingAmount, address underlyingContract, uint256 underlyingTokenId) internal view {
```
[[30-31](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L30-L31), [44-45](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L44-L45)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

// @audit missing location
296: 		    /**
297: 		     * ----------- EXTERNAL STORAGE ACCESS -----------
298: 		     */
299: 		
300: 		    function readSlot(bytes32 location) external view returns (bytes32 contents) {

// @audit missing from, to, delegationHash
333: 		    /**
334: 		     * ----------- INTERNAL -----------
335: 		     */
336: 		
337: 		    /// @dev Helper function to push new delegation hashes to the incoming and outgoing hashes mappings
338: 		    function _pushDelegationHashes(address from, address to, bytes32 delegationHash) internal {

// @audit missing location, position, data
343: 		    /// @dev Helper function that writes bytes32 data to delegation data location at array position
344: 		    function _writeDelegation(bytes32 location, uint256 position, bytes32 data) internal {

// @audit missing location, position, data
350: 		    /// @dev Helper function that writes uint256 data to delegation data location at array position
351: 		    function _writeDelegation(bytes32 location, uint256 position, uint256 data) internal {

// @audit missing location, from, to, contract_
357: 		    /// @dev Helper function that writes addresses according to the packing rule for delegation storage
358: 		    function _writeDelegationAddresses(bytes32 location, address from, address to, address contract_) internal {

// @audit missing location, from
368: 		    /// @dev Helper function that writes from whilst preserving the rest of the storage slot
369: 		    function _updateFrom(bytes32 location, address from) internal {

// @audit missing hashes
379: 		    /// @dev Helper function that takes an array of delegation hashes and returns an array of Delegation structs with their onchain information
380: 		    function _getValidDelegationsFromHashes(bytes32[] storage hashes) internal view returns (Delegation[] memory delegations_) {

// @audit missing hashes
410: 		    /// @dev Helper function that takes an array of delegation hashes and returns an array of valid delegation hashes
411: 		    function _getValidDelegationHashesFromHashes(bytes32[] storage hashes) internal view returns (bytes32[] memory validHashes) {

// @audit missing location, position
429: 		    /// @dev Helper function that loads delegation data from a particular array position and returns as bytes32
430: 		    function _loadDelegationBytes32(bytes32 location, uint256 position) internal view returns (bytes32 data) {

// @audit missing location, position
436: 		    /// @dev Helper function that loads delegation data from a particular array position and returns as uint256
437: 		    function _loadDelegationUint(bytes32 location, uint256 position) internal view returns (uint256 data) {

// @audit missing location
443: 		    // @dev Helper function that loads the from address from storage according to the packing rule for delegation storage
444: 		    function _loadFrom(bytes32 location) internal view returns (address) {

// @audit missing location, from
453: 		    /// @dev Helper function to establish whether a delegation is enabled
454: 		    function _validateFrom(bytes32 location, address from) internal view returns (bool) {

// @audit missing location
458: 		    /// @dev Helper function that loads the address for the delegation according to the packing rule for delegation storage
459: 		    function _loadDelegationAddresses(bytes32 location) internal view returns (address from, address to, address contract_) {
```
[[296-300](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L296-L300), [333-338](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L333-L338), [343-344](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L343-L344), [350-351](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L350-L351), [357-358](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L357-L358), [368-369](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L368-L369), [379-380](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L379-L380), [410-411](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L410-L411), [429-430](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L429-L430), [436-437](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L436-L437), [443-444](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L443-L444), [453-454](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L453-L454), [458-459](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L458-L459)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryOps.sol

// @audit missing x, y
5: 		    /// @dev `x > y ? x : y`.
6: 		    function max(uint256 x, uint256 y) internal pure returns (uint256 z) {

// @audit missing x, y
18: 		    /// @dev `x & y`.
19: 		    function and(bool x, bool y) internal pure returns (bool z) {

// @audit missing x, y
25: 		    /// @dev `x | y`.
26: 		    function or(bool x, bool y) internal pure returns (bool z) {
```
[[5-6](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L5-L6), [18-19](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L18-L19), [25-26](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L25-L26)]

</details>

---

### [NC-45] Incomplete NatSpec `@return`

Some functions have an incomplete NatSpec: add a `@return` notation to describe the function return value to improve the code documentation.

*There are 23 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/CreateOfferer.sol

// @audit missing @return
64: 		    /**
65: 		     * @notice Implementation of seaport contract offerer generateOrder
66: 		     * @param offer The delegateToken created during transfer
67: 		     * @param consideration The underlying used for create during transfer
68: 		     * @param context The upper bits of context should be encoded with the CreateOffererStruct
69: 		     * @param contractNonce Should match with the nonce tracked by this contract
70: 		     */
71: 		    function ratifyOrder(SpentItem[] calldata offer, ReceivedItem[] calldata consideration, bytes calldata context, bytes32[] calldata, uint256 contractNonce)

// @audit missing @return
240: 		    /// @notice Implementation of seaport contract offerer getSeaportMetadata
241: 		    function getSeaportMetadata() external pure returns (string memory, Schema[] memory) {
```
[[64-71](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L64-L71), [240-241](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L240-L241)]



```solidity
File: src/DelegateToken.sol

// @audit missing @return
61: 		    /*//////////////////////////////////////////////////////////////
62: 		    /                    Supported Interfaces                      /
63: 		    //////////////////////////////////////////////////////////////*/
64: 		
65: 		    function supportsInterface(bytes4 interfaceId) external pure returns (bool) {
```
[[61-65](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L61-L65)]



```solidity
File: src/libraries/CreateOffererLib.sol

// @audit missing @return
265: 		    /**
266: 		     * @notice Calculates the CreateOfferer hash, agnostic to the type
267: 		     * @param delegateToken Should be the address of the DelegateToken contract
268: 		     * @param targetTokenReceiver The receiver of the targetToken in orderInfo
269: 		     * @param conduit The address of the conduit that should conduct the create on transferFrom on seaport calling CreateOfferer
270: 		     * @param orderInfo Should be abi encoded (unpacked) with the relevant token type Order struct
271: 		     * @param delegationType Delegation type that should correspond to the token type encoded into orderInfo
272: 		     * @dev Should revert if a delegateToken has already been created with the parameters above
273: 		     */
274: 		    function calculateOrderHashAndId(address delegateToken, address targetTokenReceiver, address conduit, bytes memory orderInfo, IDelegateRegistry.DelegationType delegationType)

// @audit missing @return
319: 		    /**
320: 		     * @notice Calculates an effective expiry for an order at the time of execution
321: 		     * @param expiryType Defines the type of expiry, should be relative or absolute
322: 		     * @param expiryLength Length of the expiry given its reference point
323: 		     * @dev Must revert if the expiryType is invalid
324: 		     * @dev The reference for relative expiry types is block.timestamp
325: 		     */
326: 		    function calculateExpiry(CreateOffererEnums.ExpiryType expiryType, uint256 expiryLength) internal view returns (uint256) {

// @audit missing @return
385: 		    /**
386: 		     * @notice The order hash system used by CreateOfferer
387: 		     * @param targetTokenReceiver Should be the intended receiver of the targetToken in createOrderInfo
388: 		     * @param conduit Should be the intended conduit to be used in the corresponding seaport order
389: 		     * @param createOrderInfo should be the unpacked encoding for a given token type order info
390: 		     * @param tokenType Should match with the token type used in the encoded createOrderInfo
391: 		     * @dev tokenType is encoded in the last byte of the hash after it has been shifted left by a byte
392: 		     */
393: 		    function calculateOrderHash(address targetTokenReceiver, address conduit, bytes memory createOrderInfo, IDelegateRegistry.DelegationType tokenType)
```
[[265-274](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L265-L274), [319-326](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L319-L326), [385-393](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L385-L393)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

// @audit missing @return
63: 		    /**
64: 		     * @notice Loads the "from" address from a given registryHash
65: 		     * @param delegateRegistry Address of the DelegateRegistry v2 contract
66: 		     * @param registryHash The hash of the delegation to retrieve data for
67: 		     * @dev Will not revert if delegation has been revoked or never existed
68: 		     */
69: 		    function loadFrom(address delegateRegistry, bytes32 registryHash) internal view returns (address) {

// @audit missing @return
77: 		    /**
78: 		     * @notice Loads the "amount" from a given registryHash
79: 		     * @param delegateRegistry Address of the DelegateRegistry v2 contract
80: 		     * @param registryHash The hash of the delegation to retrieve data for
81: 		     */
82: 		    function loadAmount(address delegateRegistry, bytes32 registryHash) internal view returns (uint256) {

// @audit missing @return
88: 		    /**
89: 		     * @notice Loads the "rights" from a given registryHash
90: 		     * @param delegateRegistry Address of the DelegateRegistry v2 contract
91: 		     * @param registryHash The hash of the delegation to retrieve data for
92: 		     * @dev Will not return empty or revert if delegation has been revoked
93: 		     */
94: 		    function loadRights(address delegateRegistry, bytes32 registryHash) internal view returns (bytes32) {

// @audit missing @return
100: 		    /**
101: 		     * @notice Loads the "tokenId" from a given registryHash
102: 		     * @param delegateRegistry Address of the DelegateRegistry v2 contract
103: 		     * @param registryHash The hash of the delegation to retrieve data for
104: 		     * @dev Will not revert or return 0 if delegation has been revoked
105: 		     */
106: 		    function loadTokenId(address delegateRegistry, bytes32 registryHash) internal view returns (uint256) {

// @audit missing @return
112: 		    /**
113: 		     * @notice Calculates a new decreased value given an "amount" from a given registryHash
114: 		     * @param delegateRegistry Address of the DelegateRegistry v2 contract
115: 		     * @param registryHash The hash of the delegation to retrieve data for
116: 		     * @param decreaseAmount The value to decrement "amount" by
117: 		     * @dev Assumes the decreased amount won't underflow with "amount"
118: 		     */
119: 		    function calculateDecreasedAmount(address delegateRegistry, bytes32 registryHash, uint256 decreaseAmount) internal view returns (uint256) {

// @audit missing @return
126: 		    /**
127: 		     * @notice Calculates a new increased value given an "amount" from a given registryHash
128: 		     * @param delegateRegistry Address of the DelegateRegistry v2 contract
129: 		     * @param registryHash The hash of the delegation to retrieve data for
130: 		     * @param increaseAmount The value to increment "amount" by
131: 		     * @dev Assumes the increased amount won't overflow with "amount"
132: 		     */
133: 		    function calculateIncreasedAmount(address delegateRegistry, bytes32 registryHash, uint256 increaseAmount) internal view returns (uint256) {
```
[[63-69](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L63-L69), [77-82](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L77-L82), [88-94](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L88-L94), [100-106](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L100-L106), [112-119](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L112-L119), [126-133](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L126-L133)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

// @audit missing @return
296: 		    /**
297: 		     * ----------- EXTERNAL STORAGE ACCESS -----------
298: 		     */
299: 		
300: 		    function readSlot(bytes32 location) external view returns (bytes32 contents) {

// @audit missing @return
379: 		    /// @dev Helper function that takes an array of delegation hashes and returns an array of Delegation structs with their onchain information
380: 		    function _getValidDelegationsFromHashes(bytes32[] storage hashes) internal view returns (Delegation[] memory delegations_) {

// @audit missing @return
410: 		    /// @dev Helper function that takes an array of delegation hashes and returns an array of valid delegation hashes
411: 		    function _getValidDelegationHashesFromHashes(bytes32[] storage hashes) internal view returns (bytes32[] memory validHashes) {

// @audit missing @return
429: 		    /// @dev Helper function that loads delegation data from a particular array position and returns as bytes32
430: 		    function _loadDelegationBytes32(bytes32 location, uint256 position) internal view returns (bytes32 data) {

// @audit missing @return
436: 		    /// @dev Helper function that loads delegation data from a particular array position and returns as uint256
437: 		    function _loadDelegationUint(bytes32 location, uint256 position) internal view returns (uint256 data) {

// @audit missing @return
443: 		    // @dev Helper function that loads the from address from storage according to the packing rule for delegation storage
444: 		    function _loadFrom(bytes32 location) internal view returns (address) {

// @audit missing @return
453: 		    /// @dev Helper function to establish whether a delegation is enabled
454: 		    function _validateFrom(bytes32 location, address from) internal view returns (bool) {

// @audit missing @return
458: 		    /// @dev Helper function that loads the address for the delegation according to the packing rule for delegation storage
459: 		    function _loadDelegationAddresses(bytes32 location) internal view returns (address from, address to, address contract_) {
```
[[296-300](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L296-L300), [379-380](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L379-L380), [410-411](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L410-L411), [429-430](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L429-L430), [436-437](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L436-L437), [443-444](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L443-L444), [453-454](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L453-L454), [458-459](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L458-L459)]



```solidity
File: lib/delegate-registry/src/libraries/RegistryOps.sol

// @audit missing @return
5: 		    /// @dev `x > y ? x : y`.
6: 		    function max(uint256 x, uint256 y) internal pure returns (uint256 z) {

// @audit missing @return
18: 		    /// @dev `x & y`.
19: 		    function and(bool x, bool y) internal pure returns (bool z) {

// @audit missing @return
25: 		    /// @dev `x | y`.
26: 		    function or(bool x, bool y) internal pure returns (bool z) {
```
[[5-6](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L5-L6), [18-19](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L18-L19), [25-26](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/libraries/RegistryOps.sol#L25-L26)]

</details>

---

## Gas Optimizations

---

### [G-01] Multiple `mapping`s that share an ID can be combined into a single `mapping` of ID / `struct`

This can avoid a Gsset (**20000 Gas**) per mapping combined. Reads and writes will also be cheaper when a function requires both values as they both can fit in the same storage slot.Finally, if both fields are accessed in the same function, this can save **~42 gas** per access due to not having to recalculate the key's `keccak256` hash (Gkeccak256 - **30 Gas**) and that calculation's associated stack operations.

*There is 1 instance of this issue.*


```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

// @audit consider merging outgoingDelegationHashes, incomingDelegationHashes
21: 		    mapping(address from => bytes32[] delegationHashes) internal outgoingDelegationHashes;

24: 		    mapping(address to => bytes32[] delegationHashes) internal incomingDelegationHashes;
```
[[21](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L21)]


---

### [G-02] Cache state variables with stack variables

Caching of a state variable replaces each Gwarmaccess (**100 gas**) with a cheaper stack read. Other less obvious fixes/optimizations include having local memory caches of state variable structs, or having local caches of state variable contracts/addresses.

*There are 14 instances of this issue.*


```solidity
File: src/CreateOfferer.sol

// @audit transientState on lines 104, 106, 116, 128, 130, 142, 152, 91, 94
154: 		                    delegateHolder: erc1155Order.info.targetToken == Enums.TargetToken.delegate ? targetTokenReceiver : transientState.receivers.fulfiller,
```
[[154](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L154)]



```solidity
File: src/DelegateToken.sol

// @audit delegateTokenInfo on line 112
113: 		        return StorageHelpers.readApproved(delegateTokenInfo, delegateTokenId);

// @audit delegateTokenInfo on line 135
139: 		        StorageHelpers.writeApproved(delegateTokenInfo, delegateTokenId, spender);

// @audit delegateTokenInfo on lines 163, 171, 179, 183, 190, 197
204: 		                StorageHelpers.readUnderlyingAmount(delegateTokenInfo, delegateTokenId),

// @audit balances on line 169
170: 		        StorageHelpers.decrementBalance(balances, from);

// @audit delegateTokenInfo on line 228
233: 		            StorageHelpers.readExpiry(delegateTokenInfo, delegateTokenId),

// @audit delegateTokenInfo on line 240
243: 		        return spender == delegateTokenHolder || accountOperator[delegateTokenHolder][spender] || StorageHelpers.readApproved(delegateTokenInfo, delegateTokenId) == spender;

// @audit delegateTokenInfo on lines 266, 272
276: 		        else delegateInfo.amount = StorageHelpers.readUnderlyingAmount(delegateTokenInfo, delegateTokenId);

// @audit delegateTokenInfo on lines 301, 303, 308, 311, 313, 316
318: 		            StorageHelpers.writeRegistryHash(delegateTokenInfo, delegateTokenId, newRegistryHash);

// @audit delegateTokenInfo on lines 326, 328
331: 		            StorageHelpers.writeExpiry(delegateTokenInfo, delegateTokenId, newExpiry);

// @audit delegateTokenInfo on lines 341, 342
346: 		            RegistryHelpers.loadTokenHolder(delegateRegistry, StorageHelpers.readRegistryHash(delegateTokenInfo, delegateTokenId)),

// @audit delegateTokenInfo on lines 354, 355, 359, 371, 372, 377
378: 		            StorageHelpers.writeUnderlyingAmount(delegateTokenInfo, delegateTokenId, 0); // Deletes amount

// @audit principalBurnAuthorization on lines 368, 374
383: 		            StorageHelpers.burnPrincipal(principalToken, principalBurnAuthorization, delegateTokenId);

// @audit erc1155PullAuthorization on line 405
408: 		            TransferHelpers.pullERC1155AfterCheck(erc1155PullAuthorization, info.amount, info.tokenContract, info.tokenId);
```
[[113](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L113), [139](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L139), [204](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L204), [170](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L170), [233](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L233), [243](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L243), [276](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L276), [318](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L318), [331](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L331), [346](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L346), [378](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L378), [383](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L383), [408](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L408)]


---

### [G-03] Avoid contract existence checks by using low level calls

Prior to Solidity 0.8.10 the compiler inserted extra code, including EXTCODESIZE (**100 gas**), to check for contract existence for external function calls.

In more recent solidity versions, the compiler will not insert these checks if the external call has a return value.

A similar behavior can be achieved in earlier versions by using low - level calls, since low level calls never check for contract existence.

*There are 34 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/libraries/CreateOffererLib.sol

258: 		        uint256 actualDelegateId = IDelegateToken(delegateToken).create(delegateInfo, createOrderHash);

280: 		        delegateTokenId = IDelegateToken(delegateToken).getDelegateId(address(this), createOrderHash); // This should revert if already existed

314: 		            ) != keccak256(abi.encode(IDelegateToken(delegateToken).getDelegateInfo(DelegateTokenHelpers.delegateIdNoRevert(address(this), identifier))))

```
[[258](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L258), [280](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L280), [314](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L314)]



```solidity
File: src/libraries/DelegateTokenLib.sol

97: 		        if (to.code.length == 0 || IERC721Receiver(to).onERC721Received(msg.sender, from, delegateTokenId, data) == IERC721Receiver.onERC721Received.selector) return;

102: 		        if (to.code.length == 0 || IERC721Receiver(to).onERC721Received(msg.sender, from, delegateTokenId, "") == IERC721Receiver.onERC721Received.selector) return;

```
[[97](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L97), [102](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L102)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

19: 		                IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_SECOND_PACKED))

37: 		                IDelegateRegistry(delegateRegistry).readSlot(bytes32(registryLocation + RegistryStorage.POSITIONS_FIRST_PACKED)),

38: 		                IDelegateRegistry(delegateRegistry).readSlot(bytes32(registryLocation + RegistryStorage.POSITIONS_SECOND_PACKED))

57: 		                IDelegateRegistry(delegateRegistry).readSlot(bytes32(registryLocation + RegistryStorage.POSITIONS_FIRST_PACKED)),

58: 		                IDelegateRegistry(delegateRegistry).readSlot(bytes32(registryLocation + RegistryStorage.POSITIONS_SECOND_PACKED))

72: 		                IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_FIRST_PACKED))

84: 		            return uint256(IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_AMOUNT)));

96: 		            return IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_RIGHTS));

108: 		            return uint256(IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_TOKEN_ID)));

122: 		                uint256(IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_AMOUNT))) - decreaseAmount;

136: 		                uint256(IDelegateRegistry(delegateRegistry).readSlot(bytes32(uint256(RegistryHashes.location(registryHash)) + RegistryStorage.POSITIONS_AMOUNT))) + increaseAmount;

185: 		            IDelegateRegistry(delegateRegistry).delegateERC721(from, underlyingContract, underlyingTokenId, underlyingRights, false) == registryHash

186: 		                && IDelegateRegistry(delegateRegistry).delegateERC721(to, underlyingContract, underlyingTokenId, underlyingRights, true) == newRegistryHash

205: 		            IDelegateRegistry(delegateRegistry).delegateERC20(
206: 		                from, underlyingContract, underlyingRights, calculateDecreasedAmount(delegateRegistry, registryHash, underlyingAmount)
207: 		            ) == bytes32(registryHash)

208: 		                && IDelegateRegistry(delegateRegistry).delegateERC20(
209: 		                    to, underlyingContract, underlyingRights, calculateIncreasedAmount(delegateRegistry, newRegistryHash, underlyingAmount)
210: 		                ) == newRegistryHash

230: 		        if (IDelegateRegistry(delegateRegistry).delegateERC1155(from, underlyingContract, underlyingTokenId, underlyingRights, amount) != registryHash) {

234: 		        if (IDelegateRegistry(delegateRegistry).delegateERC1155(to, underlyingContract, underlyingTokenId, underlyingRights, amount) != newRegistryHash) {

242: 		            IDelegateRegistry(delegateRegistry).delegateERC721(delegateInfo.delegateHolder, delegateInfo.tokenContract, delegateInfo.tokenId, delegateInfo.rights, true)

252: 		            IDelegateRegistry(delegateRegistry).delegateERC20(
253: 		                delegateInfo.delegateHolder, delegateInfo.tokenContract, delegateInfo.rights, calculateIncreasedAmount(delegateRegistry, newRegistryHash, delegateInfo.amount)
254: 		            ) == newRegistryHash

263: 		            IDelegateRegistry(delegateRegistry).delegateERC1155(
264: 		                delegateInfo.delegateHolder,
265: 		                delegateInfo.tokenContract,
266: 		                delegateInfo.tokenId,
267: 		                delegateInfo.rights,
268: 		                calculateIncreasedAmount(delegateRegistry, newRegistryHash, delegateInfo.amount)
269: 		            ) == newRegistryHash

283: 		        if (IDelegateRegistry(delegateRegistry).delegateERC721(delegateTokenHolder, underlyingContract, underlyingTokenId, underlyingRights, false) == registryHash) {

300: 		            IDelegateRegistry(delegateRegistry).delegateERC20(
301: 		                delegateTokenHolder, underlyingContract, underlyingRights, calculateDecreasedAmount(delegateRegistry, registryHash, underlyingAmount)
302: 		            ) == registryHash

319: 		            IDelegateRegistry(delegateRegistry).delegateERC1155(
320: 		                delegateTokenHolder, underlyingContract, underlyingTokenId, underlyingRights, calculateDecreasedAmount(delegateRegistry, registryHash, underlyingAmount)
321: 		            ) == registryHash
```
[[19](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L19), [37](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L37), [38](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L38), [57](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L57), [58](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L58), [72](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L72), [84](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L84), [96](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L96), [108](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L108), [122](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L122), [136](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L136), [185](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L185), [186](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L186), [205-207](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L205-L207), [208-210](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L208-L210), [230](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L230), [234](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L234), [242](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L242), [252-254](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L252-L254), [263-269](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L263-L269), [283](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L283), [300-302](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L300-L302), [319-321](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L319-L321)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

75: 		            PrincipalToken(principalToken).burn(msg.sender, delegateTokenId);

87: 		            PrincipalToken(principalToken).mint(principalRecipient, delegateTokenId);
```
[[75](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L75), [87](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L87)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

35: 		        if (IERC721(underlyingContract).ownerOf(underlyingTokenId) != msg.sender) {

41: 		        IERC721(underlyingContract).transferFrom(msg.sender, address(this), underlyingTokenId);

52: 		        if (IERC20(underlyingContract).allowance(msg.sender, address(this)) < underlyingAmount) {

71: 		        IERC1155(underlyingContract).safeTransferFrom(msg.sender, address(this), underlyingTokenId, pullAmount, "");
```
[[35](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L35), [41](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L41), [52](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L52), [71](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L71)]

</details>

---

### [G-04] Use at least Solidity version `0.8.19` to gain some gas boost

Upgrade to at least solidity version 0.8.19 to get additional gas savings. Check the [documentation](https://blog.soliditylang.org/2023/02/22/solidity-0.8.19-release-announcement/) for reference.

Some additional details:
> In earlier releases and in the default legacy code generation, when an internal library function or a free function accessed via a module was called only during contract creation, e.g. only in the constructor, a copy of the function still also occurred in the contract’s runtime bytecode.
>
>So a function pointer in creation code also refers to the offset of the function in runtime code, which requires the function to actually be present in runtime code.
>
>For direct calls to internal contract functions the full encoding of the function expression is bypassed by the compiler. However, this bypassing did not happen for internal library functions and for free functions called via modules, causing the undesirable behaviour that is now fixed in this release.

*There are 5 instances of this issue.*


```solidity
File: src/libraries/CreateOffererLib.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L2)]



```solidity
File: src/libraries/DelegateTokenLib.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L2)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L2)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L2)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L2)]


---

### [G-05] Use of `memory` instead of `calldata` for immutable arguments

Consider refactoring the function arguments from `memory` to `calldata` when they are immutable, as `calldata` is cheaper.

*There are 4 instances of this issue.*


```solidity
File: src/libraries/CreateOffererLib.sol

// @audit decodedContext
199: 		    function updateTransientState(
200: 		        CreateOffererStructs.TransientState storage transientState,
201: 		        address fulfiller,
202: 		        SpentItem calldata minimumReceived,
203: 		        SpentItem calldata maximumSpent,
204: 		        CreateOffererStructs.Context memory decodedContext

// @audit orderInfo
274: 		    function calculateOrderHashAndId(address delegateToken, address targetTokenReceiver, address conduit, bytes memory orderInfo, IDelegateRegistry.DelegationType delegationType)

// @audit encodedOrder
378: 		    function validateCreateOrderHash(address targetTokenReceiver, uint256 createOrderHash, bytes memory encodedOrder, IDelegateRegistry.DelegationType tokenType) internal view {

// @audit createOrderInfo
393: 		    function calculateOrderHash(address targetTokenReceiver, address conduit, bytes memory createOrderInfo, IDelegateRegistry.DelegationType tokenType)
```
[[199-204](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L199-L204), [274](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L274), [378](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L378), [393](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L393)]


---

### [G-06] Using `bool` for storage incurs overhead

Use `uint256(1)` and `uint256(2)` for `true`/`false` to avoid a Gwarmaccess (100 gas), and to avoid Gsset (20000 gas) when changing from `false` to `true`, after having been `true` in the past. See [source](https://github.com/OpenZeppelin/openzeppelin-contracts/blob/58f635312aa21f947cae5f8578638a85aa2519f5/contracts/security/ReentrancyGuard.sol#L23-L27).

*There is 1 instance of this issue.*


```solidity
File: src/DelegateToken.sol

39: 		    mapping(address account => mapping(address operator => bool enabled)) internal accountOperator;
```
[[39](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L39)]


---

### [G-07] Consider activating `via-ir` for deploying

The IR-based code generator was developed to make code generation more performant by enabling optimization passes that can be applied across functions.

It is possible to activate the IR-based code generator through the command line by using the flag `--via-ir` or by including the option `{"viaIR": true}`.

Keep in mind that compiling with this option may take longer. However, you can simply test it before deploying your code. If you find that it provides better performance, you can add the `--via-ir` flag to your deploy command.



---

### [G-08] Function calls should be cached instead of re-calling the function

Consider caching the result instead of re-calling the function when possible. Note: this also includes casts, which cost between 42-46 gas, depending on the type.

*There are 2 instances of this issue.*

<details>
<summary>Expand findings</summary>

```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

// @audit IDelegateRegistry(delegateRegistry) is duplicated on line 38
37: 		                IDelegateRegistry(delegateRegistry).readSlot(bytes32(registryLocation + RegistryStorage.POSITIONS_FIRST_PACKED)),

// @audit IDelegateRegistry(delegateRegistry) is duplicated on line 58
57: 		                IDelegateRegistry(delegateRegistry).readSlot(bytes32(registryLocation + RegistryStorage.POSITIONS_FIRST_PACKED)),
```
[[37](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L37), [57](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L57)]

</details>

---

### [G-09] Functions that revert when called by normal users can be `payable`

If a function modifier such as `onlyOwner` is used, the function will revert if a normal user tries to pay the function.

Marking the function as `payable` will lower the gas for legitimate callers, as the compiler will not include checks for whether a payment was provided.

The extra opcodes avoided are:

`CALLVALUE(2), DUP1(3), ISZERO(3), PUSH2(3), JUMPI(10), PUSH1(3), DUP1(3), REVERT(0), JUMPDEST(1), POP(2)`

which cost an average of about 21 gas per call to the function, in addition to the extra deployment cost.

*There are 2 instances of this issue.*


```solidity
File: src/CreateOfferer.sol

52: 		    function generateOrder(address fulfiller, SpentItem[] calldata minimumReceived, SpentItem[] calldata maximumSpent, bytes calldata context)
53: 		        external
54: 		        checkStage(Enums.Stage.generate, Enums.Stage.transfer)
55: 		        onlySeaport(msg.sender)

71: 		    function ratifyOrder(SpentItem[] calldata offer, ReceivedItem[] calldata consideration, bytes calldata context, bytes32[] calldata, uint256 contractNonce)
72: 		        external
73: 		        checkStage(Enums.Stage.ratify, Enums.Stage.generate)
74: 		        onlySeaport(msg.sender)
```
[[52-55](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L52-L55), [71-74](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L71-L74)]


---

### [G-10] Array `length` is not cached

Solidity compiler reads array length every iteration if not cached. Storage array requires an extra sload operation (100 gas), memory array requires an extra mload operation (3 gas).

*There are 2 instances of this issue.*


```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

35: 		            for (uint256 i = 0; i < data.length; ++i) {

275: 		            for (uint256 i = 0; i < hashes.length; ++i) {
```
[[35](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L35), [275](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L275)]


---

### [G-11] Usage of `uints`/`ints` smaller than 32 bytes (256 bits) incurs overhead

Citing the [documentation](https://docs.soliditylang.org/en/latest/internals/layout_in_storage.html):

> When using elements that are smaller than 32 bytes, your contract’s gas usage may be higher.This is because the EVM operates on 32 bytes at a time.Therefore, if the element is smaller than that, the EVM must use more operations in order to reduce the size of the element from 32 bytes to the desired size.

For example, each operation involving a `uint8` costs an extra ** 22 - 28 gas ** (depending on whether the other operand is also a variable of type `uint8`) as compared to ones involving`uint256`, due to the compiler having to clear the higher bits of the memory word before operating on the`uint8`, as well as the associated stack operations of doing so.

Note that it might be beneficial to use reduced-size types when dealing with storage values because the compiler will pack multiple elements into one storage slot, but if not, it will have the opposite effect.

*There is 1 instance of this issue.*


```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

38: 		        uint96 expiry = uint96(delegateTokenInfo[delegateTokenId][PACKED_INFO_POSITION]);
```
[[38](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L38)]


---

### [G-12] Using pre instead of post increments/decrements

Pre increments/decrements (`++i/--i`) are cheaper than post increments/decrements (`i++/i--`): it saves 6 gas per expression.

*There are 2 instances of this issue.*


```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

389: 		                filteredHashes[count++] = hash;

420: 		                filteredHashes[count++] = hash;
```
[[389](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L389), [420](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L420)]


---

### [G-13] `>=`/`<=` costs less gas than `>`/`<`

The compiler uses opcodes `GT` and `ISZERO` for code that uses `>`, but only requires `LT` for `>=`. A similar behaviour applies for `>`, which uses opcodes `LT` and `ISZERO`, but only requires `GT` for `<=`.

*There are 14 instances of this issue.*

<details>
<summary>Expand findings</summary>


```solidity
File: src/DelegateToken.sol

341: 		        if (StorageHelpers.readExpiry(delegateTokenInfo, delegateTokenId) < block.timestamp) {
```
[[341](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L341)]



```solidity
File: src/libraries/DelegateTokenLib.sol

109: 		        if (expiry > block.timestamp) return;
```
[[109](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L109)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

159: 		        if (info.amount > availableAmount) revert Errors.ERC20FlashAmountUnavailable();

168: 		        if (info.amount > availableAmount) {
```
[[159](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L159), [168](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L168)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

45: 		        if (expiry > MAX_EXPIRY) revert Errors.ExpiryTooLarge();

162: 		        if (block.timestamp < readExpiry(delegateTokenInfo, delegateTokenId)) {
```
[[45](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L45), [162](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L162)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

52: 		        if (IERC20(underlyingContract).allowance(msg.sender, address(this)) < underlyingAmount) {
```
[[52](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L52)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

35: 		            for (uint256 i = 0; i < data.length; ++i) {

275: 		            for (uint256 i = 0; i < hashes.length; ++i) {

312: 		            for (uint256 i = 0; i < length; ++i) {

386: 		            for (uint256 i = 0; i < hashesLength; ++i) {

393: 		            for (uint256 i = 0; i < count; ++i) {

417: 		            for (uint256 i = 0; i < hashesLength; ++i) {

423: 		            for (uint256 i = 0; i < count; ++i) {
```
[[35](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L35), [275](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L275), [312](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L312), [386](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L386), [393](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L393), [417](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L417), [423](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L423)]

</details>

---

### [G-14] `internal/private` functions only called once can be inlined to save gas

Consider removing those internal functions and to put the logic directly where they are called, as they are called only once.

*There are 7 instances of this issue.*


```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

31: 		    function checkERC721BeforePull(uint256 underlyingAmount, address underlyingContract, uint256 underlyingTokenId) internal view {

40: 		    function pullERC721AfterCheck(address underlyingContract, uint256 underlyingTokenId) internal {

45: 		    function checkERC20BeforePull(uint256 underlyingAmount, address underlyingContract, uint256 underlyingTokenId) internal view {

57: 		    function pullERC20AfterCheck(address underlyingContract, uint256 pullAmount) internal {

61: 		    function checkERC1155BeforePull(Structs.Uint256 storage erc1155Pulled, uint256 pullAmount) internal {

70: 		    function pullERC1155AfterCheck(Structs.Uint256 storage erc1155Pulled, uint256 pullAmount, address underlyingContract, uint256 underlyingTokenId) internal {

77: 		    function checkERC1155Pulled(Structs.Uint256 storage erc1155Pulled, address operator) internal returns (bool) {
```
[[31](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L31), [40](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L40), [45](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L45), [57](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L57), [61](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L61), [70](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L70), [77](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L77)]


---

### [G-15] Function names can be optimized

Function that are `public`/`external` and `public` state variable names can be optimized to save gas.

Method IDs that have two leading zero bytes can save **128 gas** each during deployment, and renaming functions to have lower method IDs will save **22 gas** per call, per sorted position shifted. [Reference](https://blog.emn178.cc/en/post/solidity-gas-optimization-function-name/)

*There are 4 instances of this issue.*


```solidity
File: src/CreateOfferer.sol

23: 		contract CreateOfferer is Modifiers, ContractOffererInterface, ERC1155Holder {
```
[[23](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L23)]



```solidity
File: src/DelegateToken.sol

15: 		contract DelegateToken is ReentrancyGuard, IDelegateToken {
```
[[15](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L15)]



```solidity
File: src/PrincipalToken.sol

11: 		contract PrincipalToken is ERC721("PrincipalToken", "PT") {
```
[[11](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L11)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

16: 		contract DelegateRegistry is IDelegateRegistry {
```
[[16](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L16)]


---

### [G-16] Using `delete` instead of setting mapping/struct to 0 saves gas

Avoid an assignment by deleting the value instead of setting it to zero, as it's [cheaper](https://gist.github.com/DadeKuma/ea874815202fc77e9d81f81a047c1e5e).

*There are 2 instances of this issue.*


```solidity
File: src/DelegateToken.sol

273: 		        if (delegateInfo.tokenType == IDelegateRegistry.DelegationType.ERC20) delegateInfo.tokenId = 0;

275: 		        if (delegateInfo.tokenType == IDelegateRegistry.DelegationType.ERC721) delegateInfo.amount = 0;
```
[[273](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L273), [275](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L275)]


---

### [G-17] Use a more recent version of Solidity

v0.8.2 has a simple compiler automatic inlining

v0.8.3 has a better struct packing and cheaper multiple storage reads

v0.8.4 has custom errors, which are cheaper at deployment than revert/require strings

v0.8.10 has external calls skip contract existence checks if the external call has a return value

*There are 5 instances of this issue.*


```solidity
File: src/libraries/CreateOffererLib.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L2)]



```solidity
File: src/libraries/DelegateTokenLib.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L2)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L2)]



```solidity
File: src/libraries/DelegateTokenStorageHelpers.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenStorageHelpers.sol#L2)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

2: 		pragma solidity ^0.8.4;
```
[[2](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L2)]


---

### [G-18] Constructors can be marked `payable`

`payable` functions cost less gas to execute, since the compiler does not have to add extra checks to ensure that a payment wasn't provided.

A `constructor` can safely be marked as `payable`, since only the deployer would be able to pass funds, and the project itself would not pass any funds.

*There are 4 instances of this issue.*


```solidity
File: src/CreateOfferer.sol

29: 		    constructor(Structs.Parameters memory parameters) Modifiers(parameters.seaport, Enums.Stage.generate) {
```
[[29](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L29)]



```solidity
File: src/DelegateToken.sol

52: 		    constructor(Structs.DelegateTokenParameters memory parameters) {
```
[[52](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L52)]



```solidity
File: src/PrincipalToken.sol

20: 		    constructor(address setDelegateToken, address setMarketMetadata) {
```
[[20](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L20)]



```solidity
File: src/libraries/CreateOffererLib.sol

145: 		    constructor(address setSeaport, CreateOffererEnums.Stage firstStage) {
```
[[145](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L145)]


---

### [G-19] Nesting `if` statements that use `&&` saves gas

Using the `&&` operator on a single `if` [costs more gas](https://gist.github.com/DadeKuma/931ce6794a050201ec6544dbcc31316c) than using two nested `if`.

*There are 4 instances of this issue.*


```solidity
File: src/libraries/CreateOffererLib.sol

355: 		        if (maximumSpent[0].itemType != ItemType.ERC721 && maximumSpent[0].itemType != ItemType.ERC20 && maximumSpent[0].itemType != ItemType.ERC1155) {
```
[[355](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L355)]



```solidity
File: src/libraries/DelegateTokenRegistryHelpers.sol

185: 		            IDelegateRegistry(delegateRegistry).delegateERC721(from, underlyingContract, underlyingTokenId, underlyingRights, false) == registryHash
186: 		                && IDelegateRegistry(delegateRegistry).delegateERC721(to, underlyingContract, underlyingTokenId, underlyingRights, true) == newRegistryHash

205: 		            IDelegateRegistry(delegateRegistry).delegateERC20(
206: 		                from, underlyingContract, underlyingRights, calculateDecreasedAmount(delegateRegistry, registryHash, underlyingAmount)
207: 		            ) == bytes32(registryHash)
208: 		                && IDelegateRegistry(delegateRegistry).delegateERC20(
209: 		                    to, underlyingContract, underlyingRights, calculateIncreasedAmount(delegateRegistry, newRegistryHash, underlyingAmount)
210: 		                ) == newRegistryHash
```
[[185-186](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L185-L186), [205-210](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenRegistryHelpers.sol#L205-L210)]



```solidity
File: src/libraries/DelegateTokenTransferHelpers.sol

78: 		        if (erc1155Pulled.flag == ERC1155_PULLED && address(this) == operator) {
```
[[78](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenTransferHelpers.sol#L78)]


---

### [G-20] Lack of `unchecked` in loops

Use `unchecked` to increment the loop variable as it can save gas:

```solidity
for(uint256 i; i < length;) {
	unchecked{
		++i;
	}
}
```

*There are 7 instances of this issue.*


```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

35: 		            for (uint256 i = 0; i < data.length; ++i) {

275: 		            for (uint256 i = 0; i < hashes.length; ++i) {

312: 		            for (uint256 i = 0; i < length; ++i) {

386: 		            for (uint256 i = 0; i < hashesLength; ++i) {

393: 		            for (uint256 i = 0; i < count; ++i) {

417: 		            for (uint256 i = 0; i < hashesLength; ++i) {

423: 		            for (uint256 i = 0; i < count; ++i) {
```
[[35](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L35), [275](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L275), [312](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L312), [386](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L386), [393](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L393), [417](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L417), [423](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L423)]


---

### [G-21] Use assembly to check for `address(0)`

A simple zero address check can be written in assembly to save some gas.

*There are 12 instances of this issue.*


```solidity
File: src/CreateOfferer.sol

30: 		        if (parameters.delegateToken == address(0)) revert Errors.DelegateTokenIsZero();

32: 		        if (parameters.principalToken == address(0)) revert Errors.PrincipalTokenIsZero();
```
[[30](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L30), [32](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L32)]



```solidity
File: src/DelegateToken.sol

53: 		        if (parameters.delegateRegistry == address(0)) revert Errors.DelegateRegistryZero();

54: 		        if (parameters.principalToken == address(0)) revert Errors.PrincipalTokenZero();

55: 		        if (parameters.marketMetadata == address(0)) revert Errors.MarketMetadataZero();

100: 		        if (delegateTokenHolder == address(0)) revert Errors.DelegateTokenHolderZero();

107: 		        if (delegateTokenHolder == address(0)) revert Errors.DelegateTokenHolderZero();

162: 		        if (to == address(0)) revert Errors.ToIsZero();

299: 		        if (delegateInfo.delegateHolder == address(0)) revert Errors.ToIsZero();
```
[[53](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L53), [54](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L54), [55](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L55), [100](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L100), [107](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L107), [162](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L162), [299](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L299)]



```solidity
File: src/PrincipalToken.sol

21: 		        if (setDelegateToken == address(0)) revert DelegateTokenZero();

23: 		        if (setMarketMetadata == address(0)) revert MarketMetadataZero();
```
[[21](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L21), [23](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L23)]



```solidity
File: src/libraries/CreateOffererLib.sol

146: 		        if (setSeaport == address(0)) revert CreateOffererErrors.SeaportIsZero();
```
[[146](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L146)]


---

### [G-22] Use assembly to write hashes

Considering using [assembly](https://medium.com/@kalexotsu/understanding-solidity-assembly-hashing-a-string-from-calldata-fbd2ece82263) to write hashes, as it's possible to save a considerable amount of gas.

*There are 4 instances of this issue.*


```solidity
File: src/libraries/CreateOffererLib.sol

301: 		            keccak256(
302: 		                abi.encode(
303: 		                    IDelegateTokenStructs.DelegateInfo({
304: 		                        tokenType: tokenType,
305: 		                        principalHolder: decodedContext.targetToken == CreateOffererEnums.TargetToken.principal ? receivers.targetTokenReceiver : receivers.fulfiller,
306: 		                        delegateHolder: decodedContext.targetToken == CreateOffererEnums.TargetToken.delegate ? receivers.targetTokenReceiver : receivers.fulfiller,
307: 		                        expiry: CreateOffererHelpers.calculateExpiry(decodedContext.expiryType, decodedContext.expiryLength),
308: 		                        rights: decodedContext.rights,
309: 		                        tokenContract: consideration.token,
310: 		                        tokenId: (tokenType != IDelegateRegistry.DelegationType.ERC20) ? consideration.identifier : 0,
311: 		                        amount: (tokenType != IDelegateRegistry.DelegationType.ERC721) ? consideration.amount : 0
312: 		                    })
313: 		                )
314: 		            ) != keccak256(abi.encode(IDelegateToken(delegateToken).getDelegateInfo(DelegateTokenHelpers.delegateIdNoRevert(address(this), identifier))))

314: 		            ) != keccak256(abi.encode(IDelegateToken(delegateToken).getDelegateInfo(DelegateTokenHelpers.delegateIdNoRevert(address(this), identifier))))

398: 		        uint256 hashWithoutType = uint256(keccak256(abi.encode(targetTokenReceiver, conduit, createOrderInfo)));
```
[[301-314](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L301-L314), [314](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L314), [398](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L398)]



```solidity
File: src/libraries/DelegateTokenLib.sol

114: 		        return uint256(keccak256(abi.encode(caller, salt)));
```
[[114](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/DelegateTokenLib.sol#L114)]


---

### [G-23] Use assembly to write `address` storage values

Using assembly `{ sstore(state.slot, addr)` instead of `state = addr` can save gas.

*There are 8 instances of this issue.*


```solidity
File: src/CreateOfferer.sol

31: 		        delegateToken = parameters.delegateToken;

33: 		        principalToken = parameters.principalToken;
```
[[31](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L31), [33](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/CreateOfferer.sol#L33)]



```solidity
File: src/DelegateToken.sol

56: 		        delegateRegistry = parameters.delegateRegistry;

57: 		        principalToken = parameters.principalToken;

58: 		        marketMetadata = parameters.marketMetadata;
```
[[56](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L56), [57](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L57), [58](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L58)]



```solidity
File: src/PrincipalToken.sol

22: 		        delegateToken = setDelegateToken;

24: 		        marketMetadata = setMarketMetadata;
```
[[22](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L22), [24](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/PrincipalToken.sol#L24)]



```solidity
File: src/libraries/CreateOffererLib.sol

147: 		        seaport = setSeaport;
```
[[147](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/libraries/CreateOffererLib.sol#L147)]


---

### [G-24] Use assembly to emit an `event`

To efficiently emit events, it's possible to utilize assembly by making use of scratch space and the free memory pointer. This approach has the advantage of potentially avoiding the costs associated with memory expansion.

However, it's important to note that in order to safely optimize this process, it is preferable to cache and restore the free memory pointer.

A good example of such practice can be seen in [Solady's](https://github.com/Vectorized/solady/blob/main/src/tokens/ERC1155.sol#L167) codebase.

*There are 11 instances of this issue.*


```solidity
File: src/DelegateToken.sol

140: 		        emit Approval(delegateTokenHolder, spender, delegateTokenId);

146: 		        emit ApprovalForAll(msg.sender, operator, approved);

172: 		        emit Transfer(from, to, delegateTokenId);

304: 		        emit Transfer(address(0), delegateInfo.delegateHolder, delegateTokenId);

332: 		            emit ExpiryExtended(delegateTokenId, previousExpiry, newExpiry);

362: 		        emit Transfer(delegateTokenHolder, address(0), delegateTokenId);
```
[[140](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L140), [146](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L146), [172](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L172), [304](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L304), [332](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L332), [362](https://github.com/code-423n4/2023-09-delegate/blob/87dda32e96e5249e51bcd1b5dd53361d7c794694/src/DelegateToken.sol#L362)]



```solidity
File: lib/delegate-registry/src/DelegateRegistry.sol

59: 		        emit DelegateAll(msg.sender, to, rights, enable);

78: 		        emit DelegateContract(msg.sender, to, contract_, rights, enable);

98: 		        emit DelegateERC721(msg.sender, to, contract_, tokenId, rights, enable);

122: 		        emit DelegateERC20(msg.sender, to, contract_, rights, amount);

147: 		        emit DelegateERC1155(msg.sender, to, contract_, tokenId, rights, amount);
```
[[59](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L59), [78](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L78), [98](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L98), [122](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L122), [147](https://github.com/delegatexyz/delegate-registry/blob/6d1254de793ccc40134f9bec0b7cb3d9c3632bc1/src/DelegateRegistry.sol#L147)]


---
