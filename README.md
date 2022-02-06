# bep20-contract-template
Token templates for BEP20 Binance Smart Chain.
- Standard BEP20 Token
- Mint and Burn BEP20 Token
- TAX BEP20 Token
- Standard and Burn BEP20 Token
- Baby BEP20 Token
- Safemoon Token Clone

Before deploying the token change the constructor:

```solidity
 constructor() public {
    _name = "BEP20 Standard";
    _symbol = "BEST";
    _decimals = 8;
    _totalSupply = 10000000000000; // 100 thousand
    _balances[msg.sender] = _totalSupply;    
```
NOTE: zeros in total supply must be decimals + supply you want (8 zeros for decimals and 5 zeros for 100k total supply)
