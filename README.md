# @lcooper/pug-lint-config

[![npm][npm-badge]][npm-link]
[![license][license-badge]][license-link]

A sharable [pug-lint](https://github.com/pugjs/pug-lint) config for linting `pug` files.

## Installation

Install with the peer dependency [pug-lint](https://www.npmjs.com/package/pug-lint):

```bash
npm install --save-dev pug-lint @lcooper/pug-lint-config
```

## Usage

Add the `pugLintConfig` field to your `package.json` file:

```json
"pugLintConfig": {
  "extends": "@lcooper/pug-lint-config"
}
```

Or create a pug-lint config file type of your choice in the root folder of your project:

`.pug-lintrc` or `.pug-lintrc.json`

```json
{
  "extends": "@lcooper/pug-lint-config"
}
```

`.pug-lintrc.js`

```javascript
module.exports = {
    extends: '@lcooper/pug-lint-config',
};
```

## Scripts

Add a script to your `package.json` file:

```json
"scripts": {
  "lint:pug": "pug-lint **/*.pug"
}
```

[npm-link]: https://www.npmjs.com/package/@lcooper/pug-lint-config
[npm-badge]: https://img.shields.io/npm/v/@lcooper/pug-lint-config?logo=npm&style=for-the-badge
[license-link]: LICENSE
[license-badge]: https://img.shields.io/github/license/luciancooper/pug-lint-config?color=brightgreen&style=for-the-badge