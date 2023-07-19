# Gas Optimization

![12 July - Gas Optimisation Challenge](https://github.com/clement-stackup/gas_challenge/assets/120361535/21c826fb-8776-4837-a8fe-b7040426eafa)

## Getting Started

To get started, clone this repository to your local machine and navigate to the project directory. Next, install the required dependencies.

```bash
git clone https://github.com/alade-dev/gas_challenge.git
cd gas_challenge && npm install
```

Once you have cloned the repository and installed the necessary dependencies, open the `contracts/gasChallenge.sol` file to view the smart contract and apply the following gas optimization techniques above.

## Test Smart Contract

Next, head over to `test/test_gasChallenge.js`. You are required to write a unit test under the describe block to check that after running the gas optimized function, the sum of array is 0. Once you have implemented the test block, proceed the run the following command to test your smart contract.

```bash
npx hardhat test
```

This command will test the smart contract and compute the estimated gas cost. This is computed using the [hardhat-gas-reporter](https://www.npmjs.com/package/hardhat-gas-reporter) library.

The library has been configured to output the estimated gas costs to a new `gas-report.txt` file on your root directory. You can then view the estimated gas consumption for each of the smart contract functions in this file. The `optimizedFunction()` should output a lower gas consumption to the `notOptimizedFunction()` as shown below.

![Screenshot 2023-07-11 at 2 34 24 PM](https://github.com/clement-stackup/gas_challenge/assets/120361535/99e33517-5974-40a1-aa87-279051e58e42)

This command will also check if the sum of the array returns 0. You can refer below to view the terminal console when all tests have passed!

![image](https://github.com/clement-stackup/gas_challenge/assets/120361535/760df9a2-c9f5-4c0f-af50-7a88093bdbda)



