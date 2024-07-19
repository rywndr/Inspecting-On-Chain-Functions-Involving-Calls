# RealT Token Smart Contract Analysis

## Introduction

**Protocol Name**: RealT Token  
**Category**: RWA Tokenization  
**Smart Contract**: REALT

## Function Analysis

**Function Name**: `transfer`  

**Block Explorer Link**: [RealT Contract on Etherscan](https://etherscan.io/token/0x46cc7ec70746f4cbd56ce5fa9bb7d648398eaa5c#code)

**Function Code**:
```solidity
function transfer(address _to, uint _value) public NotBlacklisted(_to) NotBlacklisted(msg.sender) whenNotPaused {
    return super.transfer(_to, _value);
}
