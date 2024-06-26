CryptoThemeX-CTX

## Summary

| |Issue|Instances| Gas Savings
|-|:-|:-:|:-:|
| [[M-01](#m-01)] | Arbitrary `from` in transferFrom | 2| 0|
| [[M-02](#m-02)] | `block.number` means different things on different L2s | 1| 0|
| [[M-03](#m-03)] | `increaseAllowance/decreaseAllowance` won't work on mainnet for USDT | 2| 0|
| [[L-01](#l-01)] | Return values not checked for `approve()` | 2| 0|
| [[L-02](#l-02)] | int/uint passed to abi.encodePacked without casting to string | 1| 0|
| [[L-03](#l-03)] | Chainlink answer is not compared against min/max values | 2| 0|
| [[L-04](#l-04)] | `decimals()` is not part of the ERC20 standard | 4| 0|
| [[L-05](#l-05)] | Function calls within loops | 7| 0|
| [[L-06](#l-06)] | Loops in external functions should be avoided due to high gas costs and possible DOS | 6| 0|
| [[L-07](#l-07)] | Missing zero address check in initializer | 3| 0|
| [[L-08](#l-08)] | Prefer skip over revert model in loop | 1| 0|
| [[L-09](#l-09)] | Upgradable contracts not taken into account when making wrapped calls | 9| 0|
| [[L-10](#l-10)] | Complex Computation - Multiplication on result of a Division | 4| 0|
| [[L-11](#l-11)] | Dangerous strict equalities | 18| 0|
| [[L-12](#l-12)] | Local variable shadowing | 3| 0|
| [[L-13](#l-13)] | Missing events arithmetic | 1| 0|
| [[L-14](#l-14)] | Missing zero address validation | 22| 0|
| [[L-15](#l-15)] | Benign reentrancy vulnerabilities | 22| 0|
| [[L-16](#l-16)] | Reentrancy vulnerabilities (events) | 38| 0|
| [[L-17](#l-17)] | Reentrancy vulnerabilities (loss of non-ether assets) | 11| 0|
| [[L-18](#l-18)] | Block timestamp | 13| 0|
| [[L-19](#l-19)] | Unchecked transfer | 6| 0|
| [[L-20](#l-20)] | Uninitialized local variables | 28| 0|
| [[L-21](#l-21)] | Uninitialized state variables | 2| 0|
| [[L-22](#l-22)] | Unused return | 22| 0|
| [[L-23](#l-23)] | `approve()`/`safeApprove()` may revert if the current approval is not zero | 11| 0|
| [[L-24](#l-24)] | Centralization Risk for trusted owners | 34| 0|
| [[L-25](#l-25)] | Fees can be set to be greater than 100%. | 1| 0|
| [[L-26](#l-26)] | Contracts are vulnerable to fee-on-transfer accounting-related issues | 1| 0|
| [[L-27](#l-27)] | Some tokens may revert when zero value transfers are made | 4| 0|
| [[L-28](#l-28)] | Missing checks for zero address when assigning values to address state variables | 23| 0|
| [[L-29](#l-29)] | Use of `ecrecover` is susceptible to signature malleability | 2| 0|
| [[L-30](#l-30)] | `abi.encodePacked()` should not be used with dynamic types | 2| 0|
| [[L-31](#l-31)] | `decimals()` should be of type `uint8` | 2| 0|
| [[L-32](#l-32)] | Deprecated approve() function | 3| 0|
| [[L-33](#l-33)] | Do not use deprecated library functions | 2| 0|
| [[L-34](#l-34)] | `safeApprove()` is deprecated | 2| 0|
| [[L-35](#l-35)] | Division by zero not prevented | 18| 0|
| [[L-36](#l-36)] | `domainSeparator()` isn't protected against replay attacks in case of a future chain split  | 19| 0|
| [[L-37](#l-37)] | Empty `receive()/payable fallback()` function does not authenticate requests | 1| 0|
| [[L-38](#l-38)] | External call recipient may consume all transaction gas | 5| 0|
| [[L-39](#l-39)] | Signature use at deadlines should be allowed | 5| 0|
| [[L-40](#l-40)] | Prevent accidentally minting/ burning tokens | 3| 0|
| [[L-41](#l-41)] | Loss of precision | 15| 0|
| [[L-42](#l-42)] | Solidity version 0.8.20+ may not work on other chains due to `PUSH0` | 18| 0|
| [[L-43](#l-43)] | Use `Ownable2Step.transferOwnership` instead of `Ownable.transferOwnership` | 2| 0|
| [[L-44](#l-44)] | Sweeping may break accounting if tokens with multiple addresses are used | 19| 0|
| [[L-45](#l-45)] | Consider using OpenZeppelin's SafeCast library to prevent unexpected overflows when downcasting | 5| 0|
| [[L-46](#l-46)] | Unsafe ERC20 operation(s) | 15| 0|
| [[L-47](#l-47)] | Upgradeable contract not initialized | 17| 0|
| [[L-48](#l-48)] | Use of ecrecover is susceptible to signature malleability | 2| 0|
| [[G-01](#g-01)] | Inefficient use of `abi.encode()` | 3| 300|
| [[G-02](#g-02)] | Cache address(this) when used more than once | 3| 0|
| [[G-03](#g-03)] | Multiple accesses of a mapping/array should use a local variable cache | 20| 0|
| [[G-04](#g-04)] | Constructors can be marked `payable` | 19| 399|
| [[G-05](#g-05)] | Division which can not overflow | 8| 680|
| [[G-06](#g-06)] | Use assembly to emit events | 88| 3344|
| [[G-07](#g-07)] | Emitting events with struct/ state variables consume more gas | 7| 0|
| [[G-08](#g-08)] | Waste of GAS to emit variable literals | 9| 0|
| [[G-09](#g-09)] | Avoid emitting events in loops | 1| 0|
| [[G-10](#g-10)] | Emit event in setter function only if the state variable was changed | 22| 0|
| [[G-11](#g-11)] | Use nested if to save gas | 19| 0|
| [[G-12](#g-12)] | Internal or Private Function can be Inlined to Save Gas | 9| 180|
| [[G-13](#g-13)] | Using Storage Instead of Memory for structs/arrays Saves Gas | 5| 21000|
| [[G-14](#g-14)] | Modulus operations that could be unchecked | 2| 60|
| [[G-15](#g-15)] | Functions guaranteed to revert when called by normal users can be marked `payable` | 45| 0|
| [[G-16](#g-16)] | if variable is casted more than once, consider caching the result to save gas | 10| 0|
| [[G-17](#g-17)] | Inefficient Parameter Storage | 47| 2350|
| [[G-18](#g-18)] | Redundant state variable getters | 4| 0|
| [[G-19](#g-19)] | Argument validation should be at the top of the function/block | 2| 4200|
| [[G-20](#g-20)] | Split require/ assert statement | 14| 0|
| [[G-21](#g-21)] | Avoid updating storage when the value hasn't changed | 14| 11200|
| [[G-22](#g-22)] | smaller uint/int types cause gas overhead | 8| 48|
| [[G-23](#g-23)] | Use Bytes32 for small data storage | 9| 0|
| [[G-24](#g-24)] | Solidity versions 0.8.19 and above are more gas efficient | 39| 0|
| [[G-25](#g-25)] | Use assembly to write address storage values | 13| 1001|
| [[G-26](#g-26)] | State variable read in a loop | 5| 0|
| [[G-27](#g-27)] | State variable written in a loop | 1| 0|
| [[G-28](#g-28)] | Safe Subtraction Should Be Unchecked | 12| 1020|
| [[G-29](#g-29)] | Unnecessary casting as variable is already of the same type | 2| 0|
| [[G-30](#g-30)] | Mappings are cheaper to use than storage arrays | 3| 0|
| [[G-31](#g-31)] | Comparing to a Boolean constant | 1| 0|
| [[G-32](#g-32)] | State variables that could be declared constant | 10| 0|
| [[G-33](#g-33)] | `public` functions not called internally should be declared `external` to save gas | 17| 0|
| [[G-34](#g-34)] | Variables need not be initialized to zero | 17| 102|
| [[G-35](#g-35)] | Shorten the array rather than copying to a new one | 1| 0|
| [[G-36](#g-36)] | checks for zero uint should be done using assembly to save gas | 29| 870|
| [[G-37](#g-37)] | Use Assembly for Hash Calculation | 13| 1040|
| [[G-38](#g-38)] | error strings longer than 32 characters consume more gas | 109| 1962|
| [[G-39](#g-39)] | `>=` costs less gas than `>` | 123| 369|
| [[G-40](#g-40)] | Counting down in for statements is more gas efficient | 11| 330|
| [[G-41](#g-41)] | Setting struct to 0 consumes more gas | 5| 0|
| [[G-42](#g-42)] | Avoid transferring amounts of zero in order to save gas | 7| 700|
| [[G-43](#g-43)] | `a = a + b` is more gas effective than `a += b` for state variables (excluding arrays and mappings) | 4| 64|
| [[G-44](#g-44)] | Use assembly to check for zero address | 29| 1682|
| [[G-45](#g-45)] | `array[index] += amount` is cheaper than `array[index] = array[index] + amount` (or related variants) | 2| 56|
| [[G-46](#g-46)] | Using bools for storage incurs overhead | 4| 3600|
| [[G-47](#g-47)] | Cache array length outside of loop | 4| 0|
| [[G-48](#g-48)] | State variables should be cached in stack variables rather than re-reading them from storage | 3| 300|
| [[G-49](#g-49)] | Use calldata instead of memory for function arguments that do not get mutated | 6| 360|
| [[G-50](#g-50)] | Use Custom Errors instead of Revert Strings to save Gas | 100| 5000|
| [[G-51](#g-51)] | Avoid contract existence checks by using low level calls | 9| 900|
| [[G-52](#g-52)] | Stack variable used as a cheaper cache for a state variable is only used once | 1| 0|
| [[G-53](#g-53)] | State variables only set in the constructor should be declared `immutable` | 54| 0|
| [[G-54](#g-54)] | `++i` costs less gas compared to `i++` or `i += 1` (same for `--i` vs `i--` or `i -= 1`) | 13| 65|
| [[G-55](#g-55)] | Using `private` rather than `public` for constants, saves gas | 31| 105586|
| [[G-56](#g-56)] | Use shift right/left instead of division/multiplication if possible | 4| 80|
| [[G-57](#g-57)] | Superfluous event fields | 3| 0|
| [[G-58](#g-58)] | Increments/decrements can be `unchecked` in for-loops | 11| 330|
| [[G-59](#g-59)] | Use `!= 0` instead of `> 0` for unsigned integer comparison | 52| 208|
| [[G-60](#g-60)] | `internal` functions not called by the contract should be removed | 8| 0|
| [[N-01](#n-01)] | Consider providing a ranged getter for array state variables | 3| 0|
| [[N-02](#n-02)] | Consider emitting an event at the end of the constructor | 14| 0|
| [[N-03](#n-03)] | Similar Constants decalred in Multiple Contracts  | 24| 0|
| [[N-04](#n-04)] | Duplicate error strings | 5| 0|
| [[N-05](#n-05)] | Events are missing sender information | 58| 0|
| [[N-06](#n-06)] | Validate user inputs | 125| 0|
| [[N-07](#n-07)] | `msg.sender` in `require` | 10| 0|
| [[N-08](#n-08)] | Return bool explicitly | 6| 0|
| [[N-09](#n-09)] | Assembly usage | 4| 0|
| [[N-10](#n-10)] | Costly operations inside a loop | 8| 0|
| [[N-11](#n-11)] | Dead-code | 2| 0|
| [[N-12](#n-12)] | Conformance to Solidity naming conventions | 203| 0|
| [[N-13](#n-13)] | Variable names too similar | 72| 0|
| [[N-14](#n-14)] | Too many digits | 7| 0|
| [[N-15](#n-15)] | Unused state variable | 2| 0|
| [[N-16](#n-16)] | Array is `push()`ed | 1| 0|
| [[N-17](#n-17)] | Getting a bool return value does not confirm the existence of a function in an external call | 1| 0|
| [[N-18](#n-18)] | Consider splitting complex checks into multiple steps | 13| 0|
| [[N-19](#n-19)] | Constant decimal values | 8| 0|
| [[N-20](#n-20)] | Constants in comparisons should appear on the left side | 100| 0|
| [[N-21](#n-21)] | Consider adding emergency-stop functionality | 6| 0|
| [[N-22](#n-22)] | Consider making contracts `Upgradeable` | 6| 0|
| [[N-23](#n-23)] | Consider using descriptive `constant`s when passing zero as a function argument | 69| 0|
| [[N-24](#n-24)] | Using abi.encodePacked can in hash function | 3| 0|
| [[N-25](#n-25)] | Use of `override` is unnecessary | 81| 0|
| [[N-26](#n-26)] | Consider using a `struct` rather than having many function input parameters | 109| 0|
| [[N-27](#n-27)] | uint/int variables should have the bit size defined explicitly | 35| 0|
| [[N-28](#n-28)] | Consider using named function arguments | 24| 0|
| [[N-29](#n-29)] | Consider using named returns | 230| 0|
| [[N-30](#n-30)] | Returning a struct instead of returning many variables is better | 38| 0|
| [[N-31](#n-31)] | Array indices should be referenced via `enum`s rather than via numeric literals | 2| 0|
| [[N-32](#n-32)] | `require()` should be used instead of `assert()` | 1| 0|
| [[N-33](#n-33)] | Use `string.concat()` or `bytes.concat()` instead of `abi.encodePacked` | 3| 0|
| [[N-34](#n-34)] | Constants should be in CONSTANT_CASE | 1| 0|
| [[N-35](#n-35)] | `constant`s should be defined rather than using magic numbers | 18| 0|
| [[N-36](#n-36)] | Control structures do not follow the Solidity Style Guide | 54| 0|
| [[N-37](#n-37)] | Default Visibility for constants | 4| 0|
| [[N-38](#n-38)] | Duplicated `require()`/`revert()` Checks Should Be Refactored To A Modifier Or Function | 11| 0|
| [[N-39](#n-39)] | Events should use parameters to convey information | 2| 0|
| [[N-40](#n-40)] | Event missing indexed field | 29| 0|
| [[N-41](#n-41)] | Events that mark critical parameter changes should contain both the old and the new value | 22| 0|
| [[N-42](#n-42)] | Function ordering does not follow the Solidity style guide | 16| 0|
| [[N-43](#n-43)] | Longer/ Complex `function` implementation | 3| 0|
| [[N-44](#n-44)] | Change `int` to `int256` | 5| 0|
| [[N-45](#n-45)] | Change`uint` to `uint256` | 39| 0|
| [[N-46](#n-46)] | Interfaces should be defined in separate files from their usage | 2| 0|
| [[N-47](#n-47)] | Lack of checks in setters | 17| 0|
| [[N-48](#n-48)] | Missing Event for critical parameters change | 5| 0|
| [[N-49](#n-49)] | NatSpec is completely non-existent on functions that should have them | 6| 0|
| [[N-50](#n-50)] | Incomplete NatSpec: `@param` is missing on actually documented functions | 7| 0|
| [[N-51](#n-51)] | Incomplete NatSpec: `@return` is missing on actually documented functions | 6| 0|
| [[N-52](#n-52)] | Use a `modifier` instead of a `require/if` statement for a special `msg.sender` actor | 17| 0|
| [[N-53](#n-53)] | Constant state variables defined more than once | 11| 0|
| [[N-54](#n-54)] | Consider using named mappings | 14| 0|
| [[N-55](#n-55)] | Numeric values having to do with time should use time units for readability | 2| 0|
| [[N-56](#n-56)] | Adding a `return` statement when the function defines a named return variable, is redundant | 24| 0|
| [[N-57](#n-57)] | `require()` / `revert()` statements should have descriptive reason strings | 12| 0|
| [[N-58](#n-58)] | Take advantage of Custom Error's return value property | 1| 0|
| [[N-59](#n-59)] | Contract does not follow the Solidity style guide's suggested layout ordering | 11| 0|
| [[N-60](#n-60)] | Use Underscores for Number Literals (add an underscore every 3 digits) | 10| 0|
| [[N-61](#n-61)] | Internal and private variables and functions names should begin with an underscore | 15| 0|
| [[N-62](#n-62)] | Event is missing `indexed` on some of the fields | 42| 0|
| [[N-63](#n-63)] | `override` function arguments that are unused should have the variable name removed or commented out to avoid compiler warnings | 6| 0|
| [[N-64](#n-64)] | Use scratch space when building emitted events with two data arguments | 31| 465|
| [[N-65](#n-65)] | Use `do`-`while` loop | 11| 0|
| [[N-66](#n-66)] | Accessing Multi-Dimensional Array | 23| 0|
| [[N-67](#n-67)] | Check `msg.sender` using `xor` and the scratch space | 20| 420|
