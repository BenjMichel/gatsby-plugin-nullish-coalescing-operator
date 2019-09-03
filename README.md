# Nullish coalescing operator support for Gatsby's Babel config

## Description

It enables the nullish coalescing operator (`a ?? b`): [see the TC39 proposal](https://github.com/tc39/proposal-nullish-coalescing)

## How to install

Install the plugin and its dependencies :

```bash
npm i gatsby-plugin-nullish-coalescing-operator @babel/core @babel/plugin-proposal-nullish-coalescing-operator
```

or

```bash
yarn add gatsby-plugin-nullish-coalescing-operator @babel/core @babel/plugin-proposal-nullish-coalescing-operator
```

Add the plugin in `gatsby-config.js`:

```js
module.exports = {
  plugins: [
    // other plugins
    'gatsby-plugin-nullish-coalescing-operator',
  ],
}
```

## Examples of usage

```js
const myString = '';
const headerText = myString ?? 'Default'; // result: '', whereas `myString || 'Default'` returns 'Default'
```
