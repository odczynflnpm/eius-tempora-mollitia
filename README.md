# @odczynflnpm/eius-tempora-mollitia <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][deps-svg]][deps-url]
[![dev dependency status][dev-deps-svg]][dev-deps-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Does the environment have full property descriptor support? Handles IE 8's broken defineProperty/gOPD.

## Example

```js
var hasPropertyDescriptors = require('@odczynflnpm/eius-tempora-mollitia');
var assert = require('assert');

assert.equal(hasPropertyDescriptors(), true); // will be `false` in IE 6-8, and ES5 engines

// Arrays can not have their length `[[Defined]]` in some engines
assert.equal(hasPropertyDescriptors.hasArrayLengthDefineBug(), false); // will be `true` in Firefox 4-22, and node v0.6
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@odczynflnpm/eius-tempora-mollitia
[npm-version-svg]: https://versionbadg.es/inspect-js/@odczynflnpm/eius-tempora-mollitia.svg
[deps-svg]: https://david-dm.org/inspect-js/@odczynflnpm/eius-tempora-mollitia.svg
[deps-url]: https://david-dm.org/inspect-js/@odczynflnpm/eius-tempora-mollitia
[dev-deps-svg]: https://david-dm.org/inspect-js/@odczynflnpm/eius-tempora-mollitia/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@odczynflnpm/eius-tempora-mollitia#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@odczynflnpm/eius-tempora-mollitia.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@odczynflnpm/eius-tempora-mollitia.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@odczynflnpm/eius-tempora-mollitia.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@odczynflnpm/eius-tempora-mollitia
[codecov-image]: https://codecov.io/gh/inspect-js/@odczynflnpm/eius-tempora-mollitia/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@odczynflnpm/eius-tempora-mollitia/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@odczynflnpm/eius-tempora-mollitia
[actions-url]: https://github.com/odczynflnpm/eius-tempora-mollitia/actions
