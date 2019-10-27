# LancsToken
Generate CoSign Tokens for Lancaster University

This code is meant for educational purposes only.

[![npm version](https://badge.fury.io/js/lancstoken.svg)](https://badge.fury.io/js/lancstoken)

# Installation:
```sh
yarn add lancstoken
or
npm i lancstoken
```

# TODO:
Rewrite the Cosign Auth section, it is messy. will switch to a tailing function to clean it up :)

# Usage:
```js
const CoSign = require('lancstoken');
var account = new CoSign({
    user: "Username",
    pass: "Password",
});
account.getUserToken().then(()=>{
    console.log(account.token, account.cookie);
})


account.token //user token
account.cookie //user cookie
```
