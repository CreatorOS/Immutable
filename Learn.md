# Immutable
Immutable variables are like constants. Values of immutable variables can be set inside the constructor but cannot be modified afterwards.

Helpful for setting constant variables at time of deployment and not hardcoding like in case of `constant`.

```
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.3;

contract Immutable {
    // coding convention to uppercase constant variables
    address public immutable MY_ADDRESS;
    uint public immutable MY_UINT;

    constructor(uint _myUint) {
        MY_ADDRESS = msg.sender;
        MY_UINT = _myUint;
    }
}
```