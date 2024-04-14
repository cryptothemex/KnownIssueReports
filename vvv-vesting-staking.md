CryptoThemeX-CTX

## Summary

| |Issue|Instances| Gas Savings
|-|:-|:-:|:-:|
| [[L-01](#l-01)] | `fallback` or `receive` do not exist | 1| 0|
| [[L-02](#l-02)] | Function calls within loops | 2| 0|
| [[L-03](#l-03)] | Loops in external functions should be avoided due to high gas costs and possible DOS | 2| 0|
| [[L-04](#l-04)] | Possible length difference of two array parameters | 1| 0|
| [[L-05](#l-05)] | External calls in `modifier` | 1| 0|
| [[L-06](#l-06)] | Upgradable contracts not taken into account when making wrapped calls | 3| 0|
| [[L-07](#l-07)] | Functions that send Ether to arbitrary destinations | 1| 0|
| [[L-08](#l-08)] | Complex Computation - Multiplication on result of a Division | 1| 0|
| [[L-09](#l-09)] | Dangerous strict equalities | 1| 0|
| [[L-10](#l-10)] | Local variable shadowing | 1| 0|
| [[L-11](#l-11)] | Missing inheritance | 1| 0|
| [[L-12](#l-12)] | Reentrancy vulnerabilities (events) | 3| 0|
| [[L-13](#l-13)] | Block timestamp | 4| 0|
| [[L-14](#l-14)] | Uninitialized local variables | 1| 0|
| [[L-15](#l-15)] | Centralization Risk for trusted owners | 1| 0|
| [[L-16](#l-16)] | Some tokens may revert when zero value transfers are made | 2| 0|
| [[L-17](#l-17)] | Division by zero not prevented | 2| 0|
| [[L-18](#l-18)] | External call recipient may consume all transaction gas | 2| 0|
| [[L-19](#l-19)] | Prevent accidentally minting/ burning tokens | 2| 0|
| [[L-20](#l-20)] | Solidity version 0.8.20+ may not work on other chains due to `PUSH0` | 4| 0|
| [[L-21](#l-21)] | Consider using OpenZeppelin's SafeCast library to prevent unexpected overflows when downcasting | 2| 0|
| [[G-01](#g-01)] | Multiple accesses of a mapping/array should use a local variable cache | 1| 0|
| [[G-02](#g-02)] | Constructors can be marked `payable` | 5| 0|
| [[G-03](#g-03)] | Use assembly to emit events | 9| 0|
| [[G-04](#g-04)] | emitting events with struct/ state variables consume more gas | 1| 0|
| [[G-05](#g-05)] | emit event in setter function only if the state variable was changed | 1| 0|
| [[G-06](#g-06)] | Functions guaranteed to revert when called by normal users can be marked `payable` | 1| 0|
| [[G-07](#g-07)] | if variable is casted more than once, consider caching the result to save gas | 1| 0|
| [[G-08](#g-08)] | Avoid updating storage when the value hasn't changed | 5| 0|
| [[G-09](#g-09)] | State variable read in a loop | 1| 0|
| [[G-10](#g-10)] | State variable written in a loop | 1| 0|
| [[G-11](#g-11)] | Mappings are cheaper to use than storage arrays | 2| 0|
| [[G-12](#g-12)] | `public` functions not called internally should be declared `external` to save gas | 1| 0|
| [[G-13](#g-13)] | checks for zero uint should be done using assembly to save gas | 7| 210|
| [[G-14](#g-14)] | Use assembly hashing | 1| 0|
| [[G-15](#g-15)] | Counting down in for statements is more gas efficient | 3| 90|
| [[G-16](#g-16)] | Low level call can be optimized with assembly | 2| 0|
| [[G-17](#g-17)] | `a = a + b` is more gas effective than `a += b` for state variables (excluding arrays and mappings) | 3| 48|
| [[G-18](#g-18)] | Use assembly to check for zero address | 2| 12|
| [[G-19](#g-19)] | Using bools for storage incurs overhead | 1| 100|
| [[G-20](#g-20)] | Cache array length outside of loop | 3| 0|
| [[G-21](#g-21)] | Use calldata instead of memory for function arguments that do not get mutated | 3| 180|
| [[G-22](#g-22)] | State variables only set in the constructor should be declared `immutable` | 1| 0|
| [[G-23](#g-23)] | Functions guaranteed to revert when called by normal users can be marked `payable` | 6| 0|
| [[G-24](#g-24)] | Using `private` rather than `public`, saves gas | 11| 0|
| [[G-25](#g-25)] | Increments/decrements can be `unchecked` in for-loops | 3| 90|
| [[N-01](#n-01)] | Consider providing a ranged getter for array state variables | 2| 0|
| [[N-02](#n-02)] | Consider emitting an event at the end of the constructor | 5| 0|
| [[N-03](#n-03)] | Events are missing sender information | 4| 0|
| [[N-04](#n-04)] | Validate user inputs | 11| 0|
| [[N-05](#n-05)] | Different pragma directives are used | 5| 0|
| [[N-06](#n-06)] | Low-level calls | 2| 0|
| [[N-07](#n-07)] | Conformance to Solidity naming conventions | 42| 0|
| [[N-08](#n-08)] | Array is `push()`ed | 2| 0|
| [[N-09](#n-09)] | Contract timekeeping will break earlier than the Ethereum network itself will stop working | 2| 0|
| [[N-10](#n-10)] | Getting a bool return value does not confirm the existence of a function in an external call | 2| 0|
| [[N-11](#n-11)] | Consider splitting complex checks into multiple steps | 1| 0|
| [[N-12](#n-12)] | Constant decimal values | 1| 0|
| [[N-13](#n-13)] | Constants in comparisons should appear on the left side | 7| 0|
| [[N-14](#n-14)] | use `AccessControlDefaultAdminRules` rather than `AccessControl` | 1| 0|
| [[N-15](#n-15)] | Consider adding emergency-stop functionality | 1| 0|
| [[N-16](#n-16)] | Consider making contracts `Upgradeable` | 1| 0|
| [[N-17](#n-17)] | Consider using descriptive `constant`s when passing zero as a function argument | 3| 0|
| [[N-18](#n-18)] | Using abi.encodePacked can in hash function | 1| 0|
| [[N-19](#n-19)] | Consider using a `struct` rather than having many function input parameters | 6| 0|
| [[N-20](#n-20)] | Consider using named function arguments | 1| 0|
| [[N-21](#n-21)] | Consider using named returns | 11| 0|
| [[N-22](#n-22)] | Use `string.concat()` or `bytes.concat()` instead of `abi.encodePacked` | 1| 0|
| [[N-23](#n-23)] | `constant`s should be defined rather than using magic numbers | 11| 0|
| [[N-24](#n-24)] | Control structures do not follow the Solidity Style Guide | 30| 0|
| [[N-25](#n-25)] | Events should use parameters to convey information | 1| 0|
| [[N-26](#n-26)] | Events that mark critical parameter changes should contain both the old and the new value | 1| 0|
| [[N-27](#n-27)] | Function ordering does not follow the Solidity style guide | 2| 0|
| [[N-28](#n-28)] | Change `int` to `int256` | 1| 0|
| [[N-29](#n-29)] | Interfaces should be defined in separate files from their usage | 1| 0|
| [[N-30](#n-30)] | Lack of checks in setters | 5| 0|
| [[N-31](#n-31)] | Lines are too long | 2| 0|
| [[N-32](#n-32)] | Missing Event for critical parameters change | 5| 0|
| [[N-33](#n-33)] | NatSpec is completely non-existent on functions that should have them | 1| 0|
| [[N-34](#n-34)] | Incomplete NatSpec: `@param` is missing on actually documented functions | 4| 0|
| [[N-35](#n-35)] | Incomplete NatSpec: `@return` is missing on actually documented functions | 1| 0|
| [[N-36](#n-36)] | Use a `modifier` instead of a `require/if` statement for a special `msg.sender` actor | 1| 0|
| [[N-37](#n-37)] | Consider using named mappings | 7| 0|
| [[N-38](#n-38)] | Take advantage of Custom Error's return value property | 15| 0|
| [[N-39](#n-39)] | Contract does not follow the Solidity style guide's suggested layout ordering | 3| 0|
| [[N-40](#n-40)] | Event is missing `indexed` on some of the fields | 6| 0|
| [[N-41](#n-41)] | Variables need not be initialized to zero | 3| 0|
| [[N-42](#n-42)] | Use scratch space when building emitted events with two data arguments | 2| 30|
| [[N-43](#n-43)] | Use `do`-`while` loop | 3| 0|
| [[N-44](#n-44)] | `>=` costs less gas than `>` | 9| 27|
| [[N-45](#n-45)] | Accessing Multi-Dimensional Array | 8| 0|
