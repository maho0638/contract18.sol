# contract18.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

// Smart contract event on Base network
contract Contract18 {
    event Action(address user, uint value);

    function trigger(uint value) public {
        emit Action(msg.sender, value);
    }
}
