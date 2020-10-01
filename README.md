# rugpullgame-contract


REMEMBER 
THE FUNNCTION:

```
    function randomWin() internal returns (uint) {
        uint randomnumber = uint(keccak256(abi.encodePacked(block.timestamp, msg.sender, nonce, block.difficulty))).mod(1000);
        randomnumber = randomnumber;
        nonce++;
        return randomnumber;
        }    
```

IS PREDICTABLE!!

If you wanna make the contract more safe, exclude contract calls.
But better is using a different algo for random numbers.
