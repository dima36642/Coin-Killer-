// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";
import "@openzeppelin/contracts/access/Ownable.sol";

/**
 * @title Coin Killer
 * @dev This is the final contract for the Coin Killer (CK) token.
 * The entire initial supply is minted to the contract deployer.
 */
contract CoinKiller is ERC20, Ownable {
    /**
     * @dev The constructor sets the name, symbol, and owner.
     * @param initialOwner The address that will own the contract and receive all tokens.
     */
    constructor(address initialOwner)
        ERC20("Coin Killer", "CK") // Your Name and Symbol
        Ownable(initialOwner)
    {
        // Total supply of tokens to be created.
        // 1,000,000 with 18 decimal places. You can change the number 1000000 if you want.
        uint256 initialSupply = 1000000 * (10**decimals());
        _mint(initialOwner, initialSupply); // Mints the tokens to the owner's address.
    }
}
