# unofficial common-blockchain biteasy adapter

A Biteasy adapter built to standardize the output of requests to follow the union of the bitcoind and common-blockchain convention. Aliases are introduced in the return of functions to account for differences in convention between the two standards. It is our hope that the Bitcoin community will come to an agreement on proper style and convention for requests on addresses, transactions, and blocks.

## Installation

Install as you normally install an npm module:
```
  npm install biteasy-unofficial
```

## Usage

To use the Biteasy API, simply require the module.
```
  var biteasyAPI = require('biteasy-unofficial');
```
For Mainnet, use ```biteasyAPI({ network: 'mainnet' })``` when calling a function. For Testnet, use ```biteasyAPI({network: 'testnet'})``` when calling a function. By default, if no parameter is provided, Mainnet will be used.

```javascript
var commonBlockchain = biteasyAPI({ network: 'mainnet' });
```
[See abstract-common-blockchain for API](https://github.com/blockai/abstract-common-blockchain/edit/master/README.md)

## Convention

Standard convention is described fully in the ```types.json``` file.

## Maintainers
  * Howard Wu (howardwu) - howardwu@berkeley.edu
  * Andrew Malta (andrewmalta13) - andrew.malta@yale.edu
