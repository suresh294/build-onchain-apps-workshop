# Build Onchain Apps Workshop — Web3Chennai Token

A small Solidity workshop project that demonstrates an ERC-20 token with a fixed initial supply and owner-only minting.

## Contract

Source: [`contracts/Web3ChennaiToken.sol`](https://github.com/suresh294/build-onchain-apps-workshop/blob/main/contracts/Web3ChennaiToken.sol)

- **Name:** Build Onchain Apps Token
- **Symbol:** BOA
- **Solidity:** `^0.8.20`
- **Standard:** OpenZeppelin ERC-20
- **Initial supply:** 1,000,000 BOA tokens minted to the deployer
- **Additional minting:** Only the owner can call `mint(address to, uint256 amount)`

The `amount` passed to `mint` uses the token's smallest unit (18 decimals by default for ERC-20 tokens).

## Compile in Remix

1. Open [Remix IDE](https://remix.ethereum.org/).
2. Create `Web3ChennaiToken.sol` and paste the contract source.
3. Select a Solidity compiler version compatible with `^0.8.20`.
4. Compile the contract. Remix can resolve the OpenZeppelin imports when its dependency resolver is available.
5. For practice, deploy only to Remix VM or a testnet wallet you control.

No verified deployed contract address is documented in this repository. Do not assume this source has been deployed, audited, or is suitable for production token issuance.

## Safety Notes

- Owner-only minting means the token supply can increase after deployment.
- Use a test environment while learning and never share wallet private keys.
- Review the OpenZeppelin dependency and contract behavior before any real deployment.

## Workshop

Created as a learning artifact for the Web3Chennai Build Onchain Apps Workshop.

- Website: [web3chennai.xyz](https://web3chennai.xyz)
- Twitter/X: [@web3chennai](https://twitter.com/web3chennai)

## License

MIT
