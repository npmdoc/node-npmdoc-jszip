# npmdoc-jszip

#### basic api documentation for  [jszip (v3.1.3)](https://github.com/Stuk/jszip#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-jszip.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jszip) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jszip.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jszip)

#### Create, read and edit .zip files with Javascript http://stuartk.com/jszip

[![NPM](https://nodei.co/npm/jszip.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/jszip)

- [https://npmdoc.github.io/node-npmdoc-jszip/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-jszip/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jszip/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jszip/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jszip/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jszip/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Stuart Knightley"
    },
    "browser": {
        "readable-stream": "./lib/readable-stream-browser.js"
    },
    "bugs": {
        "url": "https://github.com/Stuk/jszip/issues"
    },
    "contributors": [
        {
            "name": "Franz Buchinger"
        },
        {
            "name": "António Afonso"
        },
        {
            "name": "David Duponchel"
        },
        {
            "name": "yiminghe"
        }
    ],
    "dependencies": {
        "core-js": "~2.3.0",
        "es6-promise": "~3.0.2",
        "lie": "~3.1.0",
        "pako": "~1.0.2",
        "readable-stream": "~2.0.6"
    },
    "description": "Create, read and edit .zip files with Javascript http://stuartk.com/jszip",
    "devDependencies": {
        "browserify": "~13.0.0",
        "grunt": "~0.4.1",
        "grunt-browserify": "~5.0.0",
        "grunt-cli": "~1.1.0",
        "grunt-contrib-connect": "1.0.0",
        "grunt-contrib-jshint": "~1.0.0",
        "grunt-contrib-qunit": "~1.2.0",
        "grunt-contrib-uglify": "~1.0.0",
        "grunt-saucelabs": "~8.6.2",
        "jshint": "~2.9.1",
        "jszip-utils": "~0.0.2",
        "package-json-versionify": "~1.0.2",
        "qunit-cli": "~0.2.0",
        "qunitjs": "~1.23.0",
        "tmp": "0.0.28"
    },
    "directories": {},
    "dist": {
        "shasum": "8a920403b2b1651c0fc126be90192d9080957c37",
        "tarball": "https://registry.npmjs.org/jszip/-/jszip-3.1.3.tgz"
    },
    "gitHead": "a5b4343ae5db14dae08487262165e101a0e4c9c4",
    "homepage": "https://github.com/Stuk/jszip#readme",
    "keywords": [
        "zip",
        "deflate",
        "inflate"
    ],
    "license": "(MIT OR GPL-3.0)",
    "main": "./lib/index",
    "maintainers": [
        {
            "name": "cwmma"
        },
        {
            "name": "dduponchel"
        },
        {
            "name": "stuk"
        }
    ],
    "name": "jszip",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/Stuk/jszip.git"
    },
    "scripts": {
        "lint": "grunt jshint",
        "test": "npm run test-node && npm run test-browser",
        "test-browser": "grunt build && grunt test",
        "test-node": "qunit-cli -c test/helpers/test-utils.js test/helpers/node-test-utils.js test/asserts/*.js"
    },
    "version": "3.1.3",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
