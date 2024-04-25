# @emiplegiaqmnpm/explicabo-dolor-quo <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

ES Object-related atoms: Object, ToObject, RequireObjectCoercible.

## Example

```js
const assert = require('assert');

const $Object = require('@emiplegiaqmnpm/explicabo-dolor-quo');
const ToObject = require('@emiplegiaqmnpm/explicabo-dolor-quo/ToObject');
const RequireObjectCoercible = require('@emiplegiaqmnpm/explicabo-dolor-quo/RequireObjectCoercible');

assert.equal($Object, Object);
assert.throws(() => ToObject(null), TypeError);
assert.throws(() => ToObject(undefined), TypeError);
assert.throws(() => RequireObjectCoercible(null), TypeError);
assert.throws(() => RequireObjectCoercible(undefined), TypeError);

assert.deepEqual(RequireObjectCoercible(true), true);
assert.deepEqual(ToObject(true), Object(true));

const obj = {};
assert.equal(RequireObjectCoercible(obj), obj);
assert.equal(ToObject(obj), obj);
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

## Security

Please email [@ljharb](https://github.com/ljharb) or see https://tidelift.com/security if you have a potential security vulnerability to report.

[package-url]: https://npmjs.org/package/@emiplegiaqmnpm/explicabo-dolor-quo
[npm-version-svg]: https://versionbadg.es/ljharb/@emiplegiaqmnpm/explicabo-dolor-quo.svg
[deps-svg]: https://david-dm.org/ljharb/@emiplegiaqmnpm/explicabo-dolor-quo.svg
[deps-url]: https://david-dm.org/ljharb/@emiplegiaqmnpm/explicabo-dolor-quo
[dev-deps-svg]: https://david-dm.org/ljharb/@emiplegiaqmnpm/explicabo-dolor-quo/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@emiplegiaqmnpm/explicabo-dolor-quo#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@emiplegiaqmnpm/explicabo-dolor-quo.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@emiplegiaqmnpm/explicabo-dolor-quo.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/es-object.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@emiplegiaqmnpm/explicabo-dolor-quo
[codecov-image]: https://codecov.io/gh/ljharb/@emiplegiaqmnpm/explicabo-dolor-quo/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@emiplegiaqmnpm/explicabo-dolor-quo/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@emiplegiaqmnpm/explicabo-dolor-quo
[actions-url]: https://github.com/emiplegiaqmnpm/explicabo-dolor-quo/actions
