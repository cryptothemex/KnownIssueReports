## Summary

| |Issue|Instances| Gas Savings
|-|:-|:-:|:-:|
| [[M-01](#m-01)] | Arbitrary `from` in transferFrom | 2| 0|
| [[L-01](#l-01)] | Return values not checked for `approve()` | 2| 0|
| [[L-02](#l-02)] | int/uint passed to abi.encodePacked without casting to string | 1| 0|
| [[L-03](#l-03)] | Chainlink answer is not compared against min/max values | 2| 0|
| [[L-04](#l-04)] | Function calls within loops | 7| 0|
| [[L-05](#l-05)] | Loops in external functions should be avoided due to high gas costs and possible DOS | 6| 0|
| [[L-06](#l-06)] | Missing zero address check in initializer | 3| 0|
| [[L-07](#l-07)] | Prefer skip over revert model in loop | 1| 0|
| [[L-08](#l-08)] | Upgradable contracts not taken into account when making wrapped calls | 9| 0|
| [[L-09](#l-09)] | Complex Computation - Multiplication on result of a Division | 4| 0|
| [[L-10](#l-10)] | Dangerous strict equalities | 18| 0|
| [[L-11](#l-11)] | Local variable shadowing | 3| 0|
| [[L-12](#l-12)] | Missing events arithmetic | 1| 0|
| [[L-13](#l-13)] | Missing zero address validation | 22| 0|
| [[L-14](#l-14)] | Benign reentrancy vulnerabilities | 22| 0|
| [[L-15](#l-15)] | Reentrancy vulnerabilities (events) | 38| 0|
| [[L-16](#l-16)] | Reentrancy vulnerabilities (loss of non-ether assets) | 11| 0|
| [[L-17](#l-17)] | Block timestamp | 13| 0|
| [[L-18](#l-18)] | Unchecked transfer | 6| 0|
| [[L-19](#l-19)] | Uninitialized local variables | 28| 0|
| [[L-20](#l-20)] | Uninitialized state variables | 2| 0|
| [[L-21](#l-21)] | Unused return | 22| 0|
| [[G-01](#g-01)] | Inefficient use of `abi.encode()` | 3| 300|
| [[G-02](#g-02)] | Cache address(this) when used more than once | 3| 0|
| [[G-03](#g-03)] | Multiple accesses of a mapping/array should use a local variable cache | 20| 0|
| [[G-04](#g-04)] | Constructors can be marked `payable` | 19| 399|
| [[G-05](#g-05)] | Division which can not overflow | 29| 2465|
| [[G-06](#g-06)] | Use assembly to emit events | 88| 3344|
| [[G-07](#g-07)] | Emitting events with struct/ state variables consume more gas | 7| 0|
| [[G-08](#g-08)] | Waste of GAS to emit variable literals | 9| 0|
| [[G-09](#g-09)] | Avoid emitting events in loops | 1| 0|
| [[G-10](#g-10)] | Emit event in setter function only if the state variable was changed | 22| 0|
| [[G-11](#g-11)] | Optimize Function Names to Save Gas | 9| 324|
| [[G-12](#g-12)] | Use nested if to save gas | 19| 0|
| [[G-13](#g-13)] | Internal or Private Function can be Inlined to Save Gas | 9| 180|
| [[G-14](#g-14)] | Using Storage Instead of Memory for structs/arrays Saves Gas | 5| 21000|
| [[G-15](#g-15)] | Modulus operations that could be unchecked | 2| 60|
| [[G-16](#g-16)] | Functions guaranteed to revert when called by normal users can be marked `payable` | 45| 0|
| [[G-17](#g-17)] | if variable is casted more than once, consider caching the result to save gas | 10| 0|
| [[G-18](#g-18)] | Inefficient Parameter Storage | 47| 2350|
| [[G-19](#g-19)] | Redundant state variable getters | 4| 0|
| [[G-20](#g-20)] | Argument validation should be at the top of the function/block | 2| 4200|
| [[G-21](#g-21)] | Split require/ assert statement | 14| 0|
| [[G-22](#g-22)] | Consider Merge Sequential Loops | 3| 0|
| [[G-23](#g-23)] | Avoid updating storage when the value hasn't changed | 14| 11200|
| [[G-24](#g-24)] | smaller uint/int types cause gas overhead | 8| 48|
| [[G-25](#g-25)] | Use Bytes32 for small data storage | 9| 0|
| [[G-26](#g-26)] | Solidity versions 0.8.19 and above are more gas efficient | 39| 0|
| [[G-27](#g-27)] | Optimal State Variable Order | 3| 15000|
| [[G-28](#g-28)] | Use assembly to write address storage values | 13| 1001|
| [[G-29](#g-29)] | State variable read in a loop | 5| 0|
| [[G-30](#g-30)] | State variable written in a loop | 1| 0|
| [[G-31](#g-31)] | Optimal Struct Variable Order | 4| 20000|
| [[G-32](#g-32)] | Safe Subtraction Should Be Unchecked | 12| 1020|
| [[G-33](#g-33)] | Unnecessary casting as variable is already of the same type | 2| 0|
| [[G-34](#g-34)] | Mappings are cheaper to use than storage arrays | 3| 0|
| [[G-35](#g-35)] | Consider activating via-ir for deploying | 1| 0|
| [[G-36](#g-36)] | Comparing to a Boolean constant | 1| 0|
| [[G-37](#g-37)] | State variables that could be declared constant | 10| 0|
| [[G-38](#g-38)] | Consider activating via-ir for deploying | 1| 0|
| [[G-39](#g-39)] | Shorten the array rather than copying to a new one | 1| 0|
| [[G-40](#g-40)] | checks for zero uint should be done using assembly to save gas | 29| 870|
| [[G-41](#g-41)] | Use Assembly for Hash Calculation | 13| 1040|
| [[G-42](#g-42)] | error strings longer than 32 characters consume more gas | 109| 1962|
| [[G-43](#g-43)] | `>=` costs less gas than `>` | 123| 369|
| [[G-44](#g-44)] | Counting down in for statements is more gas efficient | 11| 330|
| [[G-45](#g-45)] | Setting struct to 0 consumes more gas | 5| 0|
| [[G-46](#g-46)] | Avoid transferring amounts of zero in order to save gas | 7| 700|
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
| [[N-31](#n-31)] | Use scratch space when building emitted events with two data arguments | 31| 465|
| [[N-32](#n-32)] | Use `do`-`while` loop | 11| 0|
| [[N-33](#n-33)] | Accessing Multi-Dimensional Array | 23| 0|
| [[N-34](#n-34)] | Check `msg.sender` using `xor` and the scratch space | 20| 420|
