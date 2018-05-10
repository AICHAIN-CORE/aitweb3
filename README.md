Forked from Ethereum web3.js project.
Change the address format rule : need a prefix: 'ai' instead of '0x'.

# AICHAIN JavaScript API
You need to run a local AICHAIN node to use this library.

still can use the document of ethereum for current version.
[Documentation](https://github.com/ethereum/wiki/wiki/JavaScript-API)

## Installation

### Node.js

```bash
npm install aitweb3
```

### Meteor.js  (not supported, need upload to meteor)

```bash
meteor add aichain:aitweb3
```

### As Browser module (not supported, need upload to Bower)
Bower

```bash
bower install aitweb3
```

* Include `web3.min.js` in your html file. (not required for the meteor package)

## Usage
Use the `web3` object directly from global namespace:

```js
console.log(web3); // {eth: .., shh: ...} // it's here!
```

Set a provider (HttpProvider)

```js
web3.setProvider(new web3.providers.HttpProvider('http://localhost:9523'));
```

There you go, now you can use it:

```js
var coinbase = web3.eth.coinbase;
var balance = web3.eth.getBalance(coinbase);
```

You can find more examples in [`example`](https://github.com/ethereum/web3.js/tree/master/example) directory.


## Contribute!

### Requirements

* Node.js
* npm

```bash
sudo apt-get update
sudo apt-get install nodejs
sudo apt-get install npm
sudo apt-get install nodejs-legacy
```

### Building (gulp)

```bash
npm run-script build
```


### Testing (mocha)

```bash
npm test
```

[npm-image]: https://badge.fury.io/js/web3.png
[npm-url]: https://npmjs.org/package/web3
[travis-image]: https://travis-ci.org/ethereum/web3.js.svg
[travis-url]: https://travis-ci.org/ethereum/web3.js
[dep-image]: https://david-dm.org/ethereum/web3.js.svg
[dep-url]: https://david-dm.org/ethereum/web3.js
[dep-dev-image]: https://david-dm.org/ethereum/web3.js/dev-status.svg
[dep-dev-url]: https://david-dm.org/ethereum/web3.js#info=devDependencies
[coveralls-image]: https://coveralls.io/repos/ethereum/web3.js/badge.svg?branch=master
[coveralls-url]: https://coveralls.io/r/ethereum/web3.js?branch=master
[waffle-image]: https://badge.waffle.io/ethereum/web3.js.svg?label=ready&title=Ready
[waffle-url]: http://waffle.io/ethereum/web3.js

