# University Token

## Usage

This Solidity smart contract, named UniversityToken, is an ERC-20 token that represents a university-specific currency. The token is named "AITU_Shamil" with the symbol "SHA". It includes additional functionality to retrieve information about transactions within the token.

## Demo Screenshots

![image](https://github.com/shomyich/blockchain_assignment_1/assets/129707076/995d3738-2671-4c96-8a7e-72ff7cd827ff)

## Examples

Below are examples of using the UniversityToken contract:

### Minting Tokens

```solidity
// Mint 2000 tokens to the contract deployer
_mint(msg.sender, 2000);
```

### Checking Latest Transaction Timestamp

```solidity
// Get the timestamp of the latest transaction
uint256 timestamp = getLatestTransactionTimestamp();
```

### Checking Transaction Sender

```solidity
// Get the address of the transaction sender
address sender = getTransactionSender();
```

### Checking Transaction Receiver

```solidity
// Get the address of the transaction receiver (owner of the contract)
address receiver = getTransactionReceiver();
```

### Access Control with OnlyOwner Modifier

```solidity
// Use onlyOwner modifier to restrict access to certain functions
function restrictedFunction() public onlyOwner {
    // Function logic accessible only by the contract owner
}
```

## License
https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/LICENSE 
