# npmdoc-pinyin

#### api documentation for  [pinyin (v2.8.3)](http://pinyin.hotoo.me/)  [![npm package](https://img.shields.io/npm/v/npmdoc-pinyin.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-pinyin) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-pinyin.svg)](https://travis-ci.org/npmdoc/node-npmdoc-pinyin)

#### 汉语拼音转换工具。

[![NPM](https://nodei.co/npm/pinyin.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/pinyin)

- [https://npmdoc.github.io/node-npmdoc-pinyin/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-pinyin/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-pinyin/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-pinyin/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-pinyin/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-pinyin/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "闲耘"
    },
    "bin": {
        "pinyin": "./bin/pinyin"
    },
    "browser": "lib/web-pinyin.js",
    "bugs": {
        "url": "https://github.com/hotoo/pinyin/issues"
    },
    "dependencies": {
        "commander": "~1.1.1",
        "nodejieba": "^2.2.1",
        "object-assign": "^4.0.1"
    },
    "description": "汉语拼音转换工具。",
    "devDependencies": {
        "benchmark": "~1.0.0",
        "eslint": "~0.24.0",
        "expect.js": "0.3.1",
        "istanbul": "~0.3.17",
        "mocha": "1.17.1",
        "request": "2.33.0"
    },
    "directories": {
        "example": "examples",
        "test": "tests"
    },
    "dist": {
        "shasum": "301ccb4358ccfe802523c4bd640a612bee4d7c4b",
        "tarball": "https://registry.npmjs.org/pinyin/-/pinyin-2.8.3.tgz"
    },
    "files": [
        "bin",
        "data",
        "lib",
        "index.js",
        "src"
    ],
    "gitHead": "707f9210abafcda8a937c1aee0b31a6465948764",
    "homepage": "http://pinyin.hotoo.me/",
    "keywords": [
        "拼音",
        "汉语",
        "汉字",
        "中文",
        "Pinyin"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "hotoo"
        }
    ],
    "name": "pinyin",
    "optionalDependencies": {
        "nodejieba": "^2.2.1"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/hotoo/pinyin.git"
    },
    "scripts": {
        "test": "make test"
    },
    "spm": {
        "main": "lib/web-pinyin.js",
        "devDependencies": {
            "expect.js": "0.3.1",
            "url": "1.2.0"
        },
        "build": {
            "babel": {}
        },
        "tests": "tests/*-spec.js",
        "dependencies": {
            "object-assign": "~4.0.1"
        }
    },
    "version": "2.8.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
