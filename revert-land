CryptoThemeX-CTX

## Summary

| |Issue|Instances| Gas Savings
|-|:-|:-:|:-:|
| [[M-01](#m-01)] | Incorrect erc721 interface | 1| 0|
| [[M-02](#m-02)] | Reentrancy vulnerabilities (theft of ethers) | 4| 0|
| [[M-03](#m-03)] | Contracts are vulnerable to fee-on-transfer accounting-related issues | 6| 0|
| [[M-04](#m-04)] | `increaseAllowance/decreaseAllowance` won't work on mainnet for USDT | 2| 0|
| [[M-05](#m-05)] | Chainlink's `latestRoundData` might return stale or incorrect results | 1| 0|
| [[M-06](#m-06)] | Missing checks for whether the L2 Sequencer is active | 1| 0|
| [[L-01](#l-01)] | Chainlink answer is not compared against min/max values | 1| 0|
| [[L-02](#l-02)] | `decimals()` is not part of the ERC20 standard | 4| 0|
| [[L-03](#l-03)] | `fallback` or `receive` do not exist | 4| 0|
| [[L-04](#l-04)] | Function calls within loops | 2| 0|
| [[L-05](#l-05)] | Loops in external functions should be avoided due to high gas costs and possible DOS | 2| 0|
| [[L-06](#l-06)] | Missing `require` check while setting min/ max values | 1| 0|
| [[L-07](#l-07)] | No limits when setting price | 1| 0|
| [[L-08](#l-08)] | Upgradable contracts not taken into account when making wrapped calls | 59| 0|
| [[L-09](#l-09)] | Unsafe `uint` to `int` conversion | 4| 0|
| [[L-10](#l-10)] | Functions that send Ether to arbitrary destinations | 2| 0|
| [[L-11](#l-11)] | Complex Computation - Multiplication on result of a Division | 1| 0|
| [[L-12](#l-12)] | Dangerous strict equalities | 2| 0|
| [[L-13](#l-13)] | Local variable shadowing | 21| 0|
| [[L-14](#l-14)] | Missing zero address validation | 7| 0|
| [[L-15](#l-15)] | Benign reentrancy vulnerabilities | 4| 0|
| [[L-16](#l-16)] | Reentrancy vulnerabilities (events) | 38| 0|
| [[L-17](#l-17)] | Reentrancy vulnerabilities (loss of non-ether assets) | 7| 0|
| [[L-18](#l-18)] | Block timestamp | 7| 0|
| [[L-19](#l-19)] | Uninitialized local variables | 15| 0|
| [[L-20](#l-20)] | Unused return | 33| 0|
| [[L-21](#l-21)] | Replace `abi.encodeWithSignature` and `abi.encodeWithSelector` with `abi.encodeCall` which keeps the code typo/type safe | 2| 0|
| [[L-22](#l-22)] | `approve()`/`safeApprove()` may revert if the current approval is not zero | 17| 0|
| [[L-23](#l-23)] | Centralization Risk for trusted owners | 18| 0|
| [[L-24](#l-24)] | Use a 2-step ownership transfer pattern | 4| 0|
| [[L-25](#l-25)] | Contracts are vulnerable to fee-on-transfer accounting-related issues | 6| 0|
| [[L-26](#l-26)] | Some tokens may revert when zero value transfers are made | 23| 0|
| [[L-27](#l-27)] | Missing checks for zero address when assigning values to address state variables | 6| 0|
| [[L-28](#l-28)] | Deprecated approve() function | 2| 0|
| [[L-29](#l-29)] | Do not use deprecated library functions | 15| 0|
| [[L-30](#l-30)] | `safeApprove()` is deprecated | 15| 0|
| [[L-31](#l-31)] | Division by zero not prevented | 49| 0|
| [[L-32](#l-32)] | External call recipient may consume all transaction gas | 5| 0|
| [[L-33](#l-33)] | Signature use at deadlines should be allowed | 1| 0|
| [[L-34](#l-34)] | Prevent accidentally minting/ burning tokens | 4| 0|
| [[L-35](#l-35)] | Loss of precision | 5| 0|
| [[L-36](#l-36)] | Solidity version 0.8.20+ may not work on other chains due to `PUSH0` | 9| 0|
| [[L-37](#l-37)] | Use `Ownable2Step.transferOwnership` instead of `Ownable.transferOwnership` | 4| 0|
| [[L-38](#l-38)] | File allows a version of solidity that is susceptible to an assembly optimizer bug | 9| 0|
| [[L-39](#l-39)] | Consider using OpenZeppelin's SafeCast library to prevent unexpected overflows when downcasting | 12| 0|
| [[L-40](#l-40)] | Unsafe ERC20 operation(s) | 2| 0|
| [[L-41](#l-41)] | Upgradeable contract not initialized | 2| 0|
| [[G-01](#g-01)] | `abi.encode()` is less efficient than `abi.encodepacked()` for non-address arguments | 2| 0|
| [[G-02](#g-02)] | Cache address(this) when used more than once | 16| 0|
| [[G-03](#g-03)] | Multiple accesses of a mapping/array should use a local variable cache | 14| 0|
| [[G-04](#g-04)] | Constructors can be marked `payable` | 11| 0|
| [[G-05](#g-05)] | Division which can not overflow | 5| 0|
| [[G-06](#g-06)] | Use assembly to emit events | 49| 0|
| [[G-07](#g-07)] | waste of GAS to emit variable literals | 3| 0|
| [[G-08](#g-08)] | emit event in setter function only if the state variable was changed | 17| 0|
| [[G-09](#g-09)] | Use nested if to save gas | 16| 0|
| [[G-10](#g-10)] | Initializing non-`constant`/non-`immutable` state variables to zero/false costs more gas | 1| 0|
| [[G-11](#g-11)] | Functions guaranteed to revert when called by normal users can be marked `payable` | 25| 0|
| [[G-12](#g-12)] | if variable is casted more than once, consider caching the result to save gas | 18| 0|
| [[G-13](#g-13)] | Avoid updating storage when the value hasn't changed | 11| 0|
| [[G-14](#g-14)] | smaller uint/int types cause gas overhead | 13| 0|
| [[G-15](#g-15)] | Solidity versions 0.8.19 and above are more gas efficient | 11| 0|
| [[G-16](#g-16)] | State variable read in a loop | 1| 0|
| [[G-17](#g-17)] | Unnecessary casting as variable is already of the same type | 2| 0|
| [[G-18](#g-18)] | Mappings are cheaper to use than storage arrays | 1| 0|
| [[G-19](#g-19)] | `public` functions not called internally should be declared `external` to save gas | 2| 0|
| [[G-20](#g-20)] | checks for zero uint should be done using assembly to save gas | 10| 300|
| [[G-21](#g-21)] | Counting down in for statements is more gas efficient | 2| 60|
| [[G-22](#g-22)] | Low level call can be optimized with assembly | 3| 0|
| [[G-23](#g-23)] | `a = a + b` is more gas effective than `a += b` for state variables (excluding arrays and mappings) | 15| 240|
| [[G-24](#g-24)] | Use assembly to check for zero address | 6| 36|
| [[G-25](#g-25)] | `array[index] += amount` is cheaper than `array[index] = array[index] + amount` (or related variants) | 2| 56|
| [[G-26](#g-26)] | Using bools for storage incurs overhead | 4| 400|
| [[G-27](#g-27)] | State variables should be cached in stack variables rather than re-reading them from storage | 1| 100|
| [[G-28](#g-28)] | Use calldata instead of memory for function arguments that do not get mutated | 2| 120|
| [[G-29](#g-29)] | Use Custom Errors instead of Revert Strings to save Gas | 3| 150|
| [[G-30](#g-30)] | Avoid contract existence checks by using low level calls | 19| 1900|
| [[G-31](#g-31)] | State variables only set in the constructor should be declared `immutable` | 18| 0|
| [[G-32](#g-32)] | Functions guaranteed to revert when called by normal users can be marked `payable` | 12| 0|
| [[G-33](#g-33)] | Using `private` rather than `public`, saves gas | 66| 0|
| [[G-34](#g-34)] | Use shift right/left instead of division/multiplication if possible | 2| 0|
| [[G-35](#g-35)] | Increments/decrements can be `unchecked` in for-loops | 2| 60|
| [[G-36](#g-36)] | Use `!= 0` instead of `> 0` for unsigned integer comparison | 51| 204|
| [[G-37](#g-37)] | WETH address definition can be use directly | 1| 0|
| [[N-01](#n-01)] | Consider providing a ranged getter for array state variables | 1| 0|
| [[N-02](#n-02)] | Consider emitting an event at the end of the constructor | 11| 0|
| [[N-03](#n-03)] | Similar Constants decalred in Multiple Contracts  | 4| 0|
| [[N-04](#n-04)] | Events are missing sender information | 33| 0|
| [[N-05](#n-05)] | Validate user inputs | 65| 0|
| [[N-06](#n-06)] | Return bool explicitly | 1| 0|
| [[N-07](#n-07)] | Cyclomatic complexity | 3| 0|
| [[N-08](#n-08)] | Low-level calls | 5| 0|
| [[N-09](#n-09)] | Conformance to Solidity naming conventions | 15| 0|
| [[N-10](#n-10)] | Variable names too similar | 23| 0|
| [[N-11](#n-11)] | Array is `push()`ed | 1| 0|
| [[N-12](#n-12)] | Getting a bool return value does not confirm the existence of a function in an external call | 5| 0|
| [[N-13](#n-13)] | Consider splitting complex checks into multiple steps | 14| 0|
| [[N-14](#n-14)] | Constants in comparisons should appear on the left side | 83| 0|
| [[N-15](#n-15)] | Consider using descriptive `constant`s when passing zero as a function argument | 37| 0|
| [[N-16](#n-16)] | Use of `override` is unnecessary | 37| 0|
| [[N-17](#n-17)] | Consider using a `struct` rather than having many function input parameters | 49| 0|
| [[N-18](#n-18)] | Import declarations should import specific identifiers, rather than the whole file | 21| 0|
| [[N-19](#n-19)] | Consider using named function arguments | 50| 0|
| [[N-20](#n-20)] | Consider using named returns | 31| 0|
| [[N-21](#n-21)] | Returning a struct instead of returning many variables is better | 30| 0|
| [[N-22](#n-22)] | Use SafeTransferLib.safeTransferETH() or Address.sendValue() | 3| 0|
| [[N-23](#n-23)] | Array indices should be referenced via `enum`s rather than via numeric literals | 7| 0|
| [[N-24](#n-24)] | `constant`s should be defined rather than using magic numbers | 8| 0|
| [[N-25](#n-25)] | Control structures do not follow the Solidity Style Guide | 65| 0|
| [[N-26](#n-26)] | Critical Changes Should Use Two-step Procedure | 2| 0|
| [[N-27](#n-27)] | Consider disabling `renounceOwnership()` | 4| 0|
| [[N-28](#n-28)] | Event missing indexed field | 20| 0|
| [[N-29](#n-29)] | Events that mark critical parameter changes should contain both the old and the new value | 17| 0|
| [[N-30](#n-30)] | Function ordering does not follow the Solidity style guide | 5| 0|
| [[N-31](#n-31)] | Longer/ Complex `function` implementation | 1| 0|
| [[N-32](#n-32)] | Lack of checks in setters | 6| 0|
| [[N-33](#n-33)] | Lines are too long | 2| 0|
| [[N-34](#n-34)] | NatSpec is completely non-existent on functions that should have them | 8| 0|
| [[N-35](#n-35)] | Incomplete NatSpec: `@param` is missing on actually documented functions | 9| 0|
| [[N-36](#n-36)] | Incomplete NatSpec: `@return` is missing on actually documented functions | 6| 0|
| [[N-37](#n-37)] | Use a `modifier` instead of a `require/if` statement for a special `msg.sender` actor | 26| 0|
| [[N-38](#n-38)] | Constant state variables defined more than once | 4| 0|
| [[N-39](#n-39)] | Consider using named mappings | 13| 0|
| [[N-40](#n-40)] | Adding a `return` statement when the function defines a named return variable, is redundant | 6| 0|
| [[N-41](#n-41)] | `require()` / `revert()` statements should have descriptive reason strings | 1| 0|
| [[N-42](#n-42)] | Take advantage of Custom Error's return value property | 102| 0|
| [[N-43](#n-43)] | Deprecated library used for Solidity `>= 0.8` : SafeMath | 1| 0|
| [[N-44](#n-44)] | Contract does not follow the Solidity style guide's suggested layout ordering | 11| 0|
| [[N-45](#n-45)] | Use Underscores for Number Literals (add an underscore every 3 digits) | 5| 0|
| [[N-46](#n-46)] | Internal and private variables and functions names should begin with an underscore | 4| 0|
| [[N-47](#n-47)] | Event is missing `indexed` on some of the fields | 38| 0|
| [[N-48](#n-48)] | Variables need not be initialized to zero | 13| 0|
| [[N-49](#n-49)] | Use scratch space when building emitted events with two data arguments | 15| 225|
| [[N-50](#n-50)] | Use `do`-`while` loop | 2| 0|
| [[N-51](#n-51)] | `>=` costs less gas than `>` | 118| 354|
| [[N-52](#n-52)] | Accessing Multi-Dimensional Array | 14| 0|
| [[N-53](#n-53)] | Avoid transferring amounts of zero in order to save gas | 12| 1200|
