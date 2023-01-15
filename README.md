# Sudoku Smart Contract (zkSNARK)

## **Generate Key and WASM** 


```bash
cd circuits/sudoku
chmod u+x generate.sh

./generate.sh
```

After run the bellow commands, you will get some files, then we will copy the generated file to right folder

```bash
cp sudoku_final.zkey ../../zkproof/sudoku
cp sudoku.wasm ../../zkproof/sudoku
cp sudokuVerifier.sol ../../contracts
```

## **Test**

```
yarn test
```

## **Deploy contract**

```
npx hardhat run scripts/deploy.js --network mumbai
```