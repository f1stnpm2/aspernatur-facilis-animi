# @f1stnpm2/aspernatur-facilis-animi <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Get the ArrayBuffer out of a TypedArray, robustly.

This will work in node <= 0.10 and < 0.11.4, where there's no prototype accessor, only a nonconfigurable own property.
It will also work in modern engines where `TypedArray.prototype.buffer` has been deleted after this module has loaded.

## Example

```js
const typedArrayBuffer = require('@f1stnpm2/aspernatur-facilis-animi');
const assert = require('assert');

const arr = new Uint8Array(0);
assert.equal(arr.buffer, typedArrayBuffer(arr));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@f1stnpm2/aspernatur-facilis-animi
[npm-version-svg]: https://versionbadg.es/inspect-js/@f1stnpm2/aspernatur-facilis-animi.svg
[deps-svg]: https://david-dm.org/inspect-js/@f1stnpm2/aspernatur-facilis-animi.svg
[deps-url]: https://david-dm.org/inspect-js/@f1stnpm2/aspernatur-facilis-animi
[dev-deps-svg]: https://david-dm.org/inspect-js/@f1stnpm2/aspernatur-facilis-animi/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@f1stnpm2/aspernatur-facilis-animi#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@f1stnpm2/aspernatur-facilis-animi.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@f1stnpm2/aspernatur-facilis-animi.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@f1stnpm2/aspernatur-facilis-animi.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@f1stnpm2/aspernatur-facilis-animi
[codecov-image]: https://codecov.io/gh/inspect-js/@f1stnpm2/aspernatur-facilis-animi/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@f1stnpm2/aspernatur-facilis-animi/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@f1stnpm2/aspernatur-facilis-animi
[actions-url]: https://github.com/inspect-js/@f1stnpm2/aspernatur-facilis-animi/actions
