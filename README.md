# eslint-config-prlb [![npm version](https://badge.fury.io/js/eslint-config-prlb.svg)](https://badge.fury.io/js/eslint-config-prlb) [![Build Status](https://travis-ci.org/auzmartist/eslint-config-prlb.svg?branch=master)](https://travis-ci.org/auzmartist/eslint-config-prlb)

> ESLint [shareable config](http://eslint.org/docs/developer-guide/shareable-configs.html) for the [Google JavaScript style guide on which this is based](https://google.github.io/styleguide/jsguide.html)

## Usage

Once the `eslint-config-prlb` package is installed, you can use it by specifying `prlb` in the [`extends`](http://eslint.org/docs/user-guide/configuring#extending-configuration-files) section of your [ESLint configuration](http://eslint.org/docs/user-guide/configuring).

```js
{
	"extends": "prlb",
	"rules": {
		// Additional, per-project rules...
	}
}
```

### Using the `prlb` config with `eslint:recommended`

There are several rules in the [`eslint:recommended` ruleset](http://eslint.org/docs/rules/) that this style is not opinionated about that you might want to enforce in your project.

To use this style in conjunction with ESLint's recommended rule set, extend them both, making sure to list `prlb` last:

```js
{
	"extends": ["eslint:recommended", "prlb"],
	"rules": {
		// Additional, per-project rules...
	}
}
```

To see how the `prlb` config compares with `eslint:recommended`, refer to the [source code of `index.js`](https://github.com/auzmartist/eslint-config-prlb/blob/master/index.js), which lists every ESLint rule along with whether (and how) it is enforced by the `prlb` config. For more on how the Google style differs from this fork, visit the [eslint-config-google repository.](https://github.com/google/eslint-config-google/)


## License

Apache-2
