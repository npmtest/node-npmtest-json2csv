# npmtest-json2csv

#### test coverage for  [json2csv (v3.7.3)](https://github.com/zemirco/json2csv#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-json2csv.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-json2csv) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-json2csv.svg)](https://travis-ci.org/npmtest/node-npmtest-json2csv)

#### Convert JSON to CSV

[![NPM](https://nodei.co/npm/json2csv.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/json2csv)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-json2csv/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-json2csv/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-json2csv/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-json2csv/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-json2csv/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-json2csv/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-json2csv/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-json2csv/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-json2csv/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-json2csv/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-json2csv/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-json2csv/build/test-report.html](https://npmtest.github.io/node-npmtest-json2csv/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-json2csv/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-json2csv/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-json2csv/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-json2csv/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-json2csv/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-json2csv/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-json2csv/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-json2csv/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mirco Zeiss"
    },
    "bin": {
        "json2csv": "./bin/json2csv.js"
    },
    "bugs": {
        "url": "https://github.com/zemirco/json2csv/issues"
    },
    "dependencies": {
        "cli-table": "^0.3.1",
        "commander": "^2.8.1",
        "debug": "^2.2.0",
        "flat": "^2.0.0",
        "lodash.clonedeep": "^4.3.0",
        "lodash.flatten": "^4.2.0",
        "lodash.get": "^4.3.0",
        "lodash.set": "^4.3.0",
        "lodash.uniq": "^4.3.0",
        "path-is-absolute": "^1.0.0"
    },
    "description": "Convert JSON to CSV",
    "devDependencies": {
        "async": "^2.0.1",
        "docpress": "^0.7.0",
        "eslint": "^3.3.1",
        "git-update-ghpages": "^1.3.0",
        "in-publish": "^2.0.0",
        "istanbul": "^0.4.3",
        "standard-version": "^4.0.0",
        "tap-spec": "^4.1.0",
        "tape": "^4.0.0",
        "webpack": "^1.13.1"
    },
    "directories": {},
    "dist": {
        "shasum": "dacfdfa7fb0c1b1b163868dc75f3902d023354ec",
        "tarball": "https://registry.npmjs.org/json2csv/-/json2csv-3.7.3.tgz"
    },
    "gitHead": "19e77972578e73748baa0936c1e200be41b906a3",
    "homepage": "https://github.com/zemirco/json2csv#readme",
    "keywords": [
        "json",
        "to",
        "csv",
        "export",
        "convert",
        "parse"
    ],
    "license": "MIT",
    "main": "./lib/json2csv.js",
    "maintainers": [
        {
            "name": "azhang"
        },
        {
            "name": "knownasilya"
        },
        {
            "name": "zemirco"
        }
    ],
    "name": "json2csv",
    "optionalDependencies": {},
    "preferGlobal": "true",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/zemirco/json2csv.git"
    },
    "scripts": {
        "before:publish": "npm test && npm run build && npm run deploy:docs && npm run release",
        "build": "webpack",
        "deploy:docs": "docpress b && git-update-ghpages zemirco/json2csv _docpress",
        "prepublish": "in-publish && npm run before:publish || not-in-publish",
        "release": "standard-version",
        "test": "node test | tap-spec",
        "test-coverage": "istanbul cover test/index.js --report lcovonly | tap-spec"
    },
    "version": "3.7.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
