CryptoThemeX-CTX

## Summary

| |Issue|Instances| Gas Savings
|-|:-|:-:|:-:|
| [[M-01](#m-01)] | Lack of EIP-712 compliance: using `keccak256()` directly on an array or struct variable | 1| 0|
| [[M-02](#m-02)] | Solady's SafeTransferLib does not check for token contract's existence | 1| 0|
| [[L-01](#l-01)] | `fallback` or `receive` do not exist | 1| 0|
| [[L-02](#l-02)] | `addresses` shouldn't be hard-coded | 1| 0|
| [[L-03](#l-03)] | Function calls within loops | 1| 0|
| [[L-04](#l-04)] | Functions that send Ether to arbitrary destinations | 1| 0|
| [[L-05](#l-05)] | Missing zero address validation | 1| 0|
| [[L-06](#l-06)] | External calls inside a loop | 1| 0|
| [[L-07](#l-07)] | Block timestamp | 1| 0|
| [[L-08](#l-08)] | Centralization Risk for trusted owners | 16| 0|
| [[L-09](#l-09)] | Use a 2-step ownership transfer pattern | 2| 0|
| [[L-10](#l-10)] | Missing checks for zero address when assigning values to address state variables | 1| 0|
| [[L-11](#l-11)] | `abi.encodePacked()` should not be used with dynamic types | 2| 0|
| [[L-12](#l-12)] | Do not leave an implementation contract uninitialized | 1| 0|
| [[L-13](#l-13)] | `domainSeparator()` isn't protected against replay attacks in case of a future chain split  | 2| 0|
| [[L-14](#l-14)] | Empty `receive()/payable fallback()` function does not authenticate requests | 1| 0|
| [[L-15](#l-15)] | External call recipient may consume all transaction gas | 2| 0|
| [[L-16](#l-16)] | Initializers could be front-run | 2| 0|
| [[L-17](#l-17)] | Solidity version 0.8.20+ may not work on other chains due to `PUSH0` | 6| 0|
| [[L-18](#l-18)] | Use `Ownable2Step.transferOwnership` instead of `Ownable.transferOwnership` | 2| 0|
| [[L-19](#l-19)] | File allows a version of solidity that is susceptible to an assembly optimizer bug | 3| 0|
| [[L-20](#l-20)] | Unspecific compiler version pragma | 1| 0|
| [[L-21](#l-21)] | Upgradeable contract is missing a `__gap[50]` storage variable to allow for new storage variables in later versions | 4| 0|
| [[L-22](#l-22)] | Upgradeable contract not initialized | 12| 0|
| [[G-01](#g-01)] | `abi.encode()` is less efficient than `abi.encodepacked()` for non-address arguments | 6| 0|
| [[G-02](#g-02)] | Cache address(this) when used more than once | 1| 0|
| [[G-03](#g-03)] | Multiple accesses of a mapping/array should use a local variable cache | 4| 0|
| [[G-04](#g-04)] | Constructors can be marked `payable` | 2| 0|
| [[G-05](#g-05)] | Division which can not overflow | 1| 0|
| [[G-06](#g-06)] | Use assembly to emit events | 3| 0|
| [[G-07](#g-07)] | Use nested if to save gas | 6| 0|
| [[G-08](#g-08)] | Functions guaranteed to revert when called by normal users can be marked `payable` | 2| 0|
| [[G-09](#g-09)] | Solidity versions 0.8.19 and above are more gas efficient | 4| 0|
| [[G-10](#g-10)] | Unnecessary casting as variable is already of the same type | 1| 0|
| [[G-11](#g-11)] | Comparing to a Boolean constant | 1| 0|
| [[G-12](#g-12)] | `public` functions not called internally should be declared `external` to save gas | 1| 0|
| [[G-13](#g-13)] | checks for zero uint should be done using assembly to save gas | 10| 300|
| [[G-14](#g-14)] | Use assembly hashing | 12| 0|
| [[G-15](#g-15)] | Counting down in for statements is more gas efficient | 1| 30|
| [[G-16](#g-16)] | Low level call can be optimized with assembly | 1| 0|
| [[G-17](#g-17)] | `a = a + b` is more gas effective than `a += b` for state variables (excluding arrays and mappings) | 1| 16|
| [[G-18](#g-18)] | Use assembly to check for zero address | 2| 12|
| [[G-19](#g-19)] | Using bools for storage incurs overhead | 2| 200|
| [[G-20](#g-20)] | Cache array length outside of loop | 2| 0|
| [[G-21](#g-21)] | Use calldata instead of memory for function arguments that do not get mutated | 4| 240|
| [[G-22](#g-22)] | Use Custom Errors instead of Revert Strings to save Gas | 4| 200|
| [[G-23](#g-23)] | State variables only set in the constructor should be declared `immutable` | 1| 0|
| [[G-24](#g-24)] | Functions guaranteed to revert when called by normal users can be marked `payable` | 6| 0|
| [[G-25](#g-25)] | `++i` costs less gas compared to `i++` or `i += 1` (same for `--i` vs `i--` or `i -= 1`) | 2| 10|
| [[G-26](#g-26)] | Using `private` rather than `public`, saves gas | 2| 0|
| [[G-27](#g-27)] | Use shift right/left instead of division/multiplication if possible | 1| 0|
| [[G-28](#g-28)] | Increments/decrements can be `unchecked` in for-loops | 1| 30|
| [[G-29](#g-29)] | Use `!= 0` instead of `> 0` for unsigned integer comparison | 2| 8|
| [[G-30](#g-30)] | `internal` functions not called by the contract should be removed | 2| 0|
| [[N-01](#n-01)] | Consider emitting an event at the end of the constructor | 3| 0|
| [[N-02](#n-02)] | Events are missing sender information | 3| 0|
| [[N-03](#n-03)] | Validate user inputs | 18| 0|
| [[N-04](#n-04)] | Return bool explicitly | 3| 0|
| [[N-05](#n-05)] | Assembly usage | 9| 0|
| [[N-06](#n-06)] | Different pragma directives are used | 7| 0|
| [[N-07](#n-07)] | Cyclomatic complexity | 1| 0|
| [[N-08](#n-08)] | Incorrect versions of Solidity | 1| 0|
| [[N-09](#n-09)] | Low-level calls | 2| 0|
| [[N-10](#n-10)] | Conformance to Solidity naming conventions | 24| 0|
| [[N-11](#n-11)] | Variable names too similar | 1| 0|
| [[N-12](#n-12)] | Too many digits | 5| 0|
| [[N-13](#n-13)] | Unused state variable | 1| 0|
| [[N-14](#n-14)] | Getting a bool return value does not confirm the existence of a function in an external call | 2| 0|
| [[N-15](#n-15)] | Consider splitting complex checks into multiple steps | 3| 0|
| [[N-16](#n-16)] | Constant decimal values | 1| 0|
| [[N-17](#n-17)] | Constants in comparisons should appear on the left side | 21| 0|
| [[N-18](#n-18)] | Consider adding emergency-stop functionality | 3| 0|
| [[N-19](#n-19)] | Consider making contracts `Upgradeable` | 3| 0|
| [[N-20](#n-20)] | Consider using descriptive `constant`s when passing zero as a function argument | 32| 0|
| [[N-21](#n-21)] | Using abi.encodePacked can in hash function | 1| 0|
| [[N-22](#n-22)] | Use of `override` is unnecessary | 3| 0|
| [[N-23](#n-23)] | Consider using a `struct` rather than having many function input parameters | 14| 0|
| [[N-24](#n-24)] | Consider using named function arguments | 9| 0|
| [[N-25](#n-25)] | Consider using named returns | 20| 0|
| [[N-26](#n-26)] | Returning a struct instead of returning many variables is better | 7| 0|
| [[N-27](#n-27)] | Use SafeTransferLib.safeTransferETH() or Address.sendValue() | 1| 0|
| [[N-28](#n-28)] | Array indices should be referenced via `enum`s rather than via numeric literals | 3| 0|
| [[N-29](#n-29)] | `require()` should be used instead of `assert()` | 1| 0|
| [[N-30](#n-30)] | Use `string.concat()` or `bytes.concat()` instead of `abi.encodePacked` | 2| 0|
| [[N-31](#n-31)] | Constants should be in CONSTANT_CASE | 9| 0|
| [[N-32](#n-32)] | `constant`s should be defined rather than using magic numbers | 15| 0|
| [[N-33](#n-33)] | Control structures do not follow the Solidity Style Guide | 18| 0|
| [[N-34](#n-34)] | Default Visibility for constants | 10| 0|
| [[N-35](#n-35)] | Consider disabling `renounceOwnership()` | 2| 0|
| [[N-36](#n-36)] | Unused `error` definition | 1| 0|
| [[N-37](#n-37)] | Function ordering does not follow the Solidity style guide | 2| 0|
| [[N-38](#n-38)] | Change `int` to `int256` | 2| 0|
| [[N-39](#n-39)] | File's first line is not an SPDX Identifier | 1| 0|
| [[N-40](#n-40)] | Use a `modifier` instead of a `require/if` statement for a special `msg.sender` actor | 5| 0|
| [[N-41](#n-41)] | Adding a `return` statement when the function defines a named return variable, is redundant | 11| 0|
| [[N-42](#n-42)] | Take advantage of Custom Error's return value property | 9| 0|
| [[N-43](#n-43)] | Strings should use double quotes rather than single quotes | 2| 0|
| [[N-44](#n-44)] | Contract does not follow the Solidity style guide's suggested layout ordering | 3| 0|
| [[N-45](#n-45)] | Use Underscores for Number Literals (add an underscore every 3 digits) | 1| 0|
| [[N-46](#n-46)] | Internal and private variables and functions names should begin with an underscore | 11| 0|
| [[N-47](#n-47)] | Event is missing `indexed` on some of the fields | 3| 0|
| [[N-48](#n-48)] | Use scratch space when building emitted events with two data arguments | 2| 30|
| [[N-49](#n-49)] | Use `do`-`while` loop | 1| 0|
| [[N-50](#n-50)] | `>=` costs less gas than `>` | 10| 30|
| [[N-51](#n-51)] | Accessing Multi-Dimensional Array | 3| 0|
