[![Build Status](https://travis-ci.org/kaelzhang/ignore-glob.svg?branch=master)](https://travis-ci.org/kaelzhang/ignore-glob)
<!-- optional appveyor tst
[![Windows Build Status](https://ci.appveyor.com/api/projects/status/github/kaelzhang/ignore-glob?branch=master&svg=true)](https://ci.appveyor.com/project/kaelzhang/ignore-glob)
-->
<!-- optional npm version
[![NPM version](https://badge.fury.io/js/ignore-glob.svg)](http://badge.fury.io/js/ignore-glob)
-->
<!-- optional npm downloads
[![npm module downloads per month](http://img.shields.io/npm/dm/ignore-glob.svg)](https://www.npmjs.org/package/ignore-glob)
-->
<!-- optional dependency status
[![Dependency Status](https://david-dm.org/kaelzhang/ignore-glob.svg)](https://david-dm.org/kaelzhang/ignore-glob)
-->

# ignore-glob

<!-- description -->

## Install

```sh
$ npm install ignore-glob --save
```

## Usage

```js
const glob = require('ignore-glob')

glob({
  cwd: cwd,
  ignore: [
    '/*.js',
    '*.db'
  ]
}, (err, files) => {

})
```

## glob(options, callback)

- **options** `Object` The `options` of ignore-glob is much the same as `node-glob` except for:
  - ignore `String=|Array.<String>=` ignore patterns
  - ignoreFile `path` path to the `.gitignore` or any ignore files according to gitignore spec.

## glob.sync(options)

## License

MIT
