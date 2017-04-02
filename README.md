# api documentation for  [chance (v1.0.6)](http://chancejs.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-chance.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-chance) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-chance.svg)](https://travis-ci.org/npmdoc/node-npmdoc-chance)
#### Chance - Utility library to generate anything random

[![NPM](https://nodei.co/npm/chance.png?downloads=true)](https://www.npmjs.com/package/chance)

[![apidoc](https://npmdoc.github.io/node-npmdoc-chance/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-chance_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-chance/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-chance/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Victor Quinn",
        "email": "mail@victorquinn.com"
    },
    "bugs": {
        "url": "https://github.com/chancejs/chancejs/issues"
    },
    "dependencies": {},
    "description": "Chance - Utility library to generate anything random",
    "devDependencies": {
        "coveralls": "^2.11.2",
        "grunt": "0.4.5",
        "grunt-contrib-jshint": "^0.11.0",
        "grunt-contrib-uglify": "^0.9.2",
        "grunt-contrib-watch": "0.6.1",
        "grunt-js-test": "git://github.com/victorquinn/grunt-js-test.git#ffc580375f0ff7b496026ab87b4a9666992d2f33",
        "grunt-shell": "^1.1.2",
        "istanbul": "^0.3.13",
        "line-by-line": "^0.1.3",
        "minimatch": "^2.0.4",
        "mocha-lcov-reporter": "0.0.2",
        "underscore": "^1.8.3"
    },
    "directories": {},
    "dist": {
        "shasum": "4734f62d02b738cdc2882d8b5d41f89af49e7bfd",
        "tarball": "https://registry.npmjs.org/chance/-/chance-1.0.6.tgz"
    },
    "gitHead": "330656d5e0316a0be515d9125f81372a5d3f89a9",
    "github": "https://github.com/chancejs/chancejs",
    "homepage": "http://chancejs.com",
    "jam": {
        "main": "chance.js"
    },
    "keywords": [
        "chance",
        "random",
        "generator",
        "test",
        "mersenne",
        "name",
        "address",
        "dice"
    ],
    "license": "MIT",
    "main": "./chance.js",
    "maintainers": [
        {
            "name": "victorquinn",
            "email": "mail@victorquinn.com"
        }
    ],
    "name": "chance",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/chancejs/chancejs.git"
    },
    "scripts": {
        "test": "grunt test-ci"
    },
    "spm": {
        "main": "chance.js",
        "ignore": [
            "test"
        ]
    },
    "version": "1.0.6"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module chance](#apidoc.module.chance)
1.  [function <span class="apidocSignatureSpan">chance.</span>Chance (seed)](#apidoc.element.chance.Chance)



# <a name="apidoc.module.chance"></a>[module chance](#apidoc.module.chance)

#### <a name="apidoc.element.chance.Chance"></a>[function <span class="apidocSignatureSpan">chance.</span>Chance (seed)](#apidoc.element.chance.Chance)
- description and source-code
```javascript
function Chance(seed) {
    if (!(this instanceof Chance)) {
        return seed == null ? new Chance() : new Chance(seed);
    }

    // if user has provided a function, use that as the generator
    if (typeof seed === 'function') {
        this.random = seed;
        return this;
    }

    if (arguments.length) {
        // set a starting value of zero so we can add to it
        this.seed = 0;
    }

    // otherwise, leave this.seed blank so that MT will receive a blank

    for (var i = 0; i < arguments.length; i++) {
        var seedling = 0;
        if (Object.prototype.toString.call(arguments[i]) === '[object String]') {
            for (var j = 0; j < arguments[i].length; j++) {
                // create a numeric hash for each argument, add to seedling
                var hash = 0;
                for (var k = 0; k < arguments[i].length; k++) {
                    hash = arguments[i].charCodeAt(k) + (hash << 6) + (hash << 16) - hash;
                }
                seedling += hash;
            }
        } else {
            seedling = arguments[i];
        }
        this.seed += (arguments.length - i) * seedling;
    }

    // If no generator function was provided, use our MT
    this.mt = this.mersenne_twister(this.seed);
    this.bimd5 = this.blueimp_md5();
    this.random = function () {
        return this.mt.random(this.seed);
    };

    return this;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
