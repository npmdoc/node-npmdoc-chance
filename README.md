# api documentation for  [chance (v1.0.6)](http://chancejs.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-chance.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-chance) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-chance.svg)](https://travis-ci.org/npmdoc/node-npmdoc-chance)
#### Chance - Utility library to generate anything random

[![NPM](https://nodei.co/npm/chance.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/chance)

[![apidoc](https://npmdoc.github.io/node-npmdoc-chance/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-chance/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-chance/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-chance/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Victor Quinn"
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
            "name": "victorquinn"
        }
    ],
    "name": "chance",
    "optionalDependencies": {},
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
1.  [function <span class="apidocSignatureSpan"></span>chance (seed)](#apidoc.element.chance.chance)
1.  [function <span class="apidocSignatureSpan">chance.</span>Chance (seed)](#apidoc.element.chance.Chance)
1.  [function <span class="apidocSignatureSpan">chance.</span>toString ()](#apidoc.element.chance.toString)
1.  object <span class="apidocSignatureSpan">chance.</span>Chance.prototype

#### [module chance.Chance](#apidoc.module.chance.Chance)
1.  [function <span class="apidocSignatureSpan">chance.</span>Chance (seed)](#apidoc.element.chance.Chance.Chance)

#### [module chance.Chance.prototype](#apidoc.module.chance.Chance.prototype)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>HIDN ()](#apidoc.element.chance.Chance.prototype.HIDN)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>address (options)](#apidoc.element.chance.Chance.prototype.address)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>age (options)](#apidoc.element.chance.Chance.prototype.age)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>altitude (options)](#apidoc.element.chance.Chance.prototype.altitude)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>ampm ()](#apidoc.element.chance.Chance.prototype.ampm)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>android_id ()](#apidoc.element.chance.Chance.prototype.android_id)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>apple_token ()](#apidoc.element.chance.Chance.prototype.apple_token)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>areacode (options)](#apidoc.element.chance.Chance.prototype.areacode)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>avatar (options)](#apidoc.element.chance.Chance.prototype.avatar)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>bb_pin ()](#apidoc.element.chance.Chance.prototype.bb_pin)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>birthday (options)](#apidoc.element.chance.Chance.prototype.birthday)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>blueimp_md5 ()](#apidoc.element.chance.Chance.prototype.blueimp_md5)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>bool (options)](#apidoc.element.chance.Chance.prototype.bool)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>capitalize (word)](#apidoc.element.chance.Chance.prototype.capitalize)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>cc (options)](#apidoc.element.chance.Chance.prototype.cc)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>cc_type (options)](#apidoc.element.chance.Chance.prototype.cc_type)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>cc_types ()](#apidoc.element.chance.Chance.prototype.cc_types)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>cf (options)](#apidoc.element.chance.Chance.prototype.cf)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>character (options)](#apidoc.element.chance.Chance.prototype.character)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>city ()](#apidoc.element.chance.Chance.prototype.city)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>cnpj ()](#apidoc.element.chance.Chance.prototype.cnpj)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>color (options)](#apidoc.element.chance.Chance.prototype.color)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>coordinates (options)](#apidoc.element.chance.Chance.prototype.coordinates)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>counties (options)](#apidoc.element.chance.Chance.prototype.counties)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>countries ()](#apidoc.element.chance.Chance.prototype.countries)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>country (options)](#apidoc.element.chance.Chance.prototype.country)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>county (options)](#apidoc.element.chance.Chance.prototype.county)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>cpf (options)](#apidoc.element.chance.Chance.prototype.cpf)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>currency ()](#apidoc.element.chance.Chance.prototype.currency)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>currency_pair (returnAsString)](#apidoc.element.chance.Chance.prototype.currency_pair)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>currency_types ()](#apidoc.element.chance.Chance.prototype.currency_types)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d10 ()](#apidoc.element.chance.Chance.prototype.d10)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d100 ()](#apidoc.element.chance.Chance.prototype.d100)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d12 ()](#apidoc.element.chance.Chance.prototype.d12)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d20 ()](#apidoc.element.chance.Chance.prototype.d20)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d30 ()](#apidoc.element.chance.Chance.prototype.d30)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d4 ()](#apidoc.element.chance.Chance.prototype.d4)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d6 ()](#apidoc.element.chance.Chance.prototype.d6)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d8 ()](#apidoc.element.chance.Chance.prototype.d8)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>date (options)](#apidoc.element.chance.Chance.prototype.date)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>depth (options)](#apidoc.element.chance.Chance.prototype.depth)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>dollar (options)](#apidoc.element.chance.Chance.prototype.dollar)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>domain (options)](#apidoc.element.chance.Chance.prototype.domain)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>email (options)](#apidoc.element.chance.Chance.prototype.email)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>euro (options)](#apidoc.element.chance.Chance.prototype.euro)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>exp (options)](#apidoc.element.chance.Chance.prototype.exp)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>exp_month (options)](#apidoc.element.chance.Chance.prototype.exp_month)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>exp_year ()](#apidoc.element.chance.Chance.prototype.exp_year)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>fbid ()](#apidoc.element.chance.Chance.prototype.fbid)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>file (options)](#apidoc.element.chance.Chance.prototype.file)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>first (options)](#apidoc.element.chance.Chance.prototype.first)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>floating (options)](#apidoc.element.chance.Chance.prototype.floating)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>gender (options)](#apidoc.element.chance.Chance.prototype.gender)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>geohash (options)](#apidoc.element.chance.Chance.prototype.geohash)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>geojson (options)](#apidoc.element.chance.Chance.prototype.geojson)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>get (name)](#apidoc.element.chance.Chance.prototype.get)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>google_analytics ()](#apidoc.element.chance.Chance.prototype.google_analytics)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>guid (options)](#apidoc.element.chance.Chance.prototype.guid)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>hammertime (options)](#apidoc.element.chance.Chance.prototype.hammertime)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>hash (options)](#apidoc.element.chance.Chance.prototype.hash)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>hashtag ()](#apidoc.element.chance.Chance.prototype.hashtag)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>hex (options)](#apidoc.element.chance.Chance.prototype.hex)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>hour (options)](#apidoc.element.chance.Chance.prototype.hour)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>iban ()](#apidoc.element.chance.Chance.prototype.iban)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>integer (options)](#apidoc.element.chance.Chance.prototype.integer)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>ip ()](#apidoc.element.chance.Chance.prototype.ip)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>ipv6 ()](#apidoc.element.chance.Chance.prototype.ipv6)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>israelId ()](#apidoc.element.chance.Chance.prototype.israelId)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>it_vat ()](#apidoc.element.chance.Chance.prototype.it_vat)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>klout ()](#apidoc.element.chance.Chance.prototype.klout)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>last (options)](#apidoc.element.chance.Chance.prototype.last)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>latitude (options)](#apidoc.element.chance.Chance.prototype.latitude)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>longitude (options)](#apidoc.element.chance.Chance.prototype.longitude)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>luhn_calculate (num)](#apidoc.element.chance.Chance.prototype.luhn_calculate)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>luhn_check (num)](#apidoc.element.chance.Chance.prototype.luhn_check)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>mac_address (options)](#apidoc.element.chance.Chance.prototype.mac_address)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>md5 (options)](#apidoc.element.chance.Chance.prototype.md5)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>mersenne_twister (seed)](#apidoc.element.chance.Chance.prototype.mersenne_twister)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>millisecond ()](#apidoc.element.chance.Chance.prototype.millisecond)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>minute (options)](#apidoc.element.chance.Chance.prototype.minute)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>mixin (obj)](#apidoc.element.chance.Chance.prototype.mixin)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>month (options)](#apidoc.element.chance.Chance.prototype.month)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>months ()](#apidoc.element.chance.Chance.prototype.months)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>mrz (options)](#apidoc.element.chance.Chance.prototype.mrz)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>n (fn, n)](#apidoc.element.chance.Chance.prototype.n)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>name (options)](#apidoc.element.chance.Chance.prototype.name)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>name_prefix (options)](#apidoc.element.chance.Chance.prototype.name_prefix)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>name_prefixes (gender)](#apidoc.element.chance.Chance.prototype.name_prefixes)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>name_suffix (options)](#apidoc.element.chance.Chance.prototype.name_suffix)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>name_suffixes ()](#apidoc.element.chance.Chance.prototype.name_suffixes)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>nationalities ()](#apidoc.element.chance.Chance.prototype.nationalities)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>nationality ()](#apidoc.element.chance.Chance.prototype.nationality)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>natural (options)](#apidoc.element.chance.Chance.prototype.natural)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>normal (options)](#apidoc.element.chance.Chance.prototype.normal)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>normal_pool (options)](#apidoc.element.chance.Chance.prototype.normal_pool)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>pad (number, width, pad)](#apidoc.element.chance.Chance.prototype.pad)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>paragraph (options)](#apidoc.element.chance.Chance.prototype.paragraph)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>phone (options)](#apidoc.element.chance.Chance.prototype.phone)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>pick (arr, count)](#apidoc.element.chance.Chance.prototype.pick)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>pickone (arr)](#apidoc.element.chance.Chance.prototype.pickone)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>pickset (arr, count)](#apidoc.element.chance.Chance.prototype.pickset)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>pl_nip ()](#apidoc.element.chance.Chance.prototype.pl_nip)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>pl_pesel ()](#apidoc.element.chance.Chance.prototype.pl_pesel)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>pl_regon ()](#apidoc.element.chance.Chance.prototype.pl_regon)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>port ()](#apidoc.element.chance.Chance.prototype.port)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>postal ()](#apidoc.element.chance.Chance.prototype.postal)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>prefix (options)](#apidoc.element.chance.Chance.prototype.prefix)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>profession ()](#apidoc.element.chance.Chance.prototype.profession)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>province (options)](#apidoc.element.chance.Chance.prototype.province)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>provinces (options)](#apidoc.element.chance.Chance.prototype.provinces)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>radio (options)](#apidoc.element.chance.Chance.prototype.radio)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>rpg (thrown, options)](#apidoc.element.chance.Chance.prototype.rpg)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>second ()](#apidoc.element.chance.Chance.prototype.second)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>semver (options)](#apidoc.element.chance.Chance.prototype.semver)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>sentence (options)](#apidoc.element.chance.Chance.prototype.sentence)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>set (name, values)](#apidoc.element.chance.Chance.prototype.set)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>shuffle (arr)](#apidoc.element.chance.Chance.prototype.shuffle)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>ssn (options)](#apidoc.element.chance.Chance.prototype.ssn)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>state (options)](#apidoc.element.chance.Chance.prototype.state)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>states (options)](#apidoc.element.chance.Chance.prototype.states)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>street (options)](#apidoc.element.chance.Chance.prototype.street)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>street_suffix (options)](#apidoc.element.chance.Chance.prototype.street_suffix)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>street_suffixes (options)](#apidoc.element.chance.Chance.prototype.street_suffixes)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>string (options)](#apidoc.element.chance.Chance.prototype.string)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>suffix (options)](#apidoc.element.chance.Chance.prototype.suffix)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>syllable (options)](#apidoc.element.chance.Chance.prototype.syllable)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>timestamp ()](#apidoc.element.chance.Chance.prototype.timestamp)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>timezone ()](#apidoc.element.chance.Chance.prototype.timezone)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>timezones ()](#apidoc.element.chance.Chance.prototype.timezones)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>tld ()](#apidoc.element.chance.Chance.prototype.tld)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>tlds ()](#apidoc.element.chance.Chance.prototype.tlds)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>tv (options)](#apidoc.element.chance.Chance.prototype.tv)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>twitter ()](#apidoc.element.chance.Chance.prototype.twitter)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>unique (fn, num, options)](#apidoc.element.chance.Chance.prototype.unique)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>url (options)](#apidoc.element.chance.Chance.prototype.url)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>vat (options)](#apidoc.element.chance.Chance.prototype.vat)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>weekday (options)](#apidoc.element.chance.Chance.prototype.weekday)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>weighted (arr, weights, trim)](#apidoc.element.chance.Chance.prototype.weighted)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>word (options)](#apidoc.element.chance.Chance.prototype.word)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>wp7_anid ()](#apidoc.element.chance.Chance.prototype.wp7_anid)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>wp8_anid2 ()](#apidoc.element.chance.Chance.prototype.wp8_anid2)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>year (options)](#apidoc.element.chance.Chance.prototype.year)
1.  [function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>zip (options)](#apidoc.element.chance.Chance.prototype.zip)
1.  string <span class="apidocSignatureSpan">chance.Chance.prototype.</span>VERSION



# <a name="apidoc.module.chance"></a>[module chance](#apidoc.module.chance)

#### <a name="apidoc.element.chance.chance"></a>[function <span class="apidocSignatureSpan"></span>chance (seed)](#apidoc.element.chance.chance)
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

#### <a name="apidoc.element.chance.toString"></a>[function <span class="apidocSignatureSpan">chance.</span>toString ()](#apidoc.element.chance.toString)
- description and source-code
```javascript
toString = function () {
    return toString;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.chance.Chance"></a>[module chance.Chance](#apidoc.module.chance.Chance)

#### <a name="apidoc.element.chance.Chance.Chance"></a>[function <span class="apidocSignatureSpan">chance.</span>Chance (seed)](#apidoc.element.chance.Chance.Chance)
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



# <a name="apidoc.module.chance.Chance.prototype"></a>[module chance.Chance.prototype](#apidoc.module.chance.Chance.prototype)

#### <a name="apidoc.element.chance.Chance.prototype.HIDN"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>HIDN ()](#apidoc.element.chance.Chance.prototype.HIDN)
- description and source-code
```javascript
HIDN = function (){
 //Hungarian ID nuber structure: XXXXXXYY (X=number,Y=Capital Latin letter)
  var idn_pool="0123456789";
  var idn_chrs="ABCDEFGHIJKLMNOPQRSTUVWXYXZ";
  var idn="";
    idn+=this.string({pool:idn_pool,length:6});
    idn+=this.string({pool:idn_chrs,length:2});
    return idn;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.address"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>address (options)](#apidoc.element.chance.Chance.prototype.address)
- description and source-code
```javascript
address = function (options) {
    options = initOptions(options);
    return this.natural({min: 5, max: 2000}) + ' ' + this.street(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.age"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>age (options)](#apidoc.element.chance.Chance.prototype.age)
- description and source-code
```javascript
age = function (options) {
    options = initOptions(options);
    var ageRange;

    switch (options.type) {
        case 'child':
            ageRange = {min: 0, max: 12};
            break;
        case 'teen':
            ageRange = {min: 13, max: 19};
            break;
        case 'adult':
            ageRange = {min: 18, max: 65};
            break;
        case 'senior':
            ageRange = {min: 65, max: 100};
            break;
        case 'all':
            ageRange = {min: 0, max: 100};
            break;
        default:
            ageRange = {min: 18, max: 65};
            break;
    }

    return this.natural(ageRange);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.altitude"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>altitude (options)](#apidoc.element.chance.Chance.prototype.altitude)
- description and source-code
```javascript
altitude = function (options) {
    options = initOptions(options, {fixed: 5, min: 0, max: 8848});
    return this.floating({
        min: options.min,
        max: options.max,
        fixed: options.fixed
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.ampm"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>ampm ()](#apidoc.element.chance.Chance.prototype.ampm)
- description and source-code
```javascript
ampm = function () {
    return this.bool() ? 'am' : 'pm';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.android_id"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>android_id ()](#apidoc.element.chance.Chance.prototype.android_id)
- description and source-code
```javascript
android_id = function () {
    return "APA91" + this.string({ pool: "0123456789abcefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ-_", length: 178 });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.apple_token"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>apple_token ()](#apidoc.element.chance.Chance.prototype.apple_token)
- description and source-code
```javascript
apple_token = function () {
    return this.string({ pool: "abcdef1234567890", length: 64 });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.areacode"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>areacode (options)](#apidoc.element.chance.Chance.prototype.areacode)
- description and source-code
```javascript
areacode = function (options) {
    options = initOptions(options, {parens : true});
    // Don't want area codes to start with 1, or have a 9 as the second digit
    var areacode = this.natural({min: 2, max: 9}).toString() +
            this.natural({min: 0, max: 8}).toString() +
            this.natural({min: 0, max: 9}).toString();

    return options.parens ? '(' + areacode + ')' : areacode;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.avatar"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>avatar (options)](#apidoc.element.chance.Chance.prototype.avatar)
- description and source-code
```javascript
avatar = function (options) {
    var url = null;
    var URL_BASE = '//www.gravatar.com/avatar/';
    var PROTOCOLS = {
        http: 'http',
        https: 'https'
    };
    var FILE_TYPES = {
        bmp: 'bmp',
        gif: 'gif',
        jpg: 'jpg',
        png: 'png'
    };
    var FALLBACKS = {
        '404': '404', // Return 404 if not found
        mm: 'mm', // Mystery man
        identicon: 'identicon', // Geometric pattern based on hash
        monsterid: 'monsterid', // A generated monster icon
        wavatar: 'wavatar', // A generated face
        retro: 'retro', // 8-bit icon
        blank: 'blank' // A transparent png
    };
    var RATINGS = {
        g: 'g',
        pg: 'pg',
        r: 'r',
        x: 'x'
    };
    var opts = {
        protocol: null,
        email: null,
        fileExtension: null,
        size: null,
        fallback: null,
        rating: null
    };

    if (!options) {
        // Set to a random email
        opts.email = this.email();
        options = {};
    }
    else if (typeof options === 'string') {
        opts.email = options;
        options = {};
    }
    else if (typeof options !== 'object') {
        return null;
    }
    else if (options.constructor === 'Array') {
        return null;
    }

    opts = initOptions(options, opts);

    if (!opts.email) {
        // Set to a random email
        opts.email = this.email();
    }

    // Safe checking for params
    opts.protocol = PROTOCOLS[opts.protocol] ? opts.protocol + ':' : '';
    opts.size = parseInt(opts.size, 0) ? opts.size : '';
    opts.rating = RATINGS[opts.rating] ? opts.rating : '';
    opts.fallback = FALLBACKS[opts.fallback] ? opts.fallback : '';
    opts.fileExtension = FILE_TYPES[opts.fileExtension] ? opts.fileExtension : '';

    url =
        opts.protocol +
        URL_BASE +
        this.bimd5.md5(opts.email) +
        (opts.fileExtension ? '.' + opts.fileExtension : '') +
        (opts.size || opts.rating || opts.fallback ? '?' : '') +
        (opts.size ? '&s=' + opts.size.toString() : '') +
        (opts.rating ? '&r=' + opts.rating : '') +
        (opts.fallback ? '&d=' + opts.fallback : '')
        ;

    return url;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.bb_pin"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>bb_pin ()](#apidoc.element.chance.Chance.prototype.bb_pin)
- description and source-code
```javascript
bb_pin = function () {
    return this.hash({ length: 8 });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.birthday"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>birthday (options)](#apidoc.element.chance.Chance.prototype.birthday)
- description and source-code
```javascript
birthday = function (options) {
    var age = this.age(options);
    var currentYear = new Date().getFullYear();

    if (options && options.type) {
        var min = new Date();
        var max = new Date();
        min.setFullYear(currentYear - age - 1);
        max.setFullYear(currentYear - age);

        options = initOptions(options, {
            min: min,
            max: max
        });
    } else {
        options = initOptions(options, {
            year: currentYear - age
        });
    }

    return this.date(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.blueimp_md5"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>blueimp_md5 ()](#apidoc.element.chance.Chance.prototype.blueimp_md5)
- description and source-code
```javascript
blueimp_md5 = function () {
    return new BlueImpMD5();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.bool"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>bool (options)](#apidoc.element.chance.Chance.prototype.bool)
- description and source-code
```javascript
bool = function (options) {
    // likelihood of success (true)
    options = initOptions(options, {likelihood : 50});

    // Note, we could get some minor perf optimizations by checking range
    // prior to initializing defaults, but that makes code a bit messier
    // and the check more complicated as we have to check existence of
    // the object then existence of the key before checking constraints.
    // Since the options initialization should be minor computationally,
    // decision made for code cleanliness intentionally. This is mentioned
    // here as it's the first occurrence, will not be mentioned again.
    testRange(
        options.likelihood < 0 || options.likelihood > 100,
        "Chance: Likelihood accepts values from 0 to 100."
    );

    return this.random() * 100 < options.likelihood;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.capitalize"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>capitalize (word)](#apidoc.element.chance.Chance.prototype.capitalize)
- description and source-code
```javascript
capitalize = function (word) {
    return word.charAt(0).toUpperCase() + word.substr(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.cc"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>cc (options)](#apidoc.element.chance.Chance.prototype.cc)
- description and source-code
```javascript
cc = function (options) {
    options = initOptions(options);

    var type, number, to_generate;

    type = (options.type) ?
                this.cc_type({ name: options.type, raw: true }) :
                this.cc_type({ raw: true });

    number = type.prefix.split("");
    to_generate = type.length - type.prefix.length - 1;

    // Generates n - 1 digits
    number = number.concat(this.n(this.integer, to_generate, {min: 0, max: 9}));

    // Generates the last digit according to Luhn algorithm
    number.push(this.luhn_calculate(number.join("")));

    return number.join("");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.cc_type"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>cc_type (options)](#apidoc.element.chance.Chance.prototype.cc_type)
- description and source-code
```javascript
cc_type = function (options) {
    options = initOptions(options);
    var types = this.cc_types(),
        type = null;

    if (options.name) {
        for (var i = 0; i < types.length; i++) {
            // Accept either name or short_name to specify card type
            if (types[i].name === options.name || types[i].short_name === options.name) {
                type = types[i];
                break;
            }
        }
        if (type === null) {
            throw new RangeError("Credit card type '" + options.name + "'' is not supported");
        }
    } else {
        type = this.pick(types);
    }

    return options.raw ? type : type.name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.cc_types"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>cc_types ()](#apidoc.element.chance.Chance.prototype.cc_types)
- description and source-code
```javascript
cc_types = function () {
    // http://en.wikipedia.org/wiki/Bank_card_number#Issuer_identification_number_.28IIN.29
    return this.get("cc_types");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.cf"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>cf (options)](#apidoc.element.chance.Chance.prototype.cf)
- description and source-code
```javascript
cf = function (options) {
    options = options || {};
    var gender = !!options.gender ? options.gender : this.gender(),
        first = !!options.first ? options.first : this.first( { gender: gender, nationality: 'it'} ),
        last = !!options.last ? options.last : this.last( { nationality: 'it'} ),
        birthday = !!options.birthday ? options.birthday : this.birthday(),
        city = !!options.city ? options.city : this.pickone(['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'L', 'M', 'Z']) + this
.pad(this.natural({max:999}), 3),
        cf = [],
        name_generator = function(name, isLast) {
            var temp,
                return_value = [];

            if (name.length < 3) {
                return_value = name.split("").concat("XXX".split("")).splice(0,3);
            }
            else {
                temp = name.toUpperCase().split('').map(function(c){
                    return ("BCDFGHJKLMNPRSTVWZ".indexOf(c) !== -1) ? c : undefined;
                }).join('');
                if (temp.length > 3) {
                    if (isLast) {
                        temp = temp.substr(0,3);
                    } else {
                        temp = temp[0] + temp.substr(2,2);
                    }
                }
                if (temp.length < 3) {
                    return_value = temp;
                    temp = name.toUpperCase().split('').map(function(c){
                        return ("AEIOU".indexOf(c) !== -1) ? c : undefined;
                    }).join('').substr(0, 3 - return_value.length);
                }
                return_value = return_value + temp;
            }

            return return_value;
        },
        date_generator = function(birthday, gender, that) {
            var lettermonths = ['A', 'B', 'C', 'D', 'E', 'H', 'L', 'M', 'P', 'R', 'S', 'T'];

            return  birthday.getFullYear().toString().substr(2) +
                    lettermonths[birthday.getMonth()] +
                    that.pad(birthday.getDate() + ((gender.toLowerCase() === "female") ? 40 : 0), 2);
        },
        checkdigit_generator = function(cf) {
            var range1 = "0123456789ABCDEFGHIJKLMNOPQRSTUVWXYZ",
                range2 = "ABCDEFGHIJABCDEFGHIJKLMNOPQRSTUVWXYZ",
                evens  = "ABCDEFGHIJKLMNOPQRSTUVWXYZ",
                odds   = "BAKPLCQDREVOSFTGUHMINJWZYX",
                digit  = 0;


            for(var i = 0; i < 15; i++) {
                if (i % 2 !== 0) {
                    digit += evens.indexOf(range2[range1.indexOf(cf[i])]);
                }
                else {
                    digit +=  odds.indexOf(range2[range1.indexOf(cf[i])]);
                }
            }
            return evens[digit % 26];
        };

    cf = cf.concat(name_generator(last, true), name_generator(first), date_generator(birthday, gender, this), city.toUpperCase().
split("")).join("");
    cf += checkdigit_generator(cf.toUpperCase(), this);

    return cf.toUpperCase();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.character"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>character (options)](#apidoc.element.chance.Chance.prototype.character)
- description and source-code
```javascript
character = function (options) {
    options = initOptions(options);
    testRange(
        options.alpha && options.symbols,
        "Chance: Cannot specify both alpha and symbols."
    );

    var symbols = "!@#$%^&*()[]",
        letters, pool;

    if (options.casing === 'lower') {
        letters = CHARS_LOWER;
    } else if (options.casing === 'upper') {
        letters = CHARS_UPPER;
    } else {
        letters = CHARS_LOWER + CHARS_UPPER;
    }

    if (options.pool) {
        pool = options.pool;
    } else if (options.alpha) {
        pool = letters;
    } else if (options.symbols) {
        pool = symbols;
    } else {
        pool = letters + NUMBERS + symbols;
    }

    return pool.charAt(this.natural({max: (pool.length - 1)}));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.city"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>city ()](#apidoc.element.chance.Chance.prototype.city)
- description and source-code
```javascript
city = function () {
    return this.capitalize(this.word({syllables: 3}));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.cnpj"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>cnpj ()](#apidoc.element.chance.Chance.prototype.cnpj)
- description and source-code
```javascript
cnpj = function () {
    var n = this.n(this.natural, 8, { max: 9 });
    var d1 = 2+n[7]*6+n[6]*7+n[5]*8+n[4]*9+n[3]*2+n[2]*3+n[1]*4+n[0]*5;
    d1 = 11 - (d1 % 11);
    if (d1>=10){
        d1 = 0;
    }
    var d2 = d1*2+3+n[7]*7+n[6]*8+n[5]*9+n[4]*2+n[3]*3+n[2]*4+n[1]*5+n[0]*6;
    d2 = 11 - (d2 % 11);
    if (d2>=10){
        d2 = 0;
    }
    return ''+n[0]+n[1]+'.'+n[2]+n[3]+n[4]+'.'+n[5]+n[6]+n[7]+'/0001-'+d1+d2;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.color"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>color (options)](#apidoc.element.chance.Chance.prototype.color)
- description and source-code
```javascript
color = function (options) {
		function pad(n, width, z) {
			z = z || '0';
			n = n + '';
			return n.length >= width ? n : new Array(width - n.length + 1).join(z) + n;
		}
		
    function gray(value, delimiter) {
        return [value, value, value].join(delimiter || '');
    }

    function rgb(hasAlpha) {
        var rgbValue     = (hasAlpha)    ? 'rgba' : 'rgb';
        var alphaChannel = (hasAlpha)    ? (',' + this.floating({min:min_alpha, max:max_alpha})) : "";
        var colorValue   = (isGrayscale) ? (gray(this.natural({min: min_rgb, max: max_rgb}), ',')) : (this.natural({min: min_green
, max: max_green}) + ',' + this.natural({min: min_blue, max: max_blue}) + ',' + this.natural({max: 255}));
        return rgbValue + '(' + colorValue + alphaChannel + ')';
    }

    function hex(start, end, withHash) {
        var symbol = (withHash) ? "#" : "";
			var hexstring = "";
			
			if (isGrayscale) {
				hexstring = gray(pad(this.hex({min: min_rgb, max: max_rgb}), 2));
				if (options.format === "shorthex") {
					hexstring = gray(this.hex({min: 0, max: 15}));
					console.log("hex: " + hexstring);
				}
			}
			else {
				if (options.format === "shorthex") {
					hexstring = pad(this.hex({min: Math.floor(min_red / 16), max: Math.floor(max_red / 16)}), 1) + pad(this.hex({min: Math.floor
(min_green / 16), max: Math.floor(max_green / 16)}), 1) + pad(this.hex({min: Math.floor(min_blue / 16), max: Math.floor(max_blue
 / 16)}), 1);
				}
				else if (min_red !== undefined || max_red !== undefined || min_green !== undefined || max_green !== undefined || min_blue !==
undefined || max_blue !== undefined) {
					hexstring = pad(this.hex({min: min_red, max: max_red}), 2) + pad(this.hex({min: min_green, max: max_green}), 2) + pad(this.
hex({min: min_blue, max: max_blue}), 2);
				}
				else {
					hexstring = pad(this.hex({min: min_rgb, max: max_rgb}), 2) + pad(this.hex({min: min_rgb, max: max_rgb}), 2) + pad(this.hex({
min: min_rgb, max: max_rgb}), 2);
				}
			}
			
        return symbol + hexstring;
    }

    options = initOptions(options, {
        format: this.pick(['hex', 'shorthex', 'rgb', 'rgba', '0x', 'name']),
        grayscale: false,
        casing: 'lower',
			min: 0,
			max: 255,
			min_red: undefined,
			max_red: undefined,
			min_green: undefined,
			max_green: undefined,
			min_blue: undefined,
			max_blue: undefined,
			min_alpha: 0,
			max_alpha: 1
    });

    var isGrayscale = options.grayscale;
		var min_rgb = options.min;
		var max_rgb = options.max;		
		var min_red = options.min_red;
		var max_red = options.max_red;
		var min_green = options.min_green;
		var max_green = options.max_green;
		var min_blue = options.min_blue;
		var max_blue = options.max_blue;
		var min_alpha = options.min_alpha;
		var max_alpha = options.max_alpha;
		if (options.min_red === undefined) { min_red = min_rgb; }
		if (options.max_red === undefined) { max_red = max_rgb; }
		if (options.min_green === undefined) { min_green = min_rgb; }
		if (options.max_green === undefined) { max_green = max_rgb; }
		if (options.min_blue === undefined) { min_blue = min_rgb; }
		if (options.max_blue === undefined) { max_blue = max_rgb; }
		if (options.min_alpha === undefined) { min_alpha = 0; }
		if (options.max_alpha === undefined) { max_alpha = 1; }
		if (isGrayscale && min_rgb === 0 && max_rgb === 255 && min_red !== undefined && max_red !== undefined) {			
			min_rgb = ((min_red + min_green + min_blue) / 3);
			max_rgb = ((max_red + max_green + max_blue) / 3);
		}
    var colorValue;

    if (options.format === 'hex') {
        colorValue = hex.call(this, 2, 6, true);
    }
    else if (options.format === 'shorthex') {
        colorValue = hex.call(this, 1, 3, true);
    }
    else if (options.format === 'rgb') {
        colorValue = rgb.call(this, false);
    }
    else if (options.format === 'rgba') {
        colorValue = rgb.call(this, true);
    }
    else if (options.format === '0x') {
        colorValue = '0x' + hex.call(this, 2, 6);
    }
    else if(options.format === 'name') {
        return this.pick(this.get("colorNames"));
    } ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.coordinates"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>coordinates (options)](#apidoc.element.chance.Chance.prototype.coordinates)
- description and source-code
```javascript
coordinates = function (options) {
    return this.latitude(options) + ', ' + this.longitude(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.counties"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>counties (options)](#apidoc.element.chance.Chance.prototype.counties)
- description and source-code
```javascript
counties = function (options) {
    options = initOptions(options, { country: 'uk' });
    return this.get("counties")[options.country.toLowerCase()];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.countries"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>countries ()](#apidoc.element.chance.Chance.prototype.countries)
- description and source-code
```javascript
countries = function () {
    return this.get("countries");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.country"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>country (options)](#apidoc.element.chance.Chance.prototype.country)
- description and source-code
```javascript
country = function (options) {
    options = initOptions(options);
    var country = this.pick(this.countries());
    return options.full ? country.name : country.abbreviation;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.county"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>county (options)](#apidoc.element.chance.Chance.prototype.county)
- description and source-code
```javascript
county = function (options) {
    return this.pick(this.counties(options)).name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.cpf"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>cpf (options)](#apidoc.element.chance.Chance.prototype.cpf)
- description and source-code
```javascript
cpf = function (options) {
    options = initOptions(options, {
        formatted: true
    });

    var n = this.n(this.natural, 9, { max: 9 });
    var d1 = n[8]*2+n[7]*3+n[6]*4+n[5]*5+n[4]*6+n[3]*7+n[2]*8+n[1]*9+n[0]*10;
    d1 = 11 - (d1 % 11);
    if (d1>=10) {
        d1 = 0;
    }
    var d2 = d1*2+n[8]*3+n[7]*4+n[6]*5+n[5]*6+n[4]*7+n[3]*8+n[2]*9+n[1]*10+n[0]*11;
    d2 = 11 - (d2 % 11);
    if (d2>=10) {
        d2 = 0;
    }
    var cpf = ''+n[0]+n[1]+n[2]+'.'+n[3]+n[4]+n[5]+'.'+n[6]+n[7]+n[8]+'-'+d1+d2;
    return options.formatted ? cpf : cpf.replace(/\D/g,'');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.currency"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>currency ()](#apidoc.element.chance.Chance.prototype.currency)
- description and source-code
```javascript
currency = function () {
    return this.pick(this.currency_types());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.currency_pair"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>currency_pair (returnAsString)](#apidoc.element.chance.Chance.prototype.currency_pair)
- description and source-code
```javascript
currency_pair = function (returnAsString) {
    var currencies = this.unique(this.currency, 2, {
        comparator: function(arr, val) {

            return arr.reduce(function(acc, item) {
                // If a match has been found, short circuit check and just return
                return acc || (item.code === val.code);
            }, false);
        }
    });

    if (returnAsString) {
        return currencies[0].code + '/' + currencies[1].code;
    } else {
        return currencies;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.currency_types"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>currency_types ()](#apidoc.element.chance.Chance.prototype.currency_types)
- description and source-code
```javascript
currency_types = function () {
    return this.get("currency_types");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.d10"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d10 ()](#apidoc.element.chance.Chance.prototype.d10)
- description and source-code
```javascript
d10 = function () {
    return this.natural(range);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.d100"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d100 ()](#apidoc.element.chance.Chance.prototype.d100)
- description and source-code
```javascript
d100 = function () {
    return this.natural(range);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.d12"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d12 ()](#apidoc.element.chance.Chance.prototype.d12)
- description and source-code
```javascript
d12 = function () {
    return this.natural(range);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.d20"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d20 ()](#apidoc.element.chance.Chance.prototype.d20)
- description and source-code
```javascript
d20 = function () {
    return this.natural(range);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.d30"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d30 ()](#apidoc.element.chance.Chance.prototype.d30)
- description and source-code
```javascript
d30 = function () {
    return this.natural(range);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.d4"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d4 ()](#apidoc.element.chance.Chance.prototype.d4)
- description and source-code
```javascript
d4 = function () {
    return this.natural(range);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.d6"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d6 ()](#apidoc.element.chance.Chance.prototype.d6)
- description and source-code
```javascript
d6 = function () {
    return this.natural(range);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.d8"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>d8 ()](#apidoc.element.chance.Chance.prototype.d8)
- description and source-code
```javascript
d8 = function () {
    return this.natural(range);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.date"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>date (options)](#apidoc.element.chance.Chance.prototype.date)
- description and source-code
```javascript
date = function (options) {
    var date_string, date;

    // If interval is specified we ignore preset
    if(options && (options.min || options.max)) {
        options = initOptions(options, {
            american: true,
            string: false
        });
        var min = typeof options.min !== "undefined" ? options.min.getTime() : 1;
        // 100,000,000 days measured relative to midnight at the beginning of 01 January, 1970 UTC. http://es5.github.io/#x15.9.
1.1
        var max = typeof options.max !== "undefined" ? options.max.getTime() : 8640000000000000;

        date = new Date(this.integer({min: min, max: max}));
    } else {
        var m = this.month({raw: true});
        var daysInMonth = m.days;

        if(options && options.month) {
            // Mod 12 to allow months outside range of 0-11 (not encouraged, but also not prevented).
            daysInMonth = this.get('months')[((options.month % 12) + 12) % 12].days;
        }

        options = initOptions(options, {
            year: parseInt(this.year(), 10),
            // Necessary to subtract 1 because Date() 0-indexes month but not day or year
            // for some reason.
            month: m.numeric - 1,
            day: this.natural({min: 1, max: daysInMonth}),
            hour: this.hour({twentyfour: true}),
            minute: this.minute(),
            second: this.second(),
            millisecond: this.millisecond(),
            american: true,
            string: false
        });

        date = new Date(options.year, options.month, options.day, options.hour, options.minute, options.second, options.millisecond
);
    }

    if (options.american) {
        // Adding 1 to the month is necessary because Date() 0-indexes
        // months but not day for some odd reason.
        date_string = (date.getMonth() + 1) + '/' + date.getDate() + '/' + date.getFullYear();
    } else {
        date_string = date.getDate() + '/' + (date.getMonth() + 1) + '/' + date.getFullYear();
    }

    return options.string ? date_string : date;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.depth"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>depth (options)](#apidoc.element.chance.Chance.prototype.depth)
- description and source-code
```javascript
depth = function (options) {
    options = initOptions(options, {fixed: 5, min: -10994, max: 0});
    return this.floating({
        min: options.min,
        max: options.max,
        fixed: options.fixed
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.dollar"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>dollar (options)](#apidoc.element.chance.Chance.prototype.dollar)
- description and source-code
```javascript
dollar = function (options) {
    // By default, a somewhat more sane max for dollar than all available numbers
    options = initOptions(options, {max : 10000, min : 0});

    var dollar = this.floating({min: options.min, max: options.max, fixed: 2}).toString(),
        cents = dollar.split('.')[1];

    if (cents === undefined) {
        dollar += '.00';
    } else if (cents.length < 2) {
        dollar = dollar + '0';
    }

    if (dollar < 0) {
        return '-$' + dollar.replace('-', '');
    } else {
        return '$' + dollar;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.domain"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>domain (options)](#apidoc.element.chance.Chance.prototype.domain)
- description and source-code
```javascript
domain = function (options) {
    options = initOptions(options);
    return this.word() + '.' + (options.tld || this.tld());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.email"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>email (options)](#apidoc.element.chance.Chance.prototype.email)
- description and source-code
```javascript
email = function (options) {
    options = initOptions(options);
    return this.word({length: options.length}) + '@' + (options.domain || this.domain());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.euro"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>euro (options)](#apidoc.element.chance.Chance.prototype.euro)
- description and source-code
```javascript
euro = function (options) {
    return Number(this.dollar(options).replace("$", "")).toLocaleString() + "€";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.exp"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>exp (options)](#apidoc.element.chance.Chance.prototype.exp)
- description and source-code
```javascript
exp = function (options) {
    options = initOptions(options);
    var exp = {};

    exp.year = this.exp_year();

    // If the year is this year, need to ensure month is greater than the
    // current month or this expiration will not be valid
    if (exp.year === (new Date().getFullYear()).toString()) {
        exp.month = this.exp_month({future: true});
    } else {
        exp.month = this.exp_month();
    }

    return options.raw ? exp : exp.month + '/' + exp.year;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.exp_month"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>exp_month (options)](#apidoc.element.chance.Chance.prototype.exp_month)
- description and source-code
```javascript
exp_month = function (options) {
    options = initOptions(options);
    var month, month_int,
        // Date object months are 0 indexed
        curMonth = new Date().getMonth() + 1;

    if (options.future && (curMonth !== 12)) {
        do {
            month = this.month({raw: true}).numeric;
            month_int = parseInt(month, 10);
        } while (month_int <= curMonth);
    } else {
        month = this.month({raw: true}).numeric;
    }

    return month;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.exp_year"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>exp_year ()](#apidoc.element.chance.Chance.prototype.exp_year)
- description and source-code
```javascript
exp_year = function () {
    var curMonth = new Date().getMonth() + 1,
        curYear = new Date().getFullYear();

    return this.year({min: ((curMonth === 12) ? (curYear + 1) : curYear), max: (curYear + 10)});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.fbid"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>fbid ()](#apidoc.element.chance.Chance.prototype.fbid)
- description and source-code
```javascript
fbid = function () {
    return parseInt('10000' + this.natural({max: 100000000000}), 10);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.file"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>file (options)](#apidoc.element.chance.Chance.prototype.file)
- description and source-code
```javascript
file = function (options) {

    var fileOptions = options || {};
    var poolCollectionKey = "fileExtension";
    var typeRange   = Object.keys(this.get("fileExtension"));//['raster', 'vector', '3d', 'document'];
    var fileName;
    var fileExtension;

    // Generate random file name
    fileName = this.word({length : fileOptions.length});

    // Generate file by specific extension provided by the user
    if(fileOptions.extension) {

        fileExtension = fileOptions.extension;
        return (fileName + '.' + fileExtension);
    }

    // Generate file by specific extension collection
    if(fileOptions.extensions) {

        if(Array.isArray(fileOptions.extensions)) {

            fileExtension = this.pickone(fileOptions.extensions);
            return (fileName + '.' + fileExtension);
        }
        else if(fileOptions.extensions.constructor === Object) {

            var extensionObjectCollection = fileOptions.extensions;
            var keys = Object.keys(extensionObjectCollection);

            fileExtension = this.pickone(extensionObjectCollection[this.pickone(keys)]);
            return (fileName + '.' + fileExtension);
        }

        throw new Error("Expect collection of type Array or Object to be passed as an argument ");
    }

    // Generate file extension based on specific file type
    if(fileOptions.fileType) {

        var fileType = fileOptions.fileType;
        if(typeRange.indexOf(fileType) !== -1) {

            fileExtension = this.pickone(this.get(poolCollectionKey)[fileType]);
            return (fileName + '.' + fileExtension);
        }

        throw new Error("Expect file type value to be 'raster', 'vector', '3d' or 'document' ");
    }

    // Generate random file name if no extension options are passed
    fileExtension = this.pickone(this.get(poolCollectionKey)[this.pickone(typeRange)]);
    return (fileName + '.' + fileExtension);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.first"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>first (options)](#apidoc.element.chance.Chance.prototype.first)
- description and source-code
```javascript
first = function (options) {
    options = initOptions(options, {gender: this.gender(), nationality: 'en'});
    return this.pick(this.get("firstNames")[options.gender.toLowerCase()][options.nationality.toLowerCase()]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.floating"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>floating (options)](#apidoc.element.chance.Chance.prototype.floating)
- description and source-code
```javascript
floating = function (options) {
    options = initOptions(options, {fixed : 4});
    testRange(
        options.fixed && options.precision,
        "Chance: Cannot specify both fixed and precision."
    );

    var num;
    var fixed = Math.pow(10, options.fixed);

    var max = MAX_INT / fixed;
    var min = -max;

    testRange(
        options.min && options.fixed && options.min < min,
        "Chance: Min specified is out of range with fixed. Min should be, at least, " + min
    );
    testRange(
        options.max && options.fixed && options.max > max,
        "Chance: Max specified is out of range with fixed. Max should be, at most, " + max
    );

    options = initOptions(options, { min : min, max : max });

    // Todo - Make this work!
    // options.precision = (typeof options.precision !== "undefined") ? options.precision : false;

    num = this.integer({min: options.min * fixed, max: options.max * fixed});
    var num_fixed = (num / fixed).toFixed(options.fixed);

    return parseFloat(num_fixed);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.gender"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>gender (options)](#apidoc.element.chance.Chance.prototype.gender)
- description and source-code
```javascript
gender = function (options) {
    options = initOptions(options, {extraGenders: []});
    return this.pick(['Male', 'Female'].concat(options.extraGenders));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.geohash"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>geohash (options)](#apidoc.element.chance.Chance.prototype.geohash)
- description and source-code
```javascript
geohash = function (options) {
    options = initOptions(options, { length: 7 });
    return this.string({ length: options.length, pool: '0123456789bcdefghjkmnpqrstuvwxyz' });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.geojson"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>geojson (options)](#apidoc.element.chance.Chance.prototype.geojson)
- description and source-code
```javascript
geojson = function (options) {
    return this.latitude(options) + ', ' + this.longitude(options) + ', ' + this.altitude(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.get"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>get (name)](#apidoc.element.chance.Chance.prototype.get)
- description and source-code
```javascript
get = function (name) {
    return copyObject(data[name]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.google_analytics"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>google_analytics ()](#apidoc.element.chance.Chance.prototype.google_analytics)
- description and source-code
```javascript
google_analytics = function () {
    var account = this.pad(this.natural({max: 999999}), 6);
    var property = this.pad(this.natural({max: 99}), 2);

    return 'UA-' + account + '-' + property;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.guid"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>guid (options)](#apidoc.element.chance.Chance.prototype.guid)
- description and source-code
```javascript
guid = function (options) {
    options = initOptions(options, { version: 5 });

    var guid_pool = "abcdef1234567890",
        variant_pool = "ab89",
        guid = this.string({ pool: guid_pool, length: 8 }) + '-' +
               this.string({ pool: guid_pool, length: 4 }) + '-' +
               // The Version
               options.version +
               this.string({ pool: guid_pool, length: 3 }) + '-' +
               // The Variant
               this.string({ pool: variant_pool, length: 1 }) +
               this.string({ pool: guid_pool, length: 3 }) + '-' +
               this.string({ pool: guid_pool, length: 12 });
    return guid;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.hammertime"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>hammertime (options)](#apidoc.element.chance.Chance.prototype.hammertime)
- description and source-code
```javascript
hammertime = function (options) {
    return this.date(options).getTime();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.hash"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>hash (options)](#apidoc.element.chance.Chance.prototype.hash)
- description and source-code
```javascript
hash = function (options) {
    options = initOptions(options, {length : 40, casing: 'lower'});
    var pool = options.casing === 'upper' ? HEX_POOL.toUpperCase() : HEX_POOL;
    return this.string({pool: pool, length: options.length});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.hashtag"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>hashtag ()](#apidoc.element.chance.Chance.prototype.hashtag)
- description and source-code
```javascript
hashtag = function () {
    return '#' + this.word();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.hex"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>hex (options)](#apidoc.element.chance.Chance.prototype.hex)
- description and source-code
```javascript
hex = function (options) {
    options = initOptions(options, {min: 0, max: MAX_INT, casing: 'lower'});
    testRange(options.min < 0, "Chance: Min cannot be less than zero.");
		var integer = this.natural({min: options.min, max: options.max});
		if (options.casing === 'upper') {
			return integer.toString(16).toUpperCase();
		}
		return integer.toString(16);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.hour"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>hour (options)](#apidoc.element.chance.Chance.prototype.hour)
- description and source-code
```javascript
hour = function (options) {
    options = initOptions(options, {
        min: options && options.twentyfour ? 0 : 1,
        max: options && options.twentyfour ? 23 : 12
    });

    testRange(options.min < 0, "Chance: Min cannot be less than 0.");
    testRange(options.twentyfour && options.max > 23, "Chance: Max cannot be greater than 23 for twentyfour option.");
    testRange(!options.twentyfour && options.max > 12, "Chance: Max cannot be greater than 12.");
    testRange(options.min > options.max, "Chance: Min cannot be greater than Max.");

    return this.natural({min: options.min, max: options.max});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.iban"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>iban ()](#apidoc.element.chance.Chance.prototype.iban)
- description and source-code
```javascript
iban = function () {
    var alpha = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ';
    var alphanum = alpha + '0123456789';
    var iban =
        this.string({ length: 2, pool: alpha }) +
        this.pad(this.integer({ min: 0, max: 99 }), 2) +
        this.string({ length: 4, pool: alphanum }) +
        this.pad(this.natural(), this.natural({ min: 6, max: 26 }));
    return iban;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.integer"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>integer (options)](#apidoc.element.chance.Chance.prototype.integer)
- description and source-code
```javascript
integer = function (options) {
    // 9007199254740992 (2^53) is the max integer number in JavaScript
    // See: http://vq.io/132sa2j
    options = initOptions(options, {min: MIN_INT, max: MAX_INT});
    testRange(options.min > options.max, "Chance: Min cannot be greater than Max.");

    return Math.floor(this.random() * (options.max - options.min + 1) + options.min);
}
```
- example usage
```shell
...

'''js
require(['Chance'], function(Chance) {
    // Instantiate
    var chance = new Chance();

    // Then just use it:
    var my_random_integer = chance.integer();
});
'''

## Dependent tools

* [Chance CLI](https://github.com/chancejs/chance-cli) - Use Chance on the command line.
* [Chance Token Replacer](https://github.com/drewbrokke/chance-token-replacer) - Replace tokens in a string with Chance generated
 items.
...
```

#### <a name="apidoc.element.chance.Chance.prototype.ip"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>ip ()](#apidoc.element.chance.Chance.prototype.ip)
- description and source-code
```javascript
ip = function () {
    // Todo: This could return some reserved IPs. See http://vq.io/137dgYy
    // this should probably be updated to account for that rare as it may be
    return this.natural({min: 1, max: 254}) + '.' +
           this.natural({max: 255}) + '.' +
           this.natural({max: 255}) + '.' +
           this.natural({min: 1, max: 254});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.ipv6"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>ipv6 ()](#apidoc.element.chance.Chance.prototype.ipv6)
- description and source-code
```javascript
ipv6 = function () {
    var ip_addr = this.n(this.hash, 8, {length: 4});

    return ip_addr.join(":");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.israelId"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>israelId ()](#apidoc.element.chance.Chance.prototype.israelId)
- description and source-code
```javascript
israelId = function (){
    var x=this.string({pool: '0123456789',length:8});
    var y=0;
    for (var i=0;i<x.length;i++){
        var thisDigit=  x[i] *  (i/2===parseInt(i/2) ? 1 : 2);
        thisDigit=this.pad(thisDigit,2).toString();
        thisDigit=parseInt(thisDigit[0]) + parseInt(thisDigit[1]);
        y=y+thisDigit;
    }
    x=x+(10-parseInt(y.toString().slice(-1))).toString().slice(-1);
    return x;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.it_vat"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>it_vat ()](#apidoc.element.chance.Chance.prototype.it_vat)
- description and source-code
```javascript
it_vat = function () {
    var it_vat = this.natural({min: 1, max: 1800000});

    it_vat = this.pad(it_vat, 7) + this.pad(this.pick(this.provinces({ country: 'it' })).code, 3);
    return it_vat + this.luhn_calculate(it_vat);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.klout"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>klout ()](#apidoc.element.chance.Chance.prototype.klout)
- description and source-code
```javascript
klout = function () {
    return this.natural({min: 1, max: 99});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.last"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>last (options)](#apidoc.element.chance.Chance.prototype.last)
- description and source-code
```javascript
last = function (options) {
    options = initOptions(options, {nationality: 'en'});
    return this.pick(this.get("lastNames")[options.nationality.toLowerCase()]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.latitude"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>latitude (options)](#apidoc.element.chance.Chance.prototype.latitude)
- description and source-code
```javascript
latitude = function (options) {
    options = initOptions(options, {fixed: 5, min: -90, max: 90});
    return this.floating({min: options.min, max: options.max, fixed: options.fixed});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.longitude"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>longitude (options)](#apidoc.element.chance.Chance.prototype.longitude)
- description and source-code
```javascript
longitude = function (options) {
    options = initOptions(options, {fixed: 5, min: -180, max: 180});
    return this.floating({min: options.min, max: options.max, fixed: options.fixed});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.luhn_calculate"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>luhn_calculate (num)](#apidoc.element.chance.Chance.prototype.luhn_calculate)
- description and source-code
```javascript
luhn_calculate = function (num) {
    var digits = num.toString().split("").reverse();
    var sum = 0;
    var digit;

    for (var i = 0, l = digits.length; l > i; ++i) {
        digit = +digits[i];
        if (i % 2 === 0) {
            digit *= 2;
            if (digit > 9) {
                digit -= 9;
            }
        }
        sum += digit;
    }
    return (sum * 9) % 10;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.luhn_check"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>luhn_check (num)](#apidoc.element.chance.Chance.prototype.luhn_check)
- description and source-code
```javascript
luhn_check = function (num) {
    var str = num.toString();
    var checkDigit = +str.substring(str.length - 1);
    return checkDigit === this.luhn_calculate(+str.substring(0, str.length - 1));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.mac_address"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>mac_address (options)](#apidoc.element.chance.Chance.prototype.mac_address)
- description and source-code
```javascript
mac_address = function (options){
    // typically mac addresses are separated by ":"
    // however they can also be separated by "-"
    // the network variant uses a dot every fourth byte

    options = initOptions(options);
    if(!options.separator) {
        options.separator =  options.networkVersion ? "." : ":";
    }

    var mac_pool="ABCDEF1234567890",
        mac = "";
    if(!options.networkVersion) {
        mac = this.n(this.string, 6, { pool: mac_pool, length:2 }).join(options.separator);
    } else {
        mac = this.n(this.string, 3, { pool: mac_pool, length:4 }).join(options.separator);
    }

    return mac;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.md5"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>md5 (options)](#apidoc.element.chance.Chance.prototype.md5)
- description and source-code
```javascript
md5 = function (options) {
    var opts = { str: '', key: null, raw: false };

    if (!options) {
        opts.str = this.string();
        options = {};
    }
    else if (typeof options === 'string') {
        opts.str = options;
        options = {};
    }
    else if (typeof options !== 'object') {
        return null;
    }
    else if(options.constructor === 'Array') {
        return null;
    }

    opts = initOptions(options, opts);

    if(!opts.str){
        throw new Error('A parameter is required to return an md5 hash.');
    }

    return this.bimd5.md5(opts.str, opts.key, opts.raw);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.mersenne_twister"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>mersenne_twister (seed)](#apidoc.element.chance.Chance.prototype.mersenne_twister)
- description and source-code
```javascript
mersenne_twister = function (seed) {
    return new MersenneTwister(seed);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.millisecond"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>millisecond ()](#apidoc.element.chance.Chance.prototype.millisecond)
- description and source-code
```javascript
millisecond = function () {
    return this.natural({max: 999});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.minute"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>minute (options)](#apidoc.element.chance.Chance.prototype.minute)
- description and source-code
```javascript
minute = function (options) {
    options = initOptions(options, {min: 0, max: 59});

    testRange(options.min < 0, "Chance: Min cannot be less than 0.");
    testRange(options.max > 59, "Chance: Max cannot be greater than 59.");
    testRange(options.min > options.max, "Chance: Min cannot be greater than Max.");

    return this.natural({min: options.min, max: options.max});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.mixin"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>mixin (obj)](#apidoc.element.chance.Chance.prototype.mixin)
- description and source-code
```javascript
mixin = function (obj) {
    for (var func_name in obj) {
        Chance.prototype[func_name] = obj[func_name];
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.month"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>month (options)](#apidoc.element.chance.Chance.prototype.month)
- description and source-code
```javascript
month = function (options) {
    options = initOptions(options, {min: 1, max: 12});

    testRange(options.min < 1, "Chance: Min cannot be less than 1.");
    testRange(options.max > 12, "Chance: Max cannot be greater than 12.");
    testRange(options.min > options.max, "Chance: Min cannot be greater than Max.");

    var month = this.pick(this.months().slice(options.min - 1, options.max));
    return options.raw ? month : month.name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.months"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>months ()](#apidoc.element.chance.Chance.prototype.months)
- description and source-code
```javascript
months = function () {
    return this.get("months");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.mrz"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>mrz (options)](#apidoc.element.chance.Chance.prototype.mrz)
- description and source-code
```javascript
mrz = function (options) {
    var checkDigit = function (input) {
        var alpha = "<ABCDEFGHIJKLMNOPQRSTUVWXYXZ".split(''),
            multipliers = [ 7, 3, 1 ],
            runningTotal = 0;

        if (typeof input !== 'string') {
            input = input.toString();
        }

        input.split('').forEach(function(character, idx) {
            var pos = alpha.indexOf(character);

            if(pos !== -1) {
                character = pos === 0 ? 0 : pos + 9;
            } else {
                character = parseInt(character, 10);
            }
            character *= multipliers[idx % multipliers.length];
            runningTotal += character;
        });
        return runningTotal % 10;
    };
    var generate = function (opts) {
        var pad = function (length) {
            return new Array(length + 1).join('<');
        };
        var number = [ 'P<',
                       opts.issuer,
                       opts.last.toUpperCase(),
                       '<<',
                       opts.first.toUpperCase(),
                       pad(39 - (opts.last.length + opts.first.length + 2)),
                       opts.passportNumber,
                       checkDigit(opts.passportNumber),
                       opts.nationality,
                       opts.dob,
                       checkDigit(opts.dob),
                       opts.gender,
                       opts.expiry,
                       checkDigit(opts.expiry),
                       pad(14),
                       checkDigit(pad(14)) ].join('');

        return number +
            (checkDigit(number.substr(44, 10) +
                        number.substr(57, 7) +
                        number.substr(65, 7)));
    };

    var that = this;

    options = initOptions(options, {
        first: this.first(),
        last: this.last(),
        passportNumber: this.integer({min: 100000000, max: 999999999}),
        dob: (function () {
            var date = that.birthday({type: 'adult'});
            return [date.getFullYear().toString().substr(2),
                    that.pad(date.getMonth() + 1, 2),
                    that.pad(date.getDate(), 2)].join('');
        }()),
        expiry: (function () {
            var date = new Date();
            return [(date.getFullYear() + 5).toString().substr(2),
                    that.pad(date.getMonth() + 1, 2),
                    that.pad(date.getDate(), 2)].join('');
        }()),
        gender: this.gender() === 'Female' ? 'F': 'M',
        issuer: 'GBR',
        nationality: 'GBR'
    });
    return generate (options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.n"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>n (fn, n)](#apidoc.element.chance.Chance.prototype.n)
- description and source-code
```javascript
n = function (fn, n) {
    testRange(
        typeof fn !== "function",
        "Chance: The first argument must be a function."
    );

    if (typeof n === 'undefined') {
        n = 1;
    }
    var i = n, arr = [], params = slice.call(arguments, 2);

    // Providing a negative count should result in a noop.
    i = Math.max( 0, i );

    for (null; i--; null) {
        arr.push(fn.apply(this, params));
    }

    return arr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.name"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>name (options)](#apidoc.element.chance.Chance.prototype.name)
- description and source-code
```javascript
name = function (options) {
    options = initOptions(options);

    var first = this.first(options),
        last = this.last(options),
        name;

    if (options.middle) {
        name = first + ' ' + this.first(options) + ' ' + last;
    } else if (options.middle_initial) {
        name = first + ' ' + this.character({alpha: true, casing: 'upper'}) + '. ' + last;
    } else {
        name = first + ' ' + last;
    }

    if (options.prefix) {
        name = this.prefix(options) + ' ' + name;
    }

    if (options.suffix) {
        name = name + ' ' + this.suffix(options);
    }

    return name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.name_prefix"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>name_prefix (options)](#apidoc.element.chance.Chance.prototype.name_prefix)
- description and source-code
```javascript
name_prefix = function (options) {
    options = initOptions(options, { gender: "all" });
    return options.full ?
        this.pick(this.name_prefixes(options.gender)).name :
        this.pick(this.name_prefixes(options.gender)).abbreviation;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.name_prefixes"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>name_prefixes (gender)](#apidoc.element.chance.Chance.prototype.name_prefixes)
- description and source-code
```javascript
name_prefixes = function (gender) {
    gender = gender || "all";
    gender = gender.toLowerCase();

    var prefixes = [
        { name: 'Doctor', abbreviation: 'Dr.' }
    ];

    if (gender === "male" || gender === "all") {
        prefixes.push({ name: 'Mister', abbreviation: 'Mr.' });
    }

    if (gender === "female" || gender === "all") {
        prefixes.push({ name: 'Miss', abbreviation: 'Miss' });
        prefixes.push({ name: 'Misses', abbreviation: 'Mrs.' });
    }

    return prefixes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.name_suffix"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>name_suffix (options)](#apidoc.element.chance.Chance.prototype.name_suffix)
- description and source-code
```javascript
name_suffix = function (options) {
    options = initOptions(options);
    return options.full ?
        this.pick(this.name_suffixes()).name :
        this.pick(this.name_suffixes()).abbreviation;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.name_suffixes"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>name_suffixes ()](#apidoc.element.chance.Chance.prototype.name_suffixes)
- description and source-code
```javascript
name_suffixes = function () {
    var suffixes = [
        { name: 'Doctor of Osteopathic Medicine', abbreviation: 'D.O.' },
        { name: 'Doctor of Philosophy', abbreviation: 'Ph.D.' },
        { name: 'Esquire', abbreviation: 'Esq.' },
        { name: 'Junior', abbreviation: 'Jr.' },
        { name: 'Juris Doctor', abbreviation: 'J.D.' },
        { name: 'Master of Arts', abbreviation: 'M.A.' },
        { name: 'Master of Business Administration', abbreviation: 'M.B.A.' },
        { name: 'Master of Science', abbreviation: 'M.S.' },
        { name: 'Medical Doctor', abbreviation: 'M.D.' },
        { name: 'Senior', abbreviation: 'Sr.' },
        { name: 'The Third', abbreviation: 'III' },
        { name: 'The Fourth', abbreviation: 'IV' },
        { name: 'Bachelor of Engineering', abbreviation: 'B.E' },
        { name: 'Bachelor of Technology', abbreviation: 'B.TECH' }
    ];
    return suffixes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.nationalities"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>nationalities ()](#apidoc.element.chance.Chance.prototype.nationalities)
- description and source-code
```javascript
nationalities = function () {
    return this.get("nationalities");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.nationality"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>nationality ()](#apidoc.element.chance.Chance.prototype.nationality)
- description and source-code
```javascript
nationality = function () {
    var nationality = this.pick(this.nationalities());
    return nationality.name;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.natural"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>natural (options)](#apidoc.element.chance.Chance.prototype.natural)
- description and source-code
```javascript
natural = function (options) {
    options = initOptions(options, {min: 0, max: MAX_INT});
    testRange(options.min < 0, "Chance: Min cannot be less than zero.");
    return this.integer(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.normal"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>normal (options)](#apidoc.element.chance.Chance.prototype.normal)
- description and source-code
```javascript
normal = function (options) {
    options = initOptions(options, {mean : 0, dev : 1, pool : []});

    testRange(
        options.pool.constructor !== Array,
        "Chance: The pool option must be a valid array."
    );

    // If a pool has been passed, then we are returning an item from that pool,
    // using the normal distribution settings that were passed in
    if (options.pool.length > 0) {
        return this.normal_pool(options);
    }

    // The Marsaglia Polar method
    var s, u, v, norm,
        mean = options.mean,
        dev = options.dev;

    do {
        // U and V are from the uniform distribution on (-1, 1)
        u = this.random() * 2 - 1;
        v = this.random() * 2 - 1;

        s = u * u + v * v;
    } while (s >= 1);

    // Compute the standard normal variate
    norm = u * Math.sqrt(-2 * Math.log(s) / s);

    // Shape and scale
    return dev * norm + mean;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.normal_pool"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>normal_pool (options)](#apidoc.element.chance.Chance.prototype.normal_pool)
- description and source-code
```javascript
normal_pool = function (options) {
    var performanceCounter = 0;
    do {
        var idx = Math.round(this.normal({ mean: options.mean, dev: options.dev }));
        if (idx < options.pool.length && idx >= 0) {
            return options.pool[idx];
        } else {
            performanceCounter++;
        }
    } while(performanceCounter < 100);

    throw new RangeError("Chance: Your pool is too small for the given mean and standard deviation. Please adjust.");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.pad"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>pad (number, width, pad)](#apidoc.element.chance.Chance.prototype.pad)
- description and source-code
```javascript
pad = function (number, width, pad) {
    // Default pad to 0 if none provided
    pad = pad || '0';
    // Convert number to a string
    number = number + '';
    return number.length >= width ? number : new Array(width - number.length + 1).join(pad) + number;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.paragraph"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>paragraph (options)](#apidoc.element.chance.Chance.prototype.paragraph)
- description and source-code
```javascript
paragraph = function (options) {
    options = initOptions(options);

    var sentences = options.sentences || this.natural({min: 3, max: 7}),
        sentence_array = this.n(this.sentence, sentences);

    return sentence_array.join(' ');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.phone"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>phone (options)](#apidoc.element.chance.Chance.prototype.phone)
- description and source-code
```javascript
phone = function (options) {
    var self = this,
        numPick,
        ukNum = function (parts) {
            var section = [];
            //fills the section part of the phone number with random numbers.
            parts.sections.forEach(function(n) {
                section.push(self.string({ pool: '0123456789', length: n}));
            });
            return parts.area + section.join(' ');
        };
    options = initOptions(options, {
        formatted: true,
        country: 'us',
        mobile: false
    });
    if (!options.formatted) {
        options.parens = false;
    }
    var phone;
    switch (options.country) {
        case 'fr':
            if (!options.mobile) {
                numPick = this.pick([
                    // Valid zone and département codes.
                    '01' + this.pick(['30', '34', '39', '40', '41', '42', '43', '44', '45', '46', '47', '48', '49', '53', '55', '
56', '58', '60', '64', '69', '70', '72', '73', '74', '75', '76', '77', '78', '79', '80', '81', '82', '83']) + self.string({ pool
: '0123456789', length: 6}),
                    '02' + this.pick(['14', '18', '22', '23', '28', '29', '30', '31', '32', '33', '34', '35', '36', '37', '38', '
40', '41', '43', '44', '45', '46', '47', '48', '49', '50', '51', '52', '53', '54', '56', '57', '61', '62', '69', '72', '76', '77
', '78', '85', '90', '96', '97', '98', '99']) + self.string({ pool: '0123456789', length: 6}),
                    '03' + this.pick(['10', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '39', '44', '45', '51', '
52', '54', '55', '57', '58', '59', '60', '61', '62', '63', '64', '65', '66', '67', '68', '69', '70', '71', '72', '73', '80', '81
', '82', '83', '84', '85', '86', '87', '88', '89', '90']) + self.string({ pool: '0123456789', length: 6}),
                    '04' + this.pick(['11', '13', '15', '20', '22', '26', '27', '30', '32', '34', '37', '42', '43', '44', '50', '
56', '57', '63', '66', '67', '68', '69', '70', '71', '72', '73', '74', '75', '76', '77', '78', '79', '80', '81', '82', '83', '84
', '85', '86', '88', '89', '90', '91', '92', '93', '94', '95', '97', '98']) + self.string({ pool: '0123456789', length: 6}),
                    '05' + this.pick(['08', '16', '17', '19', '24', '31', '32', '33', '34', '35', '40', '45', '46', '47', '49', '
53', '55', '56', '57', '58', '59', '61', '62', '63', '64', '65', '67', '79', '81', '82', '86', '87', '90', '94']) + self.string({
pool: '0123456789', length: 6}),
                    '09' + self.string({ pool: '0123456789', length: 8}),
                ]);
                phone = options.formatted ? numPick.match(/../g).join(' ') : numPick;
            } else {
                numPick = this.pick(['06', '07']) + self.string({ pool: '0123456789', length: 8});
                phone = options.formatted ? numPick.match(/../g).join(' ') : numPick;
            }
            break;
        case 'uk':
            if (!options.mobile) {
                numPick = this.pick([
                    //valid area codes of major cities/counties followed by random numbers in required format.

                    { area: '01' + this.character({ pool: '234569' }) + '1 ', sections: [3,4] },
                    { area: '020 ' + this.character({ pool: '378' }), sections: [3,4] },
                    { area: '023 ' + this.character({ pool: '89' }), sections: [3,4] },
                    { area: '024 7', sections: [3,4] },
                    { area: '028 ' + this.pick(['25','28','37','71','82','90','92','95']), sections: [2,4] },
                    { area: '012' + this.pick(['04','08','54','76','97','98']) + ' ', sections: [6] },
                    { area: '013' + this.pick(['63','64','84','86']) + ' ', sections: [6] },
                    { area: '014' + this.pick(['04','20','60','61','80','88']) + ' ', sections: [6] },
                    { area: '015' + this.pick(['24','27','62','66']) + ' ', sections: [6] },
                    { area: '016' + this.pick(['06','29','35','47','59','95']) + ' ', sections: [6] },
                    { area: '017' + this.pick(['26','44','50','68']) ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.pick"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>pick (arr, count)](#apidoc.element.chance.Chance.prototype.pick)
- description and source-code
```javascript
pick = function (arr, count) {
    if (arr.length === 0) {
        throw new RangeError("Chance: Cannot pick() from an empty array");
    }
    if (!count || count === 1) {
        return arr[this.natural({max: arr.length - 1})];
    } else {
        return this.shuffle(arr).slice(0, count);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.pickone"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>pickone (arr)](#apidoc.element.chance.Chance.prototype.pickone)
- description and source-code
```javascript
pickone = function (arr) {
    if (arr.length === 0) {
      throw new RangeError("Chance: Cannot pickone() from an empty array");
    }
    return arr[this.natural({max: arr.length - 1})];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.pickset"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>pickset (arr, count)](#apidoc.element.chance.Chance.prototype.pickset)
- description and source-code
```javascript
pickset = function (arr, count) {
    if (count === 0) {
        return [];
    }
    if (arr.length === 0) {
        throw new RangeError("Chance: Cannot pickset() from an empty array");
    }
    if (count < 0) {
        throw new RangeError("Chance: count must be positive number");
    }
    if (!count || count === 1) {
        return [ this.pickone(arr) ];
    } else {
        return this.shuffle(arr).slice(0, count);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.pl_nip"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>pl_nip ()](#apidoc.element.chance.Chance.prototype.pl_nip)
- description and source-code
```javascript
pl_nip = function () {
    var number = this.natural({min: 1, max: 999999999});
    var arr = this.pad(number, 9).split('');
    for (var i = 0; i < arr.length; i++) {
        arr[i] = parseInt(arr[i]);
    }

    var controlNumber = (6 * arr[0] + 5 * arr[1] + 7 * arr[2] + 2 * arr[3] + 3 * arr[4] + 4 * arr[5] + 5 * arr[6] + 6 * arr[7] +
7 * arr[8]) % 11;
    if(controlNumber === 10) {
        return this.pl_nip();
    }

    return arr.join('') + controlNumber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.pl_pesel"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>pl_pesel ()](#apidoc.element.chance.Chance.prototype.pl_pesel)
- description and source-code
```javascript
pl_pesel = function () {
    var number = this.natural({min: 1, max: 9999999999});
    var arr = this.pad(number, 10).split('');
    for (var i = 0; i < arr.length; i++) {
        arr[i] = parseInt(arr[i]);
    }

    var controlNumber = (1 * arr[0] + 3 * arr[1] + 7 * arr[2] + 9 * arr[3] + 1 * arr[4] + 3 * arr[5] + 7 * arr[6] + 9 * arr[7] +
1 * arr[8] + 3 * arr[9]) % 10;
    if(controlNumber !== 0) {
        controlNumber = 10 - controlNumber;
    }

    return arr.join('') + controlNumber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.pl_regon"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>pl_regon ()](#apidoc.element.chance.Chance.prototype.pl_regon)
- description and source-code
```javascript
pl_regon = function () {
    var number = this.natural({min: 1, max: 99999999});
    var arr = this.pad(number, 8).split('');
    for (var i = 0; i < arr.length; i++) {
        arr[i] = parseInt(arr[i]);
    }

    var controlNumber = (8 * arr[0] + 9 * arr[1] + 2 * arr[2] + 3 * arr[3] + 4 * arr[4] + 5 * arr[5] + 6 * arr[6] + 7 * arr[7]) %
11;
    if(controlNumber === 10) {
        controlNumber = 0;
    }

    return arr.join('') + controlNumber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.port"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>port ()](#apidoc.element.chance.Chance.prototype.port)
- description and source-code
```javascript
port = function () {
    return this.integer({min: 0, max: 65535});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.postal"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>postal ()](#apidoc.element.chance.Chance.prototype.postal)
- description and source-code
```javascript
postal = function () {
    // Postal District
    var pd = this.character({pool: "XVTSRPNKLMHJGECBA"});
    // Forward Sortation Area (FSA)
    var fsa = pd + this.natural({max: 9}) + this.character({alpha: true, casing: "upper"});
    // Local Delivery Unut (LDU)
    var ldu = this.natural({max: 9}) + this.character({alpha: true, casing: "upper"}) + this.natural({max: 9});

    return fsa + " " + ldu;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.prefix"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>prefix (options)](#apidoc.element.chance.Chance.prototype.prefix)
- description and source-code
```javascript
prefix = function (options) {
    return this.name_prefix(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.profession"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>profession ()](#apidoc.element.chance.Chance.prototype.profession)
- description and source-code
```javascript
profession = function () {
    return this.pick(this.get("professions"));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.province"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>province (options)](#apidoc.element.chance.Chance.prototype.province)
- description and source-code
```javascript
province = function (options) {
    return (options && options.full) ?
        this.pick(this.provinces(options)).name :
        this.pick(this.provinces(options)).abbreviation;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.provinces"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>provinces (options)](#apidoc.element.chance.Chance.prototype.provinces)
- description and source-code
```javascript
provinces = function (options) {
    options = initOptions(options, { country: 'ca' });
    return this.get("provinces")[options.country.toLowerCase()];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.radio"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>radio (options)](#apidoc.element.chance.Chance.prototype.radio)
- description and source-code
```javascript
radio = function (options) {
    // Initial Letter (Typically Designated by Side of Mississippi River)
    options = initOptions(options, {side : "?"});
    var fl = "";
    switch (options.side.toLowerCase()) {
    case "east":
    case "e":
        fl = "W";
        break;
    case "west":
    case "w":
        fl = "K";
        break;
    default:
        fl = this.character({pool: "KW"});
        break;
    }

    return fl + this.character({alpha: true, casing: "upper"}) +
            this.character({alpha: true, casing: "upper"}) +
            this.character({alpha: true, casing: "upper"});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.rpg"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>rpg (thrown, options)](#apidoc.element.chance.Chance.prototype.rpg)
- description and source-code
```javascript
rpg = function (thrown, options) {
    options = initOptions(options);
    if (!thrown) {
        throw new RangeError("A type of die roll must be included");
    } else {
        var bits = thrown.toLowerCase().split("d"),
            rolls = [];

        if (bits.length !== 2 || !parseInt(bits[0], 10) || !parseInt(bits[1], 10)) {
            throw new Error("Invalid format provided. Please provide #d# where the first # is the number of dice to roll, the second
 # is the max of each die");
        }
        for (var i = bits[0]; i > 0; i--) {
            rolls[i - 1] = this.natural({min: 1, max: bits[1]});
        }
        return (typeof options.sum !== 'undefined' && options.sum) ? rolls.reduce(function (p, c) { return p + c; }) : rolls;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.second"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>second ()](#apidoc.element.chance.Chance.prototype.second)
- description and source-code
```javascript
second = function () {
    return this.natural({max: 59});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.semver"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>semver (options)](#apidoc.element.chance.Chance.prototype.semver)
- description and source-code
```javascript
semver = function (options) {
    options = initOptions(options, { include_prerelease: true });

    var range = this.pickone(["^", "~", "<", ">", "<=", ">=", "="]);
    if (options.range) {
        range = options.range;
    }

    var prerelease = "";
    if (options.include_prerelease) {
        prerelease = this.weighted(["", "-dev", "-beta", "-alpha"], [50, 10, 5, 1]);
    }
    return range + this.rpg('3d10').join('.') + prerelease;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.sentence"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>sentence (options)](#apidoc.element.chance.Chance.prototype.sentence)
- description and source-code
```javascript
sentence = function (options) {
    options = initOptions(options);

    var words = options.words || this.natural({min: 12, max: 18}),
        punctuation = options.punctuation,
        text, word_array = this.n(this.word, words);

    text = word_array.join(' ');

    // Capitalize first letter of sentence
    text = this.capitalize(text);

    // Make sure punctuation has a usable value
    if (punctuation !== false && !/^[\.\?;!:]$/.test(punctuation)) {
        punctuation = '.';
    }

    // Add punctuation mark
    if (punctuation) {
        text += punctuation;
    }

    return text;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.set"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>set (name, values)](#apidoc.element.chance.Chance.prototype.set)
- description and source-code
```javascript
set = function (name, values) {
    if (typeof name === "string") {
        data[name] = values;
    } else {
        data = copyObject(name, data);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.shuffle"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>shuffle (arr)](#apidoc.element.chance.Chance.prototype.shuffle)
- description and source-code
```javascript
shuffle = function (arr) {
    var old_array = arr.slice(0),
        new_array = [],
        j = 0,
        length = Number(old_array.length);

    for (var i = 0; i < length; i++) {
        // Pick a random index from the array
        j = this.natural({max: old_array.length - 1});
        // Add it to the new array
        new_array[i] = old_array[j];
        // Remove that element from the original array
        old_array.splice(j, 1);
    }

    return new_array;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.ssn"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>ssn (options)](#apidoc.element.chance.Chance.prototype.ssn)
- description and source-code
```javascript
ssn = function (options) {
    options = initOptions(options, {ssnFour: false, dashes: true});
    var ssn_pool = "1234567890",
        ssn,
        dash = options.dashes ? '-' : '';

    if(!options.ssnFour) {
        ssn = this.string({pool: ssn_pool, length: 3}) + dash +
        this.string({pool: ssn_pool, length: 2}) + dash +
        this.string({pool: ssn_pool, length: 4});
    } else {
        ssn = this.string({pool: ssn_pool, length: 4});
    }
    return ssn;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.state"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>state (options)](#apidoc.element.chance.Chance.prototype.state)
- description and source-code
```javascript
state = function (options) {
    return (options && options.full) ?
        this.pick(this.states(options)).name :
        this.pick(this.states(options)).abbreviation;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.states"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>states (options)](#apidoc.element.chance.Chance.prototype.states)
- description and source-code
```javascript
states = function (options) {
    options = initOptions(options, { country: 'us', us_states_and_dc: true } );

    var states;

    switch (options.country.toLowerCase()) {
        case 'us':
            var us_states_and_dc = this.get("us_states_and_dc"),
                territories = this.get("territories"),
                armed_forces = this.get("armed_forces");

            states = [];

            if (options.us_states_and_dc) {
                states = states.concat(us_states_and_dc);
            }
            if (options.territories) {
                states = states.concat(territories);
            }
            if (options.armed_forces) {
                states = states.concat(armed_forces);
            }
            break;
        case 'it':
            states = this.get("country_regions")[options.country.toLowerCase()];
            break;
        case 'uk':
            states = this.get("counties")[options.country.toLowerCase()];
            break;
    }

    return states;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.street"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>street (options)](#apidoc.element.chance.Chance.prototype.street)
- description and source-code
```javascript
street = function (options) {
    options = initOptions(options, { country: 'us', syllables: 2 });
    var     street;

    switch (options.country.toLowerCase()) {
        case 'us':
            street = this.word({ syllables: options.syllables });
            street = this.capitalize(street);
            street += ' ';
            street += options.short_suffix ?
                this.street_suffix(options).abbreviation :
                this.street_suffix(options).name;
            break;
        case 'it':
            street = this.word({ syllables: options.syllables });
            street = this.capitalize(street);
            street = (options.short_suffix ?
                this.street_suffix(options).abbreviation :
                this.street_suffix(options).name) + " " + street;
            break;
    }
    return street;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.street_suffix"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>street_suffix (options)](#apidoc.element.chance.Chance.prototype.street_suffix)
- description and source-code
```javascript
street_suffix = function (options) {
    options = initOptions(options, { country: 'us' });
    return this.pick(this.street_suffixes(options));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.street_suffixes"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>street_suffixes (options)](#apidoc.element.chance.Chance.prototype.street_suffixes)
- description and source-code
```javascript
street_suffixes = function (options) {
    options = initOptions(options, { country: 'us' });
    // These are the most common suffixes.
    return this.get("street_suffixes")[options.country.toLowerCase()];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.string"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>string (options)](#apidoc.element.chance.Chance.prototype.string)
- description and source-code
```javascript
string = function (options) {
    options = initOptions(options, { length: this.natural({min: 5, max: 20}) });
    testRange(options.length < 0, "Chance: Length cannot be less than zero.");
    var length = options.length,
        text = this.n(this.character, length, options);

    return text.join("");
}
```
- example usage
```shell
...
then in the HTML of your app:

'''html
<!-- Load Chance -->
<script type="text/javascript" src="app/bower_components/chance/chance.min.js"></script>
<script>
    // Use Chance immediately!
    alert(chance.string());
</script>
'''

### Component

It can also be used with [Component](http://component.io)
...
```

#### <a name="apidoc.element.chance.Chance.prototype.suffix"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>suffix (options)](#apidoc.element.chance.Chance.prototype.suffix)
- description and source-code
```javascript
suffix = function (options) {
    return this.name_suffix(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.syllable"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>syllable (options)](#apidoc.element.chance.Chance.prototype.syllable)
- description and source-code
```javascript
syllable = function (options) {
    options = initOptions(options);

    var length = options.length || this.natural({min: 2, max: 3}),
        consonants = 'bcdfghjklmnprstvwz', // consonants except hard to speak ones
        vowels = 'aeiou', // vowels
        all = consonants + vowels, // all
        text = '',
        chr;

    // I'm sure there's a more elegant way to do this, but this works
    // decently well.
    for (var i = 0; i < length; i++) {
        if (i === 0) {
            // First character can be anything
            chr = this.character({pool: all});
        } else if (consonants.indexOf(chr) === -1) {
            // Last character was a vowel, now we want a consonant
            chr = this.character({pool: consonants});
        } else {
            // Last character was a consonant, now we want a vowel
            chr = this.character({pool: vowels});
        }

        text += chr;
    }

    if (options.capitalize) {
        text = this.capitalize(text);
    }

    return text;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.timestamp"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>timestamp ()](#apidoc.element.chance.Chance.prototype.timestamp)
- description and source-code
```javascript
timestamp = function () {
    return this.natural({min: 1, max: parseInt(new Date().getTime() / 1000, 10)});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.timezone"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>timezone ()](#apidoc.element.chance.Chance.prototype.timezone)
- description and source-code
```javascript
timezone = function () {
    return this.pick(this.timezones());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.timezones"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>timezones ()](#apidoc.element.chance.Chance.prototype.timezones)
- description and source-code
```javascript
timezones = function () {
    return this.get("timezones");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.tld"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>tld ()](#apidoc.element.chance.Chance.prototype.tld)
- description and source-code
```javascript
tld = function () {
    return this.pick(this.tlds());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.tlds"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>tlds ()](#apidoc.element.chance.Chance.prototype.tlds)
- description and source-code
```javascript
tlds = function () {
    return ['com', 'org', 'edu', 'gov', 'co.uk', 'net', 'io', 'ac', 'ad', 'ae', 'af', 'ag', 'ai', 'al', 'am', 'an', 'ao', 'aq', '
ar', 'as', 'at', 'au', 'aw', 'ax', 'az', 'ba', 'bb', 'bd', 'be', 'bf', 'bg', 'bh', 'bi', 'bj', 'bm', 'bn', 'bo', 'bq', 'br', 'bs
', 'bt', 'bv', 'bw', 'by', 'bz', 'ca', 'cc', 'cd', 'cf', 'cg', 'ch', 'ci', 'ck', 'cl', 'cm', 'cn', 'co', 'cr', 'cu', 'cv', 'cw', '
cx', 'cy', 'cz', 'de', 'dj', 'dk', 'dm', 'do', 'dz', 'ec', 'ee', 'eg', 'eh', 'er', 'es', 'et', 'eu', 'fi', 'fj', 'fk', 'fm', 'fo
', 'fr', 'ga', 'gb', 'gd', 'ge', 'gf', 'gg', 'gh', 'gi', 'gl', 'gm', 'gn', 'gp', 'gq', 'gr', 'gs', 'gt', 'gu', 'gw', 'gy', 'hk', '
hm', 'hn', 'hr', 'ht', 'hu', 'id', 'ie', 'il', 'im', 'in', 'io', 'iq', 'ir', 'is', 'it', 'je', 'jm', 'jo', 'jp', 'ke', 'kg', 'kh
', 'ki', 'km', 'kn', 'kp', 'kr', 'kw', 'ky', 'kz', 'la', 'lb', 'lc', 'li', 'lk', 'lr', 'ls', 'lt', 'lu', 'lv', 'ly', 'ma', 'mc', '
md', 'me', 'mg', 'mh', 'mk', 'ml', 'mm', 'mn', 'mo', 'mp', 'mq', 'mr', 'ms', 'mt', 'mu', 'mv', 'mw', 'mx', 'my', 'mz', 'na', 'nc
', 'ne', 'nf', 'ng', 'ni', 'nl', 'no', 'np', 'nr', 'nu', 'nz', 'om', 'pa', 'pe', 'pf', 'pg', 'ph', 'pk', 'pl', 'pm', 'pn', 'pr', '
ps', 'pt', 'pw', 'py', 'qa', 're', 'ro', 'rs', 'ru', 'rw', 'sa', 'sb', 'sc', 'sd', 'se', 'sg', 'sh', 'si', 'sj', 'sk', 'sl', 'sm
', 'sn', 'so', 'sr', 'ss', 'st', 'su', 'sv', 'sx', 'sy', 'sz', 'tc', 'td', 'tf', 'tg', 'th', 'tj', 'tk', 'tl', 'tm', 'tn', 'to', '
tp', 'tr', 'tt', 'tv', 'tw', 'tz', 'ua', 'ug', 'uk', 'us', 'uy', 'uz', 'va', 'vc', 've', 'vg', 'vi', 'vn', 'vu', 'wf', 'ws', 'ye
', 'yt', 'za', 'zm', 'zw'];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.tv"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>tv (options)](#apidoc.element.chance.Chance.prototype.tv)
- description and source-code
```javascript
tv = function (options) {
    return this.radio(options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.twitter"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>twitter ()](#apidoc.element.chance.Chance.prototype.twitter)
- description and source-code
```javascript
twitter = function () {
    return '@' + this.word();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.unique"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>unique (fn, num, options)](#apidoc.element.chance.Chance.prototype.unique)
- description and source-code
```javascript
unique = function (fn, num, options) {
    testRange(
        typeof fn !== "function",
        "Chance: The first argument must be a function."
    );

    var comparator = function(arr, val) { return arr.indexOf(val) !== -1; };

    if (options) {
        comparator = options.comparator || comparator;
    }

    var arr = [], count = 0, result, MAX_DUPLICATES = num * 50, params = slice.call(arguments, 2);

    while (arr.length < num) {
        var clonedParams = JSON.parse(JSON.stringify(params));
        result = fn.apply(this, clonedParams);
        if (!comparator(arr, result)) {
            arr.push(result);
            // reset count when unique found
            count = 0;
        }

        if (++count > MAX_DUPLICATES) {
            throw new RangeError("Chance: num is likely too large for sample set");
        }
    }
    return arr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.url"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>url (options)](#apidoc.element.chance.Chance.prototype.url)
- description and source-code
```javascript
url = function (options) {
    options = initOptions(options, { protocol: "http", domain: this.domain(options), domain_prefix: "", path: this.word(), extensions
: []});

    var extension = options.extensions.length > 0 ? "." + this.pick(options.extensions) : "";
    var domain = options.domain_prefix ? options.domain_prefix + "." + options.domain : options.domain;

    return options.protocol + "://" + domain + "/" + options.path + extension;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.vat"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>vat (options)](#apidoc.element.chance.Chance.prototype.vat)
- description and source-code
```javascript
vat = function (options) {
    options = initOptions(options, { country: 'it' });
    switch (options.country.toLowerCase()) {
        case 'it':
            return this.it_vat();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.weekday"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>weekday (options)](#apidoc.element.chance.Chance.prototype.weekday)
- description and source-code
```javascript
weekday = function (options) {
    options = initOptions(options, {weekday_only: false});
    var weekdays = ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"];
    if (!options.weekday_only) {
        weekdays.push("Saturday");
        weekdays.push("Sunday");
    }
    return this.pickone(weekdays);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.weighted"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>weighted (arr, weights, trim)](#apidoc.element.chance.Chance.prototype.weighted)
- description and source-code
```javascript
weighted = function (arr, weights, trim) {
    if (arr.length !== weights.length) {
        throw new RangeError("Chance: length of array and weights must match");
    }

    // scan weights array and sum valid entries
    var sum = 0;
    var val;
    for (var weightIndex = 0; weightIndex < weights.length; ++weightIndex) {
        val = weights[weightIndex];
        if (isNaN(val)) {
            throw new RangeError("all weights must be numbers");
        }

        if (val > 0) {
            sum += val;
        }
    }

    if (sum === 0) {
        throw new RangeError("Chance: no valid entries in array weights");
    }

    // select a value within range
    var selected = this.random() * sum;

    // find array entry corresponding to selected value
    var total = 0;
    var lastGoodIdx = -1;
    var chosenIdx;
    for (weightIndex = 0; weightIndex < weights.length; ++weightIndex) {
        val = weights[weightIndex];
        total += val;
        if (val > 0) {
            if (selected <= total) {
                chosenIdx = weightIndex;
                break;
            }
            lastGoodIdx = weightIndex;
        }

        // handle any possible rounding error comparison to ensure something is picked
        if (weightIndex === (weights.length - 1)) {
            chosenIdx = lastGoodIdx;
        }
    }

    var chosen = arr[chosenIdx];
    trim = (typeof trim === 'undefined') ? false : trim;
    if (trim) {
        arr.splice(chosenIdx, 1);
        weights.splice(chosenIdx, 1);
    }

    return chosen;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.word"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>word (options)](#apidoc.element.chance.Chance.prototype.word)
- description and source-code
```javascript
word = function (options) {
    options = initOptions(options);

    testRange(
        options.syllables && options.length,
        "Chance: Cannot specify both syllables AND length."
    );

    var syllables = options.syllables || this.natural({min: 1, max: 3}),
        text = '';

    if (options.length) {
        // Either bound word by length
        do {
            text += this.syllable();
        } while (text.length < options.length);
        text = text.substring(0, options.length);
    } else {
        // Or by number of syllables
        for (var i = 0; i < syllables; i++) {
            text += this.syllable();
        }
    }

    if (options.capitalize) {
        text = this.capitalize(text);
    }

    return text;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.wp7_anid"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>wp7_anid ()](#apidoc.element.chance.Chance.prototype.wp7_anid)
- description and source-code
```javascript
wp7_anid = function () {
    return 'A=' + this.guid().replace(/-/g, '').toUpperCase() + '&E=' + this.hash({ length:3 }) + '&W=' + this.integer({ min:0,
max:9 });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.wp8_anid2"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>wp8_anid2 ()](#apidoc.element.chance.Chance.prototype.wp8_anid2)
- description and source-code
```javascript
wp8_anid2 = function () {
    return base64( this.hash( { length : 32 } ) );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.year"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>year (options)](#apidoc.element.chance.Chance.prototype.year)
- description and source-code
```javascript
year = function (options) {
    // Default to current year as min if none specified
    options = initOptions(options, {min: new Date().getFullYear()});

    // Default to one century after current year as max if none specified
    options.max = (typeof options.max !== "undefined") ? options.max : options.min + 100;

    return this.natural(options).toString();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.chance.Chance.prototype.zip"></a>[function <span class="apidocSignatureSpan">chance.Chance.prototype.</span>zip (options)](#apidoc.element.chance.Chance.prototype.zip)
- description and source-code
```javascript
zip = function (options) {
    var zip = this.n(this.natural, 5, {max: 9});

    if (options && options.plusfour === true) {
        zip.push('-');
        zip = zip.concat(this.n(this.natural, 4, {max: 9}));
    }

    return zip.join("");
}
```
- example usage
```shell
...
And it can be used in Node.js.

'''js
var Chance = require('chance'),
    chance = new Chance();

// Get a random zip code
chance.zip();
'''

### RequireJS

Chance also includes an AMD define so it can be used with RequireJS.

'''js
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
