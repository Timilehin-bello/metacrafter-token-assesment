# MyToken Smart Contract

This is a simple smart contract written in Solidity that represents a token called "MyToken". The contract includes functionality to mint and burn tokens, as well as track the balances of token holders.

## Requirements

1. The contract includes public variables to store the details about the token:

   - `name`: The name of the token.
   - `symbol`: The symbol or abbreviation of the token.
   - `totalSupply`: The total supply of tokens.

2. The contract uses a mapping to keep track of token balances for each address:

   - `balanceOf`: A mapping that maps addresses to their corresponding token balances.

3. The `mint` function is responsible for creating new tokens and assigning them to a specific address. It takes two parameters:

   - `_to`: The address to which the tokens will be assigned.
   - `_value`: The number of tokens to be minted and assigned.

4. The `burn` function is responsible for destroying tokens. It works in the opposite way to the `mint` function, reducing the total supply and deducting tokens from a specific address. It takes two parameters:

   - `_to`: The address from which the tokens will be burned.
   - `_value`: The number of tokens to be burned.

5. The `burn` function includes conditionals to ensure that the balance of the address is greater than or equal to the amount of tokens that should be burned.

## Usage

1. Deploy the `MyToken` contract on a compatible blockchain platform, such as Ethereum.
2. Interact with the contract by calling its functions:
   - `mint`: Call this function to create new tokens and assign them to an address.
   - `burn`: Call this function to destroy tokens and reduce the total supply.

## License

This contract is released under the MIT License. Please see the `LICENSE` file for more information.

## Acknowledgments

This code was created as an assessment solution to create a token using Solidity as a Metacrafter😎.

Feel free to customize and expand upon this code to meet your specific requirements. It serves as a starting point for building more complex Token contract or integrating with blockchain technologies.
