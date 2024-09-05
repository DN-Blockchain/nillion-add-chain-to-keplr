## Add Chain to Keplr Wallet

This library provides a React component that allows users to add chain to Keplr Wallet. The functionality is provided by using a button exported by the library.

### Installation

```
npm install add-chain-keplr-wallet-component
```

### Usage

```javascript
import AddChainToKeplrButton from "add-chain-keplr-wallet-component";

const chainInfo = {
  rpc: "https://testnet-nillion-rpc.lavenderfive.com",
  rest: "https://testnet-nillion-api.lavenderfive.com",
  nodeProvider: {
    name: "Lavender.Five",
    email: "hello@lavenderfive.com",
    website: "https://www.lavenderfive.com/",
  },
  chainId: "nillion-chain-testnet-1",
  chainName: "Nillion Testnet",
  chainSymbolImageUrl:
    "https://raw.githubusercontent.com/chainapsis/keplr-chain-registry/main/images/nillion-chain-testnet/nil.png",
  stakeCurrency: {
    coinDenom: "NIL",
    coinMinimalDenom: "unil",
    coinDecimals: 6,
    coinImageUrl:
      "https://raw.githubusercontent.com/chainapsis/keplr-chain-registry/main/images/nillion-chain-testnet/nil.png",
  },
  bip44: {
    coinType: 118,
  },
  bech32Config: {
    bech32PrefixAccAddr: "nillion",
    bech32PrefixAccPub: "nillionpub",
    bech32PrefixValAddr: "nillionvaloper",
    bech32PrefixValPub: "nillionvaloperpub",
    bech32PrefixConsAddr: "nillionvalcons",
    bech32PrefixConsPub: "nillionvalconspub",
  },
  currencies: [
    {
      coinDenom: "NIL",
      coinMinimalDenom: "unil",
      coinDecimals: 6,
      coinImageUrl:
        "https://raw.githubusercontent.com/chainapsis/keplr-chain-registry/main/images/nillion-chain-testnet/nil.png",
    },
  ],
  feeCurrencies: [
    {
      coinDenom: "NIL",
      coinMinimalDenom: "unil",
      coinDecimals: 6,
      coinImageUrl:
        "https://raw.githubusercontent.com/chainapsis/keplr-chain-registry/main/images/nillion-chain-testnet/nil.png",
      gasPriceStep: {
        low: 0.001,
        average: 0.001,
        high: 0.01,
      },
    },
  ],
  features: [],
};

<AddChainToKeplrButton text={"Add NilChain to Keplr"} chainInfo={chainInfo} style={} />;
```

### Props

| Prop Name       | Type     | Description                                                            |
| --------------- | -------- | ---------------------------------------------------------------------- |
| chainInfo       | object   | Chain information.                  |
| text      | string   | The text to display on the button.                                     |
| style    | object | Custom style for button                               |
