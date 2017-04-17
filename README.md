# api documentation for  [tap (v10.3.2)](http://node-tap.org/)  [![npm package](https://img.shields.io/npm/v/npmdoc-tap.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-tap) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-tap.svg)](https://travis-ci.org/npmdoc/node-npmdoc-tap)
#### A Test-Anything-Protocol library

[![NPM](https://nodei.co/npm/tap.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/tap)

- [https://npmdoc.github.io/node-npmdoc-tap/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-tap/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-tap/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-tap/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-tap/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-tap/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Isaac Z. Schlueter",
        "url": "http://blog.izs.me"
    },
    "bin": {
        "tap": "bin/run.js"
    },
    "bugs": {
        "url": "https://github.com/tapjs/node-tap/issues"
    },
    "config": {
        "nyc": {
            "exclude": [
                "node_modules/**",
                "test/**"
            ]
        }
    },
    "dependencies": {
        "bind-obj-methods": "^1.0.0",
        "bluebird": "^3.3.1",
        "clean-yaml-object": "^0.1.0",
        "color-support": "^1.1.0",
        "coveralls": "^2.11.2",
        "deeper": "^2.1.0",
        "foreground-child": "^1.3.3",
        "fs-exists-cached": "^1.0.0",
        "function-loop": "^1.0.1",
        "glob": "^7.0.0",
        "isexe": "^1.0.0",
        "js-yaml": "^3.3.1",
        "nyc": "^10.0.0",
        "only-shallow": "^1.0.2",
        "opener": "^1.4.1",
        "os-homedir": "1.0.1",
        "own-or": "^1.0.0",
        "own-or-env": "^1.0.0",
        "readable-stream": "^2.0.2",
        "signal-exit": "^3.0.0",
        "source-map-support": "^0.4.3",
        "stack-utils": "^1.0.0",
        "tap-mocha-reporter": "^3.0.1",
        "tap-parser": "^5.3.1",
        "tmatch": "^3.0.0",
        "trivial-deferred": "^1.0.1",
        "yapool": "^1.0.0"
    },
    "description": "A Test-Anything-Protocol library",
    "devDependencies": {
        "mkdirp": "^0.5.1",
        "rimraf": "^2.5.4",
        "standard": "^7.1.0",
        "which": "^1.1.1"
    },
    "directories": {},
    "dist": {
        "shasum": "77982f08368d8b1803a3b0ab5fc300e1817f31e7",
        "tarball": "https://registry.npmjs.org/tap/-/tap-10.3.2.tgz"
    },
    "engines": {
        "node": ">=0.8"
    },
    "files": [
        "bin/*",
        "lib/*"
    ],
    "gitHead": "fa3da919ec08dd4b88655f6089b2873f77b745c7",
    "homepage": "http://node-tap.org/",
    "keywords": [
        "assert",
        "test",
        "tap"
    ],
    "license": "ISC",
    "main": "lib/tap.js",
    "maintainers": [
        {
            "name": "isaacs"
        }
    ],
    "name": "tap",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tapjs/node-tap.git"
    },
    "scripts": {
        "postpublish": "git push origin --all; git push origin --tags",
        "posttest": "standard lib test",
        "postversion": "npm publish",
        "preversion": "npm test",
        "regen-fixtures": "node scripts/generate-test-test.js test/test/*.js",
        "smoke": "node bin/run.js --node-arg=test/test.js test/test/*.js -j2",
        "t": "node bin/run.js test/*.* -sfails.txt",
        "test": "node bin/run.js test/*.* --coverage -t3600 -sfails"
    },
    "version": "10.3.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
