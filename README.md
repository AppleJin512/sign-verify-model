# Coinracer Smart Pool
Simple Signature Verification Model

1. Clone repo

```shell
git clone https://github.com/Coinracer-io/signature-verification-model.git
```

2. Install yarn packages

```shell
cd signature-verification-model
yarn install
```

3. Rename `.env.example` to `.env` and paste your mnemonic and bscscan api key. They will be used for deploying and verifying contracts on live networks

```shell
BSCSCAN_API=<YOUR-BSCSCAN-API-KEY>
PRIVATE_KEY=<YOUR-PRIVATE-KEY>
CMC_APIKEY=<YOUR-COINMARKETCAP-API-KEY>
BSCTEST_RPC_URL=https://data-seed-prebsc-1-s1.binance.org:8545/

SIGNER_PRIVATE_KEY=<SIGNER-PRIVATE-KEY>
SIGNER_ADDRESS=<SIGNER-ADDRESS>
```

4. Test the model

```shell
yarn test
```

4. Deploy the contract

```shell
yarn deploy
```

5. Verify the contract

```shell
npx hardhat verify --network bsctest <YOUR_DEPLOYED_ADDRESS> "0x0000000000000000000000000000000000000000"
```
