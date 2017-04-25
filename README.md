# npmdoc-expect

#### basic api documentation for  [expect (v1.20.2)](https://github.com/mjackson/expect#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-expect.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-expect) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-expect.svg)](https://travis-ci.org/npmdoc/node-npmdoc-expect)

#### Write better assertions

[![NPM](https://nodei.co/npm/expect.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/expect)

- [https://npmdoc.github.io/node-npmdoc-expect/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-expect/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-expect/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-expect/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-expect/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-expect/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Michael Jackson"
    },
    "babel": {
        "presets": [
            "es2015"
        ]
    },
    "bugs": {
        "url": "https://github.com/mjackson/expect/issues"
    },
    "dependencies": {
        "define-properties": "~1.1.2",
        "has": "^1.0.1",
        "is-equal": "^1.5.1",
        "is-regex": "^1.0.3",
        "object-inspect": "^1.1.0",
        "object-keys": "^1.0.9",
        "tmatch": "^2.0.1"
    },
    "description": "Write better assertions",
    "devDependencies": {
        "babel-cli": "^6.6.5",
        "babel-eslint": "^6.0.0",
        "babel-loader": "^6.2.4",
        "babel-preset-es2015": "^6.6.0",
        "eslint": "^2.5.1",
        "eslint-config-airbnb": "^9.0.1",
        "eslint-plugin-import": "^1.7.0",
        "eslint-plugin-jsx-a11y": "^1.2.0",
        "eslint-plugin-react": "^5.1.1",
        "gzip-size": "^3.0.0",
        "in-publish": "^2.0.0",
        "karma": "^0.13.22",
        "karma-browserstack-launcher": "^1.0.0",
        "karma-chrome-launcher": "^1.0.1",
        "karma-mocha": "^1.0.1",
        "karma-mocha-reporter": "^2.0.0",
        "karma-sourcemap-loader": "^0.3.7",
        "karma-webpack": "^1.7.0",
        "mocha": "^2.5.3",
        "pretty-bytes": "^3.0.1",
        "readline-sync": "^1.4.1",
        "rimraf": "^2.5.2",
        "webpack": "^1.12.14"
    },
    "directories": {},
    "dist": {
        "shasum": "d458fe4c56004036bae3232416a3f6361f04f965",
        "tarball": "https://registry.npmjs.org/expect/-/expect-1.20.2.tgz"
    },
    "files": [
        "lib",
        "umd"
    ],
    "gitHead": "8301ca9b742b86631c6d3df282f3a21138ac50aa",
    "homepage": "https://github.com/mjackson/expect#readme",
    "keywords": [
        "expect",
        "assert",
        "test",
        "spec"
    ],
    "license": "MIT",
    "main": "lib",
    "maintainers": [
        {
            "name": "ljharb"
        },
        {
            "name": "mjackson"
        }
    ],
    "name": "expect",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mjackson/expect.git"
    },
    "scripts": {
        "build": "node ./scripts/build.js",
        "build-lib": "rimraf lib && babel ./modules -d lib --ignore '__tests__'",
        "build-min": "webpack -p modules/index.js umd/expect.min.js",
        "build-umd": "webpack modules/index.js umd/expect.js",
        "lint": "eslint modules",
        "prepublish": "node ./scripts/build.js",
        "release": "node ./scripts/release.js",
        "test": "npm run lint && karma start"
    },
    "version": "1.20.2",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
