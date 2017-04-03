# api documentation for  [pinyin (v2.8.3)](http://pinyin.hotoo.me/)  [![npm package](https://img.shields.io/npm/v/npmdoc-pinyin.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-pinyin) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-pinyin.svg)](https://travis-ci.org/npmdoc/node-npmdoc-pinyin)
#### 汉语拼音转换工具。

[![NPM](https://nodei.co/npm/pinyin.png?downloads=true)](https://www.npmjs.com/package/pinyin)

[![apidoc](https://npmdoc.github.io/node-npmdoc-pinyin/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-pinyin_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-pinyin/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-pinyin/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-pinyin/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "闲耘",
        "email": "hotoo.cn@gmail.com"
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
            "name": "hotoo",
            "email": "hotoo.cn@gmail.com"
        }
    ],
    "name": "pinyin",
    "optionalDependencies": {
        "nodejieba": "^2.2.1"
    },
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module pinyin](#apidoc.module.pinyin)
1.  [function <span class="apidocSignatureSpan">pinyin.</span>compare ()](#apidoc.element.pinyin.compare)
1.  [function <span class="apidocSignatureSpan">pinyin.</span>web_pinyin ()](#apidoc.element.pinyin.web_pinyin)
1.  number <span class="apidocSignatureSpan">pinyin.</span>STYLE_FIRST_LETTER
1.  number <span class="apidocSignatureSpan">pinyin.</span>STYLE_INITIALS
1.  number <span class="apidocSignatureSpan">pinyin.</span>STYLE_NORMAL
1.  number <span class="apidocSignatureSpan">pinyin.</span>STYLE_TO3NE
1.  number <span class="apidocSignatureSpan">pinyin.</span>STYLE_TONE
1.  number <span class="apidocSignatureSpan">pinyin.</span>STYLE_TONE2

#### [module pinyin.web_pinyin](#apidoc.module.pinyin.web_pinyin)
1.  [function <span class="apidocSignatureSpan">pinyin.</span>web_pinyin ()](#apidoc.element.pinyin.web_pinyin.web_pinyin)
1.  [function <span class="apidocSignatureSpan">pinyin.web_pinyin.</span>compare ()](#apidoc.element.pinyin.web_pinyin.compare)
1.  number <span class="apidocSignatureSpan">pinyin.web_pinyin.</span>STYLE_FIRST_LETTER
1.  number <span class="apidocSignatureSpan">pinyin.web_pinyin.</span>STYLE_INITIALS
1.  number <span class="apidocSignatureSpan">pinyin.web_pinyin.</span>STYLE_NORMAL
1.  number <span class="apidocSignatureSpan">pinyin.web_pinyin.</span>STYLE_TO3NE
1.  number <span class="apidocSignatureSpan">pinyin.web_pinyin.</span>STYLE_TONE
1.  number <span class="apidocSignatureSpan">pinyin.web_pinyin.</span>STYLE_TONE2



# <a name="apidoc.module.pinyin"></a>[module pinyin](#apidoc.module.pinyin)

#### <a name="apidoc.element.pinyin.compare"></a>[function <span class="apidocSignatureSpan">pinyin.</span>compare ()](#apidoc.element.pinyin.compare)
- description and source-code
```javascript
compare = function () { [native code] }
```
- example usage
```shell
...
将传入的中文字符串 (words) 转换成拼音符号串。

options 是可选的，可以设定拼音风格，或打开多音字选项。

返回二维数组，第一维每个数组项位置对应每个中文字符串位置。
第二维是各个汉字的读音列表，多音字会有多个拼音项。

### 方法 'Number pinyin.compare(a, b)'

按拼音排序的默认算法。

## 参数

### '<Boolean> options.segment'
...
```

#### <a name="apidoc.element.pinyin.web_pinyin"></a>[function <span class="apidocSignatureSpan">pinyin.</span>web_pinyin ()](#apidoc.element.pinyin.web_pinyin)
- description and source-code
```javascript
web_pinyin = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pinyin.web_pinyin"></a>[module pinyin.web_pinyin](#apidoc.module.pinyin.web_pinyin)

#### <a name="apidoc.element.pinyin.web_pinyin.web_pinyin"></a>[function <span class="apidocSignatureSpan">pinyin.</span>web_pinyin ()](#apidoc.element.pinyin.web_pinyin.web_pinyin)
- description and source-code
```javascript
web_pinyin = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pinyin.web_pinyin.compare"></a>[function <span class="apidocSignatureSpan">pinyin.web_pinyin.</span>compare ()](#apidoc.element.pinyin.web_pinyin.compare)
- description and source-code
```javascript
compare = function () { [native code] }
```
- example usage
```shell
...
将传入的中文字符串 (words) 转换成拼音符号串。

options 是可选的，可以设定拼音风格，或打开多音字选项。

返回二维数组，第一维每个数组项位置对应每个中文字符串位置。
第二维是各个汉字的读音列表，多音字会有多个拼音项。

### 方法 'Number pinyin.compare(a, b)'

按拼音排序的默认算法。

## 参数

### '<Boolean> options.segment'
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
