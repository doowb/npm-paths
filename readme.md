# npm-paths [![NPM version](https://badge.fury.io/js/npm-paths.svg)](http://badge.fury.io/js/npm-paths)  [![Build Status](https://travis-ci.org/jonschlinkert/npm-paths.svg)](https://travis-ci.org/jonschlinkert/npm-paths)

> Returns an array of unique "global" directories based on the user's platform and environment. The resulting paths can be used for doing lookups for generators or other globally installed npm packages. Node.js / JavaScript.

This lib does not include the `require.main.paths` in the result array. If you do need the `require.main.paths`, use [global-paths][] instead.

## Install

Install with [npm](https://www.npmjs.com/)

```sh
$ npm i npm-paths --save
```

## Usage

```js
var paths = require('npm-paths');
console.log(paths())
```

## Example results

Results in something like the following:

**Mac**

```js
[ '/Users/jonschlinkert/dev/npm-paths/node_modules',
  '/Users/jonschlinkert/dev/node_modules',
  '/usr/local/lib/node_modules',
  '/Users/jonschlinkert/node_modules',
  '/usr/lib/node_modules',
  '/Users/node_modules',
  '/node_modules' ]
```

**Windows**

```js
[ 'C:\\Users\\SERVER\\AppData\\Roaming\\node_modules\\npm',
  'C:\\Program Files\\nodejs\\node_modules',
  'F:\\dev\\npm-paths\\node_modules',
  'F:\\dev\\node_modules',
  'F:\\node_modules' ]
```

## Related projects

* [contains-path](https://www.npmjs.com/package/contains-path): Return true if a file path contains the given path. | [homepage](https://github.com/jonschlinkert/contains-path)
* [global-modules](https://www.npmjs.com/package/global-modules): The directory used by npm for globally installed npm modules. | [homepage](https://github.com/jonschlinkert/global-modules)
* [global-paths](https://www.npmjs.com/package/global-paths): Returns an array of unique "global" directories based on the user's platform and environment. The… [more](https://www.npmjs.com/package/global-paths) | [homepage](https://github.com/jonschlinkert/global-paths)
* [global-prefix](https://www.npmjs.com/package/global-prefix): Get the npm global path prefix. | [homepage](https://github.com/jonschlinkert/global-prefix)
* [look-up](https://www.npmjs.com/package/look-up): Faster drop-in replacement for find-up and findup-sync. | [homepage](https://github.com/jonschlinkert/look-up)
* [resolve-up](https://www.npmjs.com/package/resolve-up): Resolve paths to globally installed npm modules using glob patterns. Very fast, great for getting… [more](https://www.npmjs.com/package/resolve-up) | [homepage](https://github.com/jonschlinkert/resolve-up)

## Running tests

Install dev dependencies:

```sh
$ npm i -d && npm test
```

## Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/jonschlinkert/npm-paths/issues/new).

## Author

**Jon Schlinkert**

+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License

Copyright © 2015 Jon Schlinkert
Released under the MIT license.

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on November 19, 2015._