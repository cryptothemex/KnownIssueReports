CryptoThemeX-CTX

## Summary

| |Issue|Instances| Gas Savings
|-|:-|:-:|:-:|
| [[M-01](#m-01)] | `burn` in a loop may lead to DoS attack | 1| 0|
| [[M-02](#m-02)] | `mint` in a loop may lead to DoS attack | 3| 0|
| [[L-01](#l-01)] | Array lengths may differ | 4| 0|
| [[L-02](#l-02)] | `tokenURI()` does not follow EIP-721 | 1| 0|
| [[L-03](#l-03)] | Function calls within loops | 6| 0|
| [[L-04](#l-04)] | Loops in external functions should be avoided due to high gas costs and possible DOS | 8| 0|
| [[L-05](#l-05)] | Possible length difference of two array parameters | 4| 0|
| [[L-06](#l-06)] | Missing events for `address` updates | 10| 0|
| [[L-07](#l-07)] | Prefer skip over revert model in loop | 1| 0|
| [[L-08](#l-08)] | Missing events arithmetic | 1| 0|
| [[L-09](#l-09)] | Missing zero address validation | 24| 0|
| [[L-10](#l-10)] | Benign reentrancy vulnerabilities | 6| 0|
| [[L-11](#l-11)] | Reentrancy vulnerabilities (events) | 10| 0|
| [[L-12](#l-12)] | Reentrancy vulnerabilities (loss of non-ether assets) | 11| 0|
| [[L-13](#l-13)] | Block timestamp | 6| 0|
| [[L-14](#l-14)] | Unused return | 1| 0|
| [[L-15](#l-15)] | Centralization Risk for trusted owners | 1| 0|
| [[L-16](#l-16)] | Direct `supportsInterface()` calls may cause caller to revert | 1| 0|
| [[L-17](#l-17)] | Missing checks for zero address when assigning values to address state variables | 24| 0|
| [[L-18](#l-18)] | Do not use deprecated library functions | 3| 0|
| [[L-19](#l-19)] | Deprecated _setupRole() function | 3| 0|
| [[L-20](#l-20)] | Division by zero not prevented | 3| 0|
| [[L-21](#l-21)] | Signature use at deadlines should be allowed | 5| 0|
| [[L-22](#l-22)] | Prevent accidentally minting/ burning tokens | 15| 0|
| [[L-23](#l-23)] | NFT ownership doesn't support hard forks | 1| 0|
| [[L-24](#l-24)] | Loss of precision | 2| 0|
| [[L-25](#l-25)] | Solidity version 0.8.20+ may not work on other chains due to `PUSH0` | 8| 0|
| [[L-26](#l-26)] | Use `Ownable2Step.transferOwnership` instead of `Ownable.transferOwnership` | 7| 0|
| [[L-27](#l-27)] | File allows a version of solidity that is susceptible to an assembly optimizer bug | 8| 0|
| [[L-28](#l-28)] | Sweeping may break accounting if tokens with multiple addresses are used | 2| 0|
| [[L-29](#l-29)] | Unsafe ERC20 operation(s) | 7| 0|
| [[L-30](#l-30)] | Unspecific compiler version pragma | 8| 0|
| [[G-01](#g-01)] | `abi.encode()` is less efficient than `abi.encodepacked()` for non-address arguments | 1| 0|
| [[G-02](#g-02)] | Use `Array.unsafeAccess()` to avoid repeated array length checks | 6| 0|
| [[G-03](#g-03)] | Cache address(this) when used more than once | 1| 0|
| [[G-04](#g-04)] | Multiple accesses of a mapping/array should use a local variable cache | 36| 0|
| [[G-05](#g-05)] | Constructors can be marked `payable` | 8| 0|
| [[G-06](#g-06)] | Division which can not overflow | 1| 0|
| [[G-07](#g-07)] | Use assembly to emit events | 18| 0|
| [[G-08](#g-08)] | emitting events with struct/ state variables consume more gas | 3| 0|
| [[G-09](#g-09)] | emit event in setter function only if the state variable was changed | 4| 0|
| [[G-10](#g-10)] | Use nested if to save gas | 1| 0|
| [[G-11](#g-11)] | Initializing non-`constant`/non-`immutable` state variables to zero/false costs more gas | 4| 0|
| [[G-12](#g-12)] | Functions guaranteed to revert when called by normal users can be marked `payable` | 64| 0|
| [[G-13](#g-13)] | `private` functions only called once can be inlined to save gas | 5| 0|
| [[G-14](#g-14)] | Argument validation should be at the top of the function/block | 4| 0|
| [[G-15](#g-15)] | Avoid updating storage when the value hasn't changed | 14| 0|
| [[G-16](#g-16)] | smaller uint/int types cause gas overhead | 13| 0|
| [[G-17](#g-17)] | Solidity versions 0.8.19 and above are more gas efficient | 8| 0|
| [[G-18](#g-18)] | State variable read in a loop | 14| 0|
| [[G-19](#g-19)] | State variable written in a loop | 7| 0|
| [[G-20](#g-20)] | Mappings are cheaper to use than storage arrays | 4| 0|
| [[G-21](#g-21)] | Comparing to a Boolean constant | 3| 0|
| [[G-22](#g-22)] | State variables that could be declared constant | 3| 0|
| [[G-23](#g-23)] | State variables that could be declared immutable | 12| 0|
| [[G-24](#g-24)] | Event is never emitted | 1| 0|
| [[G-25](#g-25)] | `public` functions not called internally should be declared `external` to save gas | 19| 0|
| [[G-26](#g-26)] | Shorten the array rather than copying to a new one | 1| 0|
| [[G-27](#g-27)] | checks for zero uint should be done using assembly to save gas | 8| 240|
| [[G-28](#g-28)] | Use assembly hashing | 8| 0|
| [[G-29](#g-29)] | error strings longer than 32 characters consume more gas | 8| 0|
| [[G-30](#g-30)] | Counting down in for statements is more gas efficient | 17| 510|
| [[G-31](#g-31)] | Use ERC721A instead ERC721 | 1| 0|
| [[G-32](#g-32)] | `a = a + b` is more gas effective than `a += b` for state variables (excluding arrays and mappings) | 33| 528|
| [[G-33](#g-33)] | Using bools for storage incurs overhead | 12| 1200|
| [[G-34](#g-34)] | Cache array length outside of loop | 1| 0|
| [[G-35](#g-35)] | State variables should be cached in stack variables rather than re-reading them from storage | 3| 300|
| [[G-36](#g-36)] | Use calldata instead of memory for function arguments that do not get mutated | 8| 480|
| [[G-37](#g-37)] | Use Custom Errors instead of Revert Strings to save Gas | 80| 4000|
| [[G-38](#g-38)] | Avoid contract existence checks by using low level calls | 4| 400|
| [[G-39](#g-39)] | State variables only set in the constructor should be declared `immutable` | 12| 0|
| [[G-40](#g-40)] | `++i` costs less gas compared to `i++` or `i += 1` (same for `--i` vs `i--` or `i -= 1`) | 17| 85|
| [[G-41](#g-41)] | Using `private` rather than `public`, saves gas | 68| 0|
| [[G-42](#g-42)] | Use shift right/left instead of division/multiplication if possible | 1| 0|
| [[G-43](#g-43)] | Splitting `require()` statements that use `&&` saves gas | 1| 3|
| [[G-44](#g-44)] | `uint256` to `bool` `mapping`: Utilizing Bitmaps to dramatically save on Gas | 4| 0|
| [[G-45](#g-45)] | Increments/decrements can be `unchecked` in for-loops | 17| 510|
| [[G-46](#g-46)] | Use `!= 0` instead of `> 0` for unsigned integer comparison | 12| 48|
| [[N-01](#n-01)] | Consider providing a ranged getter for array state variables | 4| 0|
| [[N-02](#n-02)] | Consider emitting an event at the end of the constructor | 8| 0|
| [[N-03](#n-03)] | Similar Constants decalred in Multiple Contracts  | 1| 0|
| [[N-04](#n-04)] | Duplicate error strings | 4| 0|
| [[N-05](#n-05)] | Events are missing sender information | 8| 0|
| [[N-06](#n-06)] | Validate user inputs | 32| 0|
| [[N-07](#n-07)] | `msg.sender` in `require` | 8| 0|
| [[N-08](#n-08)] | Costly operations inside a loop | 1| 0|
| [[N-09](#n-09)] | Cyclomatic complexity | 1| 0|
| [[N-10](#n-10)] | Incorrect versions of Solidity | 8| 0|
| [[N-11](#n-11)] | Conformance to Solidity naming conventions | 2| 0|
| [[N-12](#n-12)] | Array is `push()`ed | 2| 0|
| [[N-13](#n-13)] | Contract timekeeping will break earlier than the Ethereum network itself will stop working | 2| 0|
| [[N-14](#n-14)] | Consider splitting complex checks into multiple steps | 5| 0|
| [[N-15](#n-15)] | Constants in comparisons should appear on the left side | 33| 0|
| [[N-16](#n-16)] | use `AccessControlDefaultAdminRules` rather than `AccessControl` | 1| 0|
| [[N-17](#n-17)] | Consider adding emergency-stop functionality | 5| 0|
| [[N-18](#n-18)] | Consider making contracts `Upgradeable` | 5| 0|
| [[N-19](#n-19)] | Consider using descriptive `constant`s when passing zero as a function argument | 6| 0|
| [[N-20](#n-20)] | Use of `override` is unnecessary | 6| 0|
| [[N-21](#n-21)] | Consider using a `struct` rather than having many function input parameters | 19| 0|
| [[N-22](#n-22)] | Import declarations should import specific identifiers, rather than the whole file | 5| 0|
| [[N-23](#n-23)] | Consider using named function arguments | 18| 0|
| [[N-24](#n-24)] | Consider using named returns | 17| 0|
| [[N-25](#n-25)] | Returning a struct instead of returning many variables is better | 3| 0|
| [[N-26](#n-26)] | Array indices should be referenced via `enum`s rather than via numeric literals | 20| 0|
| [[N-27](#n-27)] | `constant`s should be defined rather than using magic numbers | 25| 0|
| [[N-28](#n-28)] | Control structures do not follow the Solidity Style Guide | 4| 0|
| [[N-29](#n-29)] | Duplicated `require()`/`revert()` Checks Should Be Refactored To A Modifier Or Function | 4| 0|
| [[N-30](#n-30)] | Event missing indexed field | 16| 0|
| [[N-31](#n-31)] | Events that mark critical parameter changes should contain both the old and the new value | 3| 0|
| [[N-32](#n-32)] | Change `int` to `int256` | 5| 0|
| [[N-33](#n-33)] | Missing Event for critical parameters change | 14| 0|
| [[N-34](#n-34)] | Incomplete NatSpec: `@param` is missing on actually documented functions | 3| 0|
| [[N-35](#n-35)] | Use a `modifier` instead of a `require/if` statement for a special `msg.sender` actor | 64| 0|
| [[N-36](#n-36)] | Constant state variables defined more than once | 3| 0|
| [[N-37](#n-37)] | Consider using named mappings | 39| 0|
| [[N-38](#n-38)] | Adding a `return` statement when the function defines a named return variable, is redundant | 1| 0|
| [[N-39](#n-39)] | `require()` / `revert()` statements should have descriptive reason strings | 67| 0|
| [[N-40](#n-40)] | Use scientific notation (e.g. `1e18`) rather than exponentiation (e.g. `10**18`) | 8| 0|
| [[N-41](#n-41)] | Contract does not follow the Solidity style guide's suggested layout ordering | 7| 0|
| [[N-42](#n-42)] | Use Underscores for Number Literals (add an underscore every 3 digits) | 2| 0|
| [[N-43](#n-43)] | Event is missing `indexed` on some of the fields | 16| 0|
| [[N-44](#n-44)] | Variables need not be initialized to zero | 26| 0|
| [[N-45](#n-45)] | Use scratch space when building emitted events with two data arguments | 10| 150|
| [[N-46](#n-46)] | Use `do`-`while` loop | 17| 0|
| [[N-47](#n-47)] | `>=` costs less gas than `>` | 41| 123|
| [[N-48](#n-48)] | Accessing Multi-Dimensional Array | 43| 0|
| [[N-49](#n-49)] | Check `msg.sender` using `xor` and the scratch space | 43| 903|
| [[N-50](#n-50)] | Avoid transferring amounts of zero in order to save gas | 8| 800|
