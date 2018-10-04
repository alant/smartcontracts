# SMT's ico contract

## contract on etherscan
[0x55F93985431Fc9304077687a35A1BA103dC1e081](https://etherscan.io/address/0x55F93985431Fc9304077687a35A1BA103dC1e081#code)

## security issue
According to [peckshield](https://blog.peckshield.com/2018/04/25/proxyOverflow/):
> if _fee + _value happens to be 0 (the overflow case), the sanity checks in line 206 could be passed. It means the attacker could transfer huge amount of tokens to an address (line 214) with zero balance. Also, a huge amount fee would be transferred to the msg.sender in line 217.
