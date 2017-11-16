# eslint-config-onz-base

This is the base eslint config for use in Onz projects. It extends [`eslint-config-airbnb-base`](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb-base), with a few overrides.

## Installation

```bash
npm install --save-dev eslint-config-onz-base
```

## Usage

In your `.eslintrc.json` file:
```json
{
  "extends": ["onz-base"]
}
```

## Contributing

PRs are welcome if the reasoning for the proposed change is provided.

## Divergence from `eslint-config-airbnb-base`

### `camelcase`

Enforce camelcase for properties as well.

### `eqeqeq`

Don't ignore null.

### `indent` and `no-tabs`

Use tabs. Tabs are for indentation, spaces are for separation.

### `new-cap`

Call uppercase-started functions with `new`. Exception pattern is added for compatibility with [`should.js`](https://shouldjs.github.io/).

### `no-console`

Don't leave console statements lying around. Exceptions for `console.error`, `console.info` and `console.warn` so you can use console statements if you really mean it.
