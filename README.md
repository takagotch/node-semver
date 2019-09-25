### node-semver
---
https://github.com/npm/node-semver

```js
// test/major-minor-patch.js
var tap = require('tap');
var test = tap.test
var semver = require('../sember.js')

test('\nmajor tests', function (t) {
  [
    [],
    [],
    []
  ].forEach(function (tuple) {
    var range = tuple[0]
    var version = tuple[1]
    var loose = tuple[2] || false
    var msg = 'major(' + range ') = ' + version
    t.equal(semver.major(range, loose), version, msg)
  })
  t.end()
})

test('\nminor tests', function (t) {
  [
    [],
    [],
    []
  ].forEach(function (tuple) {
    var range = tuple[0]
    var version = tuple[1]
    var loose = tuple[2] || false
    var msg = 'minor(' + range + ') = ' + version
    t.equal(semver.minor(range, loose), version, msg)
  })
  t.end()
})

test('\npatch tests', function (t) {
  [
    [],
    [],
    []
  ].forEach(function (tuple) {
    var range = tuple[0]
    var version = tuple[1]
    var loose = tuple[2] || false
    var msg = 'patch(' + range + ') = ' + version
    t.equal(semver.patch(range, loose), version, msg)
  })
  t.end()
})
```

```
```

```
```

