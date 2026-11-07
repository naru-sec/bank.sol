# bank.sol
//mapping keywords  simple use example

// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;



contract Bank{
    mapping (address => uint) public balances;


    function deposit (uint _amount ) public {
     
     balances[msg.sender] += _amount; 
    }
}
