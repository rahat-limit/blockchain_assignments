# First Assignment Documentation
Welcome to my respository, which I created due to Blockchain lessons. Here you can easily find some tasks with their explanations. Hope you like it🤙
## Usage
### ✖️ ⏲️ Function getLatestTransactionTimestamp, File Assignment.sol [(source)](https://github.com/rahat-limit/blockchain_assignments/blob/main/assignment.sol)
**Create a function to return the block timestamp of the latest transaction in a human-readable format.**
```solidity
  function getLatestTransactionTimestamp() external returns (uint256) { 
      uint256 currentTime = block.timestamp;
      uint256 currentHour = (currentTime / 3600) % 24; // Hour
      uint256 currentMinute = (currentTime / 60) % 60; // Minute
      uint256 currentSecond = currentTime % 60; // Second
      emit Timestamp(currentHour, currentMinute, currentSecond);
      return currentTime;
  }
```
**In log we can see human-readable format time (hours : minute : seconds)**
<p align="center">
  <img src = "https://github.com/rahat-limit/blockchain_assignments/blob/main/assets/time_result.png" width=600>
</p>

