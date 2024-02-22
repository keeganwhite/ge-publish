# ge-publish

> CLI tool to publish GE related smart contracts to Celo.

![GitHub release (latest by date)](https://img.shields.io/github/v/release/grassrootseconomics/ge-publish)

Supported Smart Contracts:

- [x] SwapPool
- [x] DecimalQuote
- [x] PriceIndexQuote
- [x] Limiter
- [x] LimiterIndex
- [x] TokenRegistry

## Install

Download and extract the binary for your OS/Arch from the [releases page](https://github.com/grassrootseconomics/ge-publish/releases).

### Linux

```bash
wget https://github.com/grassrootseconomics/ge-publish/releases/latest/download/ge-publish-linux-amd64.zip
unzip -j ge-publish-linux-amd64.zip
mv ge-publish-linux-amd64 ge-publish
# (Optional) Make it globally available
sudo mv ge-publish /usr/local/bin
```

## Usage

```bash
ge-publish --help
```

Examples:

### Limter

```bash
# Set your private key
export PRIVATE_KEY=
ge-publish --testnet publish limiter
```

### SwapPool

```bash
# Set your private key
export PRIVATE_KEY=
ge-publish --testnet publish swap-pool --name MySwapPool --symbol SWP1 --decimals 6 --token-registry 0x000000000000000000000000000000000000dEaD --token-limiter 0x000000000000000000000000000000000000dEaD
```

## License

[AGPL-3.0](LICENSE).