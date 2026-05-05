# DigitSum.sol
DigitSum.sol
pragma solidity ^0.8.20;
contract DigitSum {
    function sum(uint n) public pure returns(uint) {
        uint s;
        while(n > 0){
            s += n % 10;
            n /= 10;
        }
        return s;
    }
}
