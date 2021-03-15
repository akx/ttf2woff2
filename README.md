[//]: # ( )
[//]: # (This file is automatically generated by a `metapak`)
[//]: # (module. Do not change it  except between the)
[//]: # (`content:start/end` flags, your changes would)
[//]: # (be overridden.)
[//]: # ( )
# ttf2woff2
> Convert TTF files to WOFF2 ones.

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/nfroidure/ttf2woff2/blob/master/LICENSE)
[![Coverage Status](https://coveralls.io/repos/github/git@github.com:nfroidure/ttf2woff2.git/badge.svg?branch=master)](https://coveralls.io/github/git@github.com:nfroidure/ttf2woff2.git?branch=master)
[![NPM version](https://badge.fury.io/js/ttf2woff2.svg)](https://npmjs.org/package/ttf2woff2)
[![Dependency Status](https://david-dm.org/nfroidure/ttf2woff2.svg)](https://david-dm.org/nfroidure/ttf2woff2)
[![devDependency Status](https://david-dm.org/nfroidure/ttf2woff2/dev-status.svg)](https://david-dm.org/nfroidure/ttf2woff2#info=devDependencies)
[![Package Quality](https://npm.packagequality.com/shield/ttf2woff2.svg)](https://packagequality.com/#?package=ttf2woff2)


[//]: # (::contents:start)

This is a NodeJS wrapper for the Google [WOFF2](https://github.com/google/woff2)
project. If the C++ wrapper compilation fail, it
[fallbacks to an Emscripten build](http://insertafter.com/en/blog/native-node-module.html).

## Usage

### CLI

Install `ttf2woff2` globally, then:

```sh
cat font.ttf | ttf2woff2 > font.woff2
```

### API

```js
var fs = require('fs');
var ttf2woff2 = require('ttf2woff2');

var input = fs.readFileSync('font.ttf');

fs.writeFileSync('font.woff2', ttf2woff2(input));
```

## Contributing

Feel free to push your code if you agree with publishing under the MIT license.

[//]: # (::contents:end)

# Authors
- [Nicolas Froidure](https://insertafter.com/en/index.html)
- [Anders Kaseorg](mailto:andersk@mit.edu)

# License
[MIT](https://github.com/nfroidure/ttf2woff2/blob/master/LICENSE)
