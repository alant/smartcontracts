# Honeypot contract
This is a honeypot contract. Something I learned at Trufflecon 2018, Portland OR. It's too good not to share.
On the surface, it looks like a reentracy attack target. However, it's a bit deeper than that. The contract is actually a honey trap that will trap the ETH you send hoping to attack with reentrancy vulnerability. Very clever.

Many thanks to Mike Seese (seesemichaelj) on the Truffle team to share with us the details of this contract and ganache fork feature.  

## contract on etherscan
[etherscan link](https://etherscan.io/address/0x95d34980095380851902ccd9a1fb4c813c2cb639#code)

## related articles
[TruffleCon 2018 - It's a Trap! Forking Workshop Steps](https://docs.google.com/document/d/1PF_LGcnMKfLxe9E4kzwb4r1vhUoGa35PNZmEIZANF3Q/mobilebasic)

[Reentrancy Attack On Smart Contracts: How To Identify The Exploitable And An Example Of An Attack Contract](https://medium.com/@gus_tavo_guim/reentrancy-attack-on-smart-contracts-how-to-identify-the-exploitable-and-an-example-of-an-attack-4470a2d8dfe4)
