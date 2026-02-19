// SPDX-License-Identifier: MIT
pragma solidity ^0.8.18;

/**
 * @title SimpleStorage
 * @author K.M Knowledge Plus Media
 * @notice A basic smart contract to store and update a favorite number
 * @dev Demonstrates state variables and basic function interaction
 */
contract SimpleStorage {

    // State variable (stored permanently on blockchain)
    uint256 public favoriteNumber = 88;

    /**
     * @notice Updates the stored favorite number
     * @param _favoriteNumber The new number to store
     */
    function store(uint256 _favoriteNumber) public {
        favoriteNumber = _favoriteNumber;
    }

    /**
     * @notice Returns the currently stored favorite number
     * @return The stored favorite number
     */
    function retrieve() public view returns (uint256) {
        return favoriteNumber;
    }
}
