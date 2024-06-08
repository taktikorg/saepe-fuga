# @taktikorg/saepe-fuga <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

`Object.defineProperty`, but not IE 8's broken one.

## Example

```js
const assert = require('assert');

const $defineProperty = require('@taktikorg/saepe-fuga');

if ($defineProperty) {
    assert.equal($defineProperty, Object.defineProperty);
} else if (Object.defineProperty) {
    assert.equal($defineProperty, false, 'this is IE 8');
} else {
    assert.equal($defineProperty, false, 'this is an ES3 engine');
}
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

## Security

Please email [@ljharb](https://github.com/ljharb) or see https://tidelift.com/security if you have a potential security vulnerability to report.

[package-url]: https://npmjs.org/package/@taktikorg/saepe-fuga
[npm-version-svg]: https://versionbadg.es/ljharb/@taktikorg/saepe-fuga.svg
[deps-svg]: https://david-dm.org/ljharb/@taktikorg/saepe-fuga.svg
[deps-url]: https://david-dm.org/ljharb/@taktikorg/saepe-fuga
[dev-deps-svg]: https://david-dm.org/ljharb/@taktikorg/saepe-fuga/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@taktikorg/saepe-fuga#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@taktikorg/saepe-fuga.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@taktikorg/saepe-fuga.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@taktikorg/saepe-fuga.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@taktikorg/saepe-fuga
[codecov-image]: https://codecov.io/gh/ljharb/@taktikorg/saepe-fuga/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@taktikorg/saepe-fuga/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@taktikorg/saepe-fuga
[actions-url]: https://github.com/taktikorg/saepe-fuga/actions
