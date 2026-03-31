# Simple-On-Chain-Notes-User-Notes-
Simple On‑Chain Notes (User → Notes)
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract Notes {
    mapping(address => string[]) public notes;

    function add(string memory text) public {
        notes[msg.sender].push(text);
    }
}
