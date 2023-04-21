# ModuleFederationEnhacedPlugin
Module Federation with a little bit more and all remotes async by default

Dont want o read the docs? Here's a TL/DR:

## Features
- Modules' Name List
- Remotes' Name List
- Remotes' URL List and Map
- Remote definition with object
- Default async 


## Install
```sh
npm i @embrapa/module-federation-enhanced-plugin
```

## Config
```js
const ModuleFederationEnhacedPlugin = require("@embrapa/module-federation-enhanced-plugin");
module.export = {
  //... rest of your config
  plugins: [
    new ModuleFederationEnhancedPlugin({
    // same as the ModuleFederationPlugin config
      exposes: {
        Button: "./src/Button",
        Input: "./src/Input"
      },
    }),
  ],
};
```