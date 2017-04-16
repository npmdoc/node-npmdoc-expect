# api documentation for  [expect (v1.20.2)](https://github.com/mjackson/expect#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-expect.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-expect) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-expect.svg)](https://travis-ci.org/npmdoc/node-npmdoc-expect)
#### Write better assertions

[![NPM](https://nodei.co/npm/expect.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/expect)

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
    "version": "1.20.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module expect](#apidoc.module.expect)
1.  [function <span class="apidocSignatureSpan"></span>expect (actual)](#apidoc.element.expect.expect)
1.  [function <span class="apidocSignatureSpan">expect.</span>assert (condition, createMessage)](#apidoc.element.expect.assert)
1.  [function <span class="apidocSignatureSpan">expect.</span>createSpy (fn)](#apidoc.element.expect.createSpy)
1.  [function <span class="apidocSignatureSpan">expect.</span>extend (extension)](#apidoc.element.expect.extend)
1.  [function <span class="apidocSignatureSpan">expect.</span>isSpy (object)](#apidoc.element.expect.isSpy)
1.  [function <span class="apidocSignatureSpan">expect.</span>restoreSpies ()](#apidoc.element.expect.restoreSpies)
1.  [function <span class="apidocSignatureSpan">expect.</span>spyOn (object, methodName)](#apidoc.element.expect.spyOn)
1.  [function <span class="apidocSignatureSpan">expect.</span>toString ()](#apidoc.element.expect.toString)

#### [module expect.expect](#apidoc.module.expect.expect)
1.  [function <span class="apidocSignatureSpan">expect.</span>expect (actual)](#apidoc.element.expect.expect.expect)
1.  [function <span class="apidocSignatureSpan">expect.expect.</span>assert (condition, createMessage)](#apidoc.element.expect.expect.assert)
1.  [function <span class="apidocSignatureSpan">expect.expect.</span>createSpy (fn)](#apidoc.element.expect.expect.createSpy)
1.  [function <span class="apidocSignatureSpan">expect.expect.</span>extend (extension)](#apidoc.element.expect.expect.extend)
1.  [function <span class="apidocSignatureSpan">expect.expect.</span>isSpy (object)](#apidoc.element.expect.expect.isSpy)
1.  [function <span class="apidocSignatureSpan">expect.expect.</span>restoreSpies ()](#apidoc.element.expect.expect.restoreSpies)
1.  [function <span class="apidocSignatureSpan">expect.expect.</span>spyOn (object, methodName)](#apidoc.element.expect.expect.spyOn)



# <a name="apidoc.module.expect"></a>[module expect](#apidoc.module.expect)

#### <a name="apidoc.element.expect.expect"></a>[function <span class="apidocSignatureSpan"></span>expect (actual)](#apidoc.element.expect.expect)
- description and source-code
```javascript
function expect(actual) {
	  return new _Expectation2.default(actual);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.expect.assert"></a>[function <span class="apidocSignatureSpan">expect.</span>assert (condition, createMessage)](#apidoc.element.expect.assert)
- description and source-code
```javascript
function assert(condition, createMessage) {
  for (var _len = arguments.length, extraArgs = Array(_len > 2 ? _len - 2 : 0), _key = 2; _key < _len; _key++) {
    extraArgs[_key - 2] = arguments[_key];
  }

  if (condition) return;

  var message = typeof createMessage === 'string' ? formatString(createMessage, extraArgs) : createMessage(extraArgs);

  throw new Error(message);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.expect.createSpy"></a>[function <span class="apidocSignatureSpan">expect.</span>createSpy (fn)](#apidoc.element.expect.createSpy)
- description and source-code
```javascript
function createSpy(fn) {
  var restore = arguments.length <= 1 || arguments[1] === undefined ? noop : arguments[1];

  if (fn == null) fn = noop;

  (0, _assert2.default)((0, _TestUtils.isFunction)(fn), 'createSpy needs a function');

  var targetFn = void 0,
      thrownValue = void 0,
      returnValue = void 0,
      spy = void 0;

  function spyLogic() {
    spy.calls.push({
      context: this,
      arguments: Array.prototype.slice.call(arguments, 0)
    });

    if (targetFn) return targetFn.apply(this, arguments);

    if (thrownValue) throw thrownValue;

    return returnValue;
  }

  if (supportsConfigurableFnLength) {
    spy = Object.defineProperty(spyLogic, 'length', { value: fn.length, writable: false, enumerable: false, configurable: true });
  } else {
    spy = new Function('spy', 'return function(' + // eslint-disable-line no-new-func
    [].concat(_toConsumableArray(Array(fn.length))).map(function (_, i) {
      return '_' + i;
    }).join(',') + ') {\n      return spy.apply(this, arguments)\n    }')(spyLogic);
  }

  spy.calls = [];

  spy.andCall = function (otherFn) {
    targetFn = otherFn;
    return spy;
  };

  spy.andCallThrough = function () {
    return spy.andCall(fn);
  };

  spy.andThrow = function (value) {
    thrownValue = value;
    return spy;
  };

  spy.andReturn = function (value) {
    returnValue = value;
    return spy;
  };

  spy.getLastCall = function () {
    return spy.calls[spy.calls.length - 1];
  };

  spy.reset = function () {
    spy.calls = [];
  };

  spy.restore = spy.destroy = restore;

  spy.__isSpy = true;

  spies.push(spy);

  return spy;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.expect.extend"></a>[function <span class="apidocSignatureSpan">expect.</span>extend (extension)](#apidoc.element.expect.extend)
- description and source-code
```javascript
function extend(extension) {
  if (Extensions.indexOf(extension) === -1) {
    Extensions.push(extension);

    for (var p in extension) {
      if (extension.hasOwnProperty(p)) _Expectation2.default.prototype[p] = extension[p];
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.expect.isSpy"></a>[function <span class="apidocSignatureSpan">expect.</span>isSpy (object)](#apidoc.element.expect.isSpy)
- description and source-code
```javascript
function isSpy(object) {
  return object && object.__isSpy === true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.expect.restoreSpies"></a>[function <span class="apidocSignatureSpan">expect.</span>restoreSpies ()](#apidoc.element.expect.restoreSpies)
- description and source-code
```javascript
function restoreSpies() {
  for (var i = spies.length - 1; i >= 0; i--) {
    spies[i].restore();
  }spies = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.expect.spyOn"></a>[function <span class="apidocSignatureSpan">expect.</span>spyOn (object, methodName)](#apidoc.element.expect.spyOn)
- description and source-code
```javascript
function spyOn(object, methodName) {
  var original = object[methodName];

  if (!isSpy(original)) {
    (0, _assert2.default)((0, _TestUtils.isFunction)(original), 'Cannot spyOn the %s property; it is not a function', methodName
);

    object[methodName] = createSpy(original, function () {
      object[methodName] = original;
    });
  }

  return object[methodName];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.expect.toString"></a>[function <span class="apidocSignatureSpan">expect.</span>toString ()](#apidoc.element.expect.toString)
- description and source-code
```javascript
toString = function () {
    return toString;
}
```
- example usage
```shell
...
	}

	function checked (length) {
	  // Note: cannot use 'length < kMaxLength' here because that fails when
	  // length is NaN (which is otherwise coerced to zero.)
	  if (length >= kMaxLength()) {
	    throw new RangeError('Attempt to allocate Buffer larger than maximum ' +
	                         'size: 0x' + kMaxLength().toString(16) + ' bytes')
	  }
	  return length | 0
	}

	function SlowBuffer (subject, encoding) {
	  if (!(this instanceof SlowBuffer)) return new SlowBuffer(subject, encoding)
...
```



# <a name="apidoc.module.expect.expect"></a>[module expect.expect](#apidoc.module.expect.expect)

#### <a name="apidoc.element.expect.expect.expect"></a>[function <span class="apidocSignatureSpan">expect.</span>expect (actual)](#apidoc.element.expect.expect.expect)
- description and source-code
```javascript
function expect(actual) {
	  return new _Expectation2.default(actual);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.expect.expect.assert"></a>[function <span class="apidocSignatureSpan">expect.expect.</span>assert (condition, createMessage)](#apidoc.element.expect.expect.assert)
- description and source-code
```javascript
function assert(condition, createMessage) {
	  for (var _len = arguments.length, extraArgs = Array(_len > 2 ? _len - 2 : 0), _key = 2; _key < _len; _key++) {
	    extraArgs[_key - 2] = arguments[_key];
	  }

	  if (condition) return;

	  var message = typeof createMessage === 'string' ? formatString(createMessage, extraArgs) : createMessage(extraArgs);

	  throw new Error(message);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.expect.expect.createSpy"></a>[function <span class="apidocSignatureSpan">expect.expect.</span>createSpy (fn)](#apidoc.element.expect.expect.createSpy)
- description and source-code
```javascript
function createSpy(fn) {
	  var restore = arguments.length <= 1 || arguments[1] === undefined ? noop : arguments[1];

	  if (fn == null) fn = noop;

	  (0, _assert2.default)((0, _TestUtils.isFunction)(fn), 'createSpy needs a function');

	  var targetFn = void 0,
	      thrownValue = void 0,
	      returnValue = void 0,
	      spy = void 0;

	  function spyLogic() {
	    spy.calls.push({
	      context: this,
	      arguments: Array.prototype.slice.call(arguments, 0)
	    });

	    if (targetFn) return targetFn.apply(this, arguments);

	    if (thrownValue) throw thrownValue;

	    return returnValue;
	  }

	  if (supportsConfigurableFnLength) {
	    spy = Object.defineProperty(spyLogic, 'length', { value: fn.length, writable: false, enumerable: false, configurable: true });
	  } else {
	    spy = new Function('spy', 'return function(' + // eslint-disable-line no-new-func
	    [].concat(_toConsumableArray(Array(fn.length))).map(function (_, i) {
	      return '_' + i;
	    }).join(',') + ') {\n      return spy.apply(this, arguments)\n    }')(spyLogic);
	  }

	  spy.calls = [];

	  spy.andCall = function (otherFn) {
	    targetFn = otherFn;
	    return spy;
	  };

	  spy.andCallThrough = function () {
	    return spy.andCall(fn);
	  };

	  spy.andThrow = function (value) {
	    thrownValue = value;
	    return spy;
	  };

	  spy.andReturn = function (value) {
	    returnValue = value;
	    return spy;
	  };

	  spy.getLastCall = function () {
	    return spy.calls[spy.calls.length - 1];
	  };

	  spy.reset = function () {
	    spy.calls = [];
	  };

	  spy.restore = spy.destroy = restore;

	  spy.__isSpy = true;

	  spies.push(spy);

	  return spy;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.expect.expect.extend"></a>[function <span class="apidocSignatureSpan">expect.expect.</span>extend (extension)](#apidoc.element.expect.expect.extend)
- description and source-code
```javascript
function extend(extension) {
	  if (Extensions.indexOf(extension) === -1) {
	    Extensions.push(extension);

	    for (var p in extension) {
	      if (extension.hasOwnProperty(p)) _Expectation2.default.prototype[p] = extension[p];
	    }
	  }
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.expect.expect.isSpy"></a>[function <span class="apidocSignatureSpan">expect.expect.</span>isSpy (object)](#apidoc.element.expect.expect.isSpy)
- description and source-code
```javascript
function isSpy(object) {
	  return object && object.__isSpy === true;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.expect.expect.restoreSpies"></a>[function <span class="apidocSignatureSpan">expect.expect.</span>restoreSpies ()](#apidoc.element.expect.expect.restoreSpies)
- description and source-code
```javascript
function restoreSpies() {
	  for (var i = spies.length - 1; i >= 0; i--) {
	    spies[i].restore();
	  }spies = [];
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.expect.expect.spyOn"></a>[function <span class="apidocSignatureSpan">expect.expect.</span>spyOn (object, methodName)](#apidoc.element.expect.expect.spyOn)
- description and source-code
```javascript
function spyOn(object, methodName) {
	  var original = object[methodName];

	  if (!isSpy(original)) {
	    (0, _assert2.default)((0, _TestUtils.isFunction)(original), 'Cannot spyOn the %s property; it is not a function', methodName
);

	    object[methodName] = createSpy(original, function () {
	      object[methodName] = original;
	    });
	  }

	  return object[methodName];
	}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
