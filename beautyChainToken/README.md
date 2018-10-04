# BEC's ico contract

## contract on etherscan
[0xC5d105E63711398aF9bbff092d4B6769C82F793D](https://etherscan.io/address/0xc5d105e63711398af9bbff092d4b6769c82f793d#code)

## security issue
According to [peckshield](https://medium.com/@peckshield/alert-new-batchoverflow-bug-in-multiple-erc20-smart-contracts-cve-2018-10299-511067db6536):
> on 4/22/2018, someone transferred an extremely large amount of BEC token — 0x8000,0000,0000,0000,0000,0000,0000,0000,0000,0000,0000,0000,0000,0000,0000,0000(63 0’s).
> The vulnerable function is located in batchTransfer() line 257, the amount local variable is calculated as the product of cnt and _value. The second parameter, i.e., _value, can be an arbitrary 256 bits integer, say 0x8000,0000,0000,0000,0000,0000,0000,0000,0000,0000,0000,0000,0000,0000,0000,0000(63 0’s). By having two _receivers passed into batchTransfer(), with that extremely large _value, we can overflow amount and make it zero. With amount zeroed, an attacker can then pass the sanity checks in lines 258–259 and make the subtraction in line 261 irrelevant. Finally, here comes the interesting part: as shown in lines 262–265, the balance of the two receivers would be added by the extremely large _value without costing a dime in the the attacker’s pocket!
