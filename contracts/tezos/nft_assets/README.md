# FA2 NFT Asset Contract

Implementation of the FA2 token contract (TZIP-12) for a NFT asset.

Instead of the off-chain view stored in the contract metadata as required
by the TZIP-12/TZIP-16 standards, this implementation provides access to token
metadata through on-chain `%token_metadata` view entry point.

## Project Structure

- [`ligo`](ligo/) - contracts code defined in [LIGO](https://ligolang.org/),
  smart-contract language for Tezos.
  - [`ligo/fa2`](ligo/fa2/) - FA2 contract interfaces and libraries
  - [`ligo/fa2_modules`](ligo/fa2_modules/) - reusable contract implementation modules
  - [`ligo/fa2_clients`](ligo/fa2_clients/) - test client contracts interacting
    with FA2 contract
  - [`ligo/src`](ligo/src/) folder - reference implementation of the multi-asset
    FA2 contract, test helper contracts and code.
  - [`ligo/out`](ligo/out/) folder - multi-asset FA2 contract and helper contract
    compiled into Michelson.
