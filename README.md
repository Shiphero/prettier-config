# ShipHero's common prettier configuration
This repository serves as a common prettier configuration that may be shared across multiple Javascript projects within the company.

## Usage
If you want to use ShipHero's prettier config in your Javascript project, follow below steps:
1. Add dev dependency in your project's `package.json`:
```json
{
  "@shiphero/prettier-config": "github:shiphero/prettier-config"
}
```
2. Create `prettier.config.js` file in the root directory of your project containing:
```js
module.exports = require('@shiphero/prettier-config')
```

You can also overwrite our rules when needed:

```js
module.exports = {
  ...require('@shiphero/prettier-config'),
  // your custom set of rules goes here
}
```
