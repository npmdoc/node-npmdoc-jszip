# api documentation for  [jszip (v3.1.3)](https://github.com/Stuk/jszip#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-jszip.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jszip) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jszip.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jszip)
#### Create, read and edit .zip files with Javascript http://stuartk.com/jszip

[![NPM](https://nodei.co/npm/jszip.png?downloads=true)](https://www.npmjs.com/package/jszip)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jszip/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-jszip_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jszip/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jszip/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jszip/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Stuart Knightley",
        "email": "stuart@stuartk.com"
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
            "name": "cwmma",
            "email": "calvin.metcalf@gmail.com"
        },
        {
            "name": "dduponchel",
            "email": "d.duponchel@gmail.com"
        },
        {
            "name": "stuk",
            "email": "stuart@stuartk.com"
        }
    ],
    "name": "jszip",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "3.1.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module jszip](#apidoc.module.jszip)
1.  [function <span class="apidocSignatureSpan">jszip.</span>compressedObject (compressedSize, uncompressedSize, crc32, compression, data)](#apidoc.element.jszip.compressedObject)
1.  [function <span class="apidocSignatureSpan">jszip.</span>loadAsync (content, options)](#apidoc.element.jszip.loadAsync)
1.  [function <span class="apidocSignatureSpan">jszip.</span>zipEntries (loadOptions)](#apidoc.element.jszip.zipEntries)
1.  [function <span class="apidocSignatureSpan">jszip.</span>zipEntry (options, loadOptions)](#apidoc.element.jszip.zipEntry)
1.  [function <span class="apidocSignatureSpan">jszip.</span>zipObject (name, data, options)](#apidoc.element.jszip.zipObject)
1.  object <span class="apidocSignatureSpan">jszip.</span>base64
1.  object <span class="apidocSignatureSpan">jszip.</span>compressedObject.prototype
1.  object <span class="apidocSignatureSpan">jszip.</span>defaults
1.  object <span class="apidocSignatureSpan">jszip.</span>external
1.  object <span class="apidocSignatureSpan">jszip.</span>flate
1.  object <span class="apidocSignatureSpan">jszip.</span>nodejsUtils
1.  object <span class="apidocSignatureSpan">jszip.</span>support
1.  object <span class="apidocSignatureSpan">jszip.</span>utf8
1.  object <span class="apidocSignatureSpan">jszip.</span>utils
1.  object <span class="apidocSignatureSpan">jszip.</span>zipEntries.prototype
1.  object <span class="apidocSignatureSpan">jszip.</span>zipEntry.prototype
1.  object <span class="apidocSignatureSpan">jszip.</span>zipObject.prototype
1.  string <span class="apidocSignatureSpan">jszip.</span>version

#### [module jszip.base64](#apidoc.module.jszip.base64)
1.  [function <span class="apidocSignatureSpan">jszip.base64.</span>decode (input)](#apidoc.element.jszip.base64.decode)
1.  [function <span class="apidocSignatureSpan">jszip.base64.</span>encode (input)](#apidoc.element.jszip.base64.encode)

#### [module jszip.compressedObject](#apidoc.module.jszip.compressedObject)
1.  [function <span class="apidocSignatureSpan">jszip.</span>compressedObject (compressedSize, uncompressedSize, crc32, compression, data)](#apidoc.element.jszip.compressedObject.compressedObject)
1.  [function <span class="apidocSignatureSpan">jszip.compressedObject.</span>createWorkerFrom (uncompressedWorker, compression, compressionOptions)](#apidoc.element.jszip.compressedObject.createWorkerFrom)

#### [module jszip.compressedObject.prototype](#apidoc.module.jszip.compressedObject.prototype)
1.  [function <span class="apidocSignatureSpan">jszip.compressedObject.prototype.</span>getCompressedWorker ()](#apidoc.element.jszip.compressedObject.prototype.getCompressedWorker)
1.  [function <span class="apidocSignatureSpan">jszip.compressedObject.prototype.</span>getContentWorker ()](#apidoc.element.jszip.compressedObject.prototype.getContentWorker)

#### [module jszip.external](#apidoc.module.jszip.external)
1.  [function <span class="apidocSignatureSpan">jszip.external.</span>Promise ()](#apidoc.element.jszip.external.Promise)

#### [module jszip.flate](#apidoc.module.jszip.flate)
1.  [function <span class="apidocSignatureSpan">jszip.flate.</span>compressWorker (compressionOptions)](#apidoc.element.jszip.flate.compressWorker)
1.  [function <span class="apidocSignatureSpan">jszip.flate.</span>uncompressWorker ()](#apidoc.element.jszip.flate.uncompressWorker)
1.  string <span class="apidocSignatureSpan">jszip.flate.</span>magic

#### [module jszip.nodejsUtils](#apidoc.module.jszip.nodejsUtils)
1.  boolean <span class="apidocSignatureSpan">jszip.nodejsUtils.</span>isNode
1.  [function <span class="apidocSignatureSpan">jszip.nodejsUtils.</span>isBuffer (b)](#apidoc.element.jszip.nodejsUtils.isBuffer)
1.  [function <span class="apidocSignatureSpan">jszip.nodejsUtils.</span>isStream (obj)](#apidoc.element.jszip.nodejsUtils.isStream)
1.  [function <span class="apidocSignatureSpan">jszip.nodejsUtils.</span>newBuffer (data, encoding)](#apidoc.element.jszip.nodejsUtils.newBuffer)

#### [module jszip.utf8](#apidoc.module.jszip.utf8)
1.  [function <span class="apidocSignatureSpan">jszip.utf8.</span>Utf8DecodeWorker ()](#apidoc.element.jszip.utf8.Utf8DecodeWorker)
1.  [function <span class="apidocSignatureSpan">jszip.utf8.</span>Utf8EncodeWorker ()](#apidoc.element.jszip.utf8.Utf8EncodeWorker)
1.  [function <span class="apidocSignatureSpan">jszip.utf8.</span>utf8decode (buf)](#apidoc.element.jszip.utf8.utf8decode)
1.  [function <span class="apidocSignatureSpan">jszip.utf8.</span>utf8encode (str)](#apidoc.element.jszip.utf8.utf8encode)

#### [module jszip.utils](#apidoc.module.jszip.utils)
1.  [function <span class="apidocSignatureSpan">jszip.utils.</span>applyFromCharCode (array)](#apidoc.element.jszip.utils.applyFromCharCode)
1.  [function <span class="apidocSignatureSpan">jszip.utils.</span>checkSupport (type)](#apidoc.element.jszip.utils.checkSupport)
1.  [function <span class="apidocSignatureSpan">jszip.utils.</span>delay (callback, args, self)](#apidoc.element.jszip.utils.delay)
1.  [function <span class="apidocSignatureSpan">jszip.utils.</span>extend ()](#apidoc.element.jszip.utils.extend)
1.  [function <span class="apidocSignatureSpan">jszip.utils.</span>getTypeOf (input)](#apidoc.element.jszip.utils.getTypeOf)
1.  [function <span class="apidocSignatureSpan">jszip.utils.</span>inherits (ctor, superCtor)](#apidoc.element.jszip.utils.inherits)
1.  [function <span class="apidocSignatureSpan">jszip.utils.</span>newBlob (parts, type)](#apidoc.element.jszip.utils.newBlob)
1.  [function <span class="apidocSignatureSpan">jszip.utils.</span>prepareContent (name, inputData, isBinary, isOptimizedBinaryString, isBase64)](#apidoc.element.jszip.utils.prepareContent)
1.  [function <span class="apidocSignatureSpan">jszip.utils.</span>pretty (str)](#apidoc.element.jszip.utils.pretty)
1.  [function <span class="apidocSignatureSpan">jszip.utils.</span>transformTo (outputType, input)](#apidoc.element.jszip.utils.transformTo)
1.  number <span class="apidocSignatureSpan">jszip.utils.</span>MAX_VALUE_16BITS
1.  number <span class="apidocSignatureSpan">jszip.utils.</span>MAX_VALUE_32BITS

#### [module jszip.zipEntries](#apidoc.module.jszip.zipEntries)
1.  [function <span class="apidocSignatureSpan">jszip.</span>zipEntries (loadOptions)](#apidoc.element.jszip.zipEntries.zipEntries)

#### [module jszip.zipEntries.prototype](#apidoc.module.jszip.zipEntries.prototype)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>checkSignature (expectedSignature)](#apidoc.element.jszip.zipEntries.prototype.checkSignature)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>isSignature (askedIndex, expectedSignature)](#apidoc.element.jszip.zipEntries.prototype.isSignature)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>load (data)](#apidoc.element.jszip.zipEntries.prototype.load)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>prepareReader (data)](#apidoc.element.jszip.zipEntries.prototype.prepareReader)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>readBlockEndOfCentral ()](#apidoc.element.jszip.zipEntries.prototype.readBlockEndOfCentral)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>readBlockZip64EndOfCentral ()](#apidoc.element.jszip.zipEntries.prototype.readBlockZip64EndOfCentral)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>readBlockZip64EndOfCentralLocator ()](#apidoc.element.jszip.zipEntries.prototype.readBlockZip64EndOfCentralLocator)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>readCentralDir ()](#apidoc.element.jszip.zipEntries.prototype.readCentralDir)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>readEndOfCentral ()](#apidoc.element.jszip.zipEntries.prototype.readEndOfCentral)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>readLocalFiles ()](#apidoc.element.jszip.zipEntries.prototype.readLocalFiles)

#### [module jszip.zipEntry](#apidoc.module.jszip.zipEntry)
1.  [function <span class="apidocSignatureSpan">jszip.</span>zipEntry (options, loadOptions)](#apidoc.element.jszip.zipEntry.zipEntry)

#### [module jszip.zipEntry.prototype](#apidoc.module.jszip.zipEntry.prototype)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>findExtraFieldUnicodeComment ()](#apidoc.element.jszip.zipEntry.prototype.findExtraFieldUnicodeComment)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>findExtraFieldUnicodePath ()](#apidoc.element.jszip.zipEntry.prototype.findExtraFieldUnicodePath)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>handleUTF8 ()](#apidoc.element.jszip.zipEntry.prototype.handleUTF8)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>isEncrypted ()](#apidoc.element.jszip.zipEntry.prototype.isEncrypted)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>parseZIP64ExtraField (reader)](#apidoc.element.jszip.zipEntry.prototype.parseZIP64ExtraField)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>processAttributes ()](#apidoc.element.jszip.zipEntry.prototype.processAttributes)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>readCentralPart (reader)](#apidoc.element.jszip.zipEntry.prototype.readCentralPart)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>readExtraFields (reader)](#apidoc.element.jszip.zipEntry.prototype.readExtraFields)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>readLocalPart (reader)](#apidoc.element.jszip.zipEntry.prototype.readLocalPart)
1.  [function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>useUTF8 ()](#apidoc.element.jszip.zipEntry.prototype.useUTF8)

#### [module jszip.zipObject](#apidoc.module.jszip.zipObject)
1.  [function <span class="apidocSignatureSpan">jszip.</span>zipObject (name, data, options)](#apidoc.element.jszip.zipObject.zipObject)

#### [module jszip.zipObject.prototype](#apidoc.module.jszip.zipObject.prototype)
1.  [function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>_compressWorker (compression, compressionOptions)](#apidoc.element.jszip.zipObject.prototype._compressWorker)
1.  [function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>_decompressWorker ()](#apidoc.element.jszip.zipObject.prototype._decompressWorker)
1.  [function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>asArrayBuffer ()](#apidoc.element.jszip.zipObject.prototype.asArrayBuffer)
1.  [function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>asBinary ()](#apidoc.element.jszip.zipObject.prototype.asBinary)
1.  [function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>asNodeBuffer ()](#apidoc.element.jszip.zipObject.prototype.asNodeBuffer)
1.  [function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>asText ()](#apidoc.element.jszip.zipObject.prototype.asText)
1.  [function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>asUint8Array ()](#apidoc.element.jszip.zipObject.prototype.asUint8Array)
1.  [function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>async (type, onUpdate)](#apidoc.element.jszip.zipObject.prototype.async)
1.  [function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>internalStream (type)](#apidoc.element.jszip.zipObject.prototype.internalStream)
1.  [function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>nodeStream (type, onUpdate)](#apidoc.element.jszip.zipObject.prototype.nodeStream)



# <a name="apidoc.module.jszip"></a>[module jszip](#apidoc.module.jszip)

#### <a name="apidoc.element.jszip.compressedObject"></a>[function <span class="apidocSignatureSpan">jszip.</span>compressedObject (compressedSize, uncompressedSize, crc32, compression, data)](#apidoc.element.jszip.compressedObject)
- description and source-code
```javascript
function CompressedObject(compressedSize, uncompressedSize, crc32, compression, data) {
    this.compressedSize = compressedSize;
    this.uncompressedSize = uncompressedSize;
    this.crc32 = crc32;
    this.compression = compression;
    this.compressedContent = data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jszip.loadAsync"></a>[function <span class="apidocSignatureSpan">jszip.</span>loadAsync (content, options)](#apidoc.element.jszip.loadAsync)
- description and source-code
```javascript
loadAsync = function (content, options) {
    return new JSZip().loadAsync(content, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jszip.zipEntries"></a>[function <span class="apidocSignatureSpan">jszip.</span>zipEntries (loadOptions)](#apidoc.element.jszip.zipEntries)
- description and source-code
```javascript
function ZipEntries(loadOptions) {
    this.files = [];
    this.loadOptions = loadOptions;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jszip.zipEntry"></a>[function <span class="apidocSignatureSpan">jszip.</span>zipEntry (options, loadOptions)](#apidoc.element.jszip.zipEntry)
- description and source-code
```javascript
function ZipEntry(options, loadOptions) {
    this.options = options;
    this.loadOptions = loadOptions;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jszip.zipObject"></a>[function <span class="apidocSignatureSpan">jszip.</span>zipObject (name, data, options)](#apidoc.element.jszip.zipObject)
- description and source-code
```javascript
zipObject = function (name, data, options) {
    this.name = name;
    this.dir = options.dir;
    this.date = options.date;
    this.comment = options.comment;
    this.unixPermissions = options.unixPermissions;
    this.dosPermissions = options.dosPermissions;

    this._data = data;
    this._dataBinary = options.binary;
    // keep only the compression
    this.options = {
        compression : options.compression,
        compressionOptions : options.compressionOptions
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jszip.base64"></a>[module jszip.base64](#apidoc.module.jszip.base64)

#### <a name="apidoc.element.jszip.base64.decode"></a>[function <span class="apidocSignatureSpan">jszip.base64.</span>decode (input)](#apidoc.element.jszip.base64.decode)
- description and source-code
```javascript
decode = function (input) {
    var chr1, chr2, chr3;
    var enc1, enc2, enc3, enc4;
    var i = 0, resultIndex = 0;

    var dataUrlPrefix = "data:";

    if (input.substr(0, dataUrlPrefix.length) === dataUrlPrefix) {
        // This is a common error: people give a data url
        // (data:image/png;base64,iVBOR...) with a {base64: true} and
        // wonders why things don't work.
        // We can detect that the string input looks like a data url but we
        // *can't* be sure it is one: removing everything up to the comma would
        // be too dangerous.
        throw new Error("Invalid base64 input, it looks like a data url.");
    }

    input = input.replace(/[^A-Za-z0-9\+\/\=]/g, "");

    var totalLength = input.length * 3 / 4;
    if(input.charAt(input.length - 1) === _keyStr.charAt(64)) {
        totalLength--;
    }
    if(input.charAt(input.length - 2) === _keyStr.charAt(64)) {
        totalLength--;
    }
    if (totalLength % 1 !== 0) {
        // totalLength is not an integer, the length does not match a valid
        // base64 content. That can happen if:
        // - the input is not a base64 content
        // - the input is *almost* a base64 content, with a extra chars at the
        //   beginning or at the end
        // - the input uses a base64 variant (base64url for example)
        throw new Error("Invalid base64 input, bad content length.");
    }
    var output;
    if (support.uint8array) {
        output = new Uint8Array(totalLength|0);
    } else {
        output = new Array(totalLength|0);
    }

    while (i < input.length) {

        enc1 = _keyStr.indexOf(input.charAt(i++));
        enc2 = _keyStr.indexOf(input.charAt(i++));
        enc3 = _keyStr.indexOf(input.charAt(i++));
        enc4 = _keyStr.indexOf(input.charAt(i++));

        chr1 = (enc1 << 2) | (enc2 >> 4);
        chr2 = ((enc2 & 15) << 4) | (enc3 >> 2);
        chr3 = ((enc3 & 3) << 6) | enc4;

        output[resultIndex++] = chr1;

        if (enc3 !== 64) {
            output[resultIndex++] = chr2;
        }
        if (enc4 !== 64) {
            output[resultIndex++] = chr3;
        }

    }

    return output;
}
```
- example usage
```shell
...
    );
}
// special case : it's way easier to work with Uint8Array than with ArrayBuffer
if (dataType === "arraybuffer") {
    data = exports.transformTo("uint8array", data);
} else if (dataType === "string") {
    if (isBase64) {
        data = base64.decode(data);
    }
    else if (isBinary) {
        // optimizedBinaryString === true means that the file has already been filtered with a 0xFF mask
        if (isOptimizedBinaryString !== true) {
            // this is a string, not in a base64 format.
            // Be sure that this is a correct "binary string"
            data = string2binary(data);
...
```

#### <a name="apidoc.element.jszip.base64.encode"></a>[function <span class="apidocSignatureSpan">jszip.base64.</span>encode (input)](#apidoc.element.jszip.base64.encode)
- description and source-code
```javascript
encode = function (input) {
    var output = [];
    var chr1, chr2, chr3, enc1, enc2, enc3, enc4;
    var i = 0, len = input.length, remainingBytes = len;

    var isArray = utils.getTypeOf(input) !== "string";
    while (i < input.length) {
        remainingBytes = len - i;

        if (!isArray) {
            chr1 = input.charCodeAt(i++);
            chr2 = i < len ? input.charCodeAt(i++) : 0;
            chr3 = i < len ? input.charCodeAt(i++) : 0;
        } else {
            chr1 = input[i++];
            chr2 = i < len ? input[i++] : 0;
            chr3 = i < len ? input[i++] : 0;
        }

        enc1 = chr1 >> 2;
        enc2 = ((chr1 & 3) << 4) | (chr2 >> 4);
        enc3 = remainingBytes > 1 ? (((chr2 & 15) << 2) | (chr3 >> 6)) : 64;
        enc4 = remainingBytes > 2 ? (chr3 & 63) : 64;

        output.push(_keyStr.charAt(enc1) + _keyStr.charAt(enc2) + _keyStr.charAt(enc3) + _keyStr.charAt(enc4));

    }

    return output.join("");
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jszip.compressedObject"></a>[module jszip.compressedObject](#apidoc.module.jszip.compressedObject)

#### <a name="apidoc.element.jszip.compressedObject.compressedObject"></a>[function <span class="apidocSignatureSpan">jszip.</span>compressedObject (compressedSize, uncompressedSize, crc32, compression, data)](#apidoc.element.jszip.compressedObject.compressedObject)
- description and source-code
```javascript
function CompressedObject(compressedSize, uncompressedSize, crc32, compression, data) {
    this.compressedSize = compressedSize;
    this.uncompressedSize = uncompressedSize;
    this.crc32 = crc32;
    this.compression = compression;
    this.compressedContent = data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jszip.compressedObject.createWorkerFrom"></a>[function <span class="apidocSignatureSpan">jszip.compressedObject.</span>createWorkerFrom (uncompressedWorker, compression, compressionOptions)](#apidoc.element.jszip.compressedObject.createWorkerFrom)
- description and source-code
```javascript
createWorkerFrom = function (uncompressedWorker, compression, compressionOptions) {
    return uncompressedWorker
    .pipe(new Crc32Probe())
    .pipe(new DataLengthProbe("uncompressedSize"))
    .pipe(compression.compressWorker(compressionOptions))
    .pipe(new DataLengthProbe("compressedSize"))
    .withStreamInfo("compression", compression);
}
```
- example usage
```shell
...
    ) {
        return this._data.getCompressedWorker();
    } else {
        var result = this._decompressWorker();
        if(!this._dataBinary) {
            result = result.pipe(new utf8.Utf8EncodeWorker());
        }
        return CompressedObject.createWorkerFrom(result, compression, compressionOptions);
    }
},
/**
 * Return a worker for the decompressed content.
 * @private
 * @return Worker the worker.
 */
...
```



# <a name="apidoc.module.jszip.compressedObject.prototype"></a>[module jszip.compressedObject.prototype](#apidoc.module.jszip.compressedObject.prototype)

#### <a name="apidoc.element.jszip.compressedObject.prototype.getCompressedWorker"></a>[function <span class="apidocSignatureSpan">jszip.compressedObject.prototype.</span>getCompressedWorker ()](#apidoc.element.jszip.compressedObject.prototype.getCompressedWorker)
- description and source-code
```javascript
getCompressedWorker = function () {
    return new DataWorker(external.Promise.resolve(this.compressedContent))
    .withStreamInfo("compressedSize", this.compressedSize)
    .withStreamInfo("uncompressedSize", this.uncompressedSize)
    .withStreamInfo("crc32", this.crc32)
    .withStreamInfo("compression", this.compression)
    ;
}
```
- example usage
```shell
...
 * @return Worker the worker.
 */
_compressWorker: function (compression, compressionOptions) {
    if (
        this._data instanceof CompressedObject &&
        this._data.compression.magic === compression.magic
    ) {
        return this._data.getCompressedWorker();
    } else {
        var result = this._decompressWorker();
        if(!this._dataBinary) {
            result = result.pipe(new utf8.Utf8EncodeWorker());
        }
        return CompressedObject.createWorkerFrom(result, compression, compressionOptions);
    }
...
```

#### <a name="apidoc.element.jszip.compressedObject.prototype.getContentWorker"></a>[function <span class="apidocSignatureSpan">jszip.compressedObject.prototype.</span>getContentWorker ()](#apidoc.element.jszip.compressedObject.prototype.getContentWorker)
- description and source-code
```javascript
getContentWorker = function () {
    var worker = new DataWorker(external.Promise.resolve(this.compressedContent))
    .pipe(this.compression.uncompressWorker())
    .pipe(new DataLengthProbe("data_length"));

    var that = this;
    worker.on("end", function () {
        if(this.streamInfo['data_length'] !== that.uncompressedSize) {
            throw new Error("Bug : uncompressed data size mismatch");
        }
    });
    return worker;
}
```
- example usage
```shell
...
/**
 * Check the CRC32 of an entry.
 * @param {ZipEntry} zipEntry the zip entry to check.
 * @return {Promise} the result.
 */
function checkEntryCRC32(zipEntry) {
return new external.Promise(function (resolve, reject) {
    var worker = zipEntry.decompressed.getContentWorker().pipe(new Crc32Probe());
    worker.on("error", function (e) {
        reject(e);
    })
    .on("end", function () {
        if (worker.streamInfo.crc32 !== zipEntry.decompressed.crc32) {
            reject(new Error("Corrupted zip : CRC32 mismatch"));
        } else {
...
```



# <a name="apidoc.module.jszip.external"></a>[module jszip.external](#apidoc.module.jszip.external)

#### <a name="apidoc.element.jszip.external.Promise"></a>[function <span class="apidocSignatureSpan">jszip.external.</span>Promise ()](#apidoc.element.jszip.external.Promise)
- description and source-code
```javascript
function Promise() { [native code] }
```
- example usage
```shell
...

/**
 * Check the CRC32 of an entry.
 * @param {ZipEntry} zipEntry the zip entry to check.
 * @return {Promise} the result.
 */
function checkEntryCRC32(zipEntry) {
return new external.Promise(function (resolve, reject) {
    var worker = zipEntry.decompressed.getContentWorker().pipe(new Crc32Probe());
    worker.on("error", function (e) {
        reject(e);
    })
    .on("end", function () {
        if (worker.streamInfo.crc32 !== zipEntry.decompressed.crc32) {
            reject(new Error("Corrupted zip : CRC32 mismatch"));
...
```



# <a name="apidoc.module.jszip.flate"></a>[module jszip.flate](#apidoc.module.jszip.flate)

#### <a name="apidoc.element.jszip.flate.compressWorker"></a>[function <span class="apidocSignatureSpan">jszip.flate.</span>compressWorker (compressionOptions)](#apidoc.element.jszip.flate.compressWorker)
- description and source-code
```javascript
compressWorker = function (compressionOptions) {
    return new FlateWorker("Deflate", compressionOptions);
}
```
- example usage
```shell
...
 * @param {Object} compressionOptions the options to use when compressing.
 * @return {GenericWorker} the new worker compressing the content.
 */
CompressedObject.createWorkerFrom = function (uncompressedWorker, compression, compressionOptions) {
    return uncompressedWorker
    .pipe(new Crc32Probe())
    .pipe(new DataLengthProbe("uncompressedSize"))
    .pipe(compression.compressWorker(compressionOptions))
    .pipe(new DataLengthProbe("compressedSize"))
    .withStreamInfo("compression", compression);
};

module.exports = CompressedObject;
...
```

#### <a name="apidoc.element.jszip.flate.uncompressWorker"></a>[function <span class="apidocSignatureSpan">jszip.flate.</span>uncompressWorker ()](#apidoc.element.jszip.flate.uncompressWorker)
- description and source-code
```javascript
uncompressWorker = function () {
    return new FlateWorker("Inflate", {});
}
```
- example usage
```shell
...
CompressedObject.prototype = {
    /**
     * Create a worker to get the uncompressed content.
     * @return {GenericWorker} the worker.
     */
    getContentWorker : function () {
var worker = new DataWorker(external.Promise.resolve(this.compressedContent))
.pipe(this.compression.uncompressWorker())
.pipe(new DataLengthProbe("data_length"));

var that = this;
worker.on("end", function () {
    if(this.streamInfo['data_length'] !== that.uncompressedSize) {
        throw new Error("Bug : uncompressed data size mismatch");
    }
...
```



# <a name="apidoc.module.jszip.nodejsUtils"></a>[module jszip.nodejsUtils](#apidoc.module.jszip.nodejsUtils)

#### <a name="apidoc.element.jszip.nodejsUtils.isBuffer"></a>[function <span class="apidocSignatureSpan">jszip.nodejsUtils.</span>isBuffer (b)](#apidoc.element.jszip.nodejsUtils.isBuffer)
- description and source-code
```javascript
isBuffer = function (b){
    return Buffer.isBuffer(b);
}
```
- example usage
```shell
...
},
/**
 * Find out if an object is a Buffer.
 * @param {Object} b the object to test.
 * @return {Boolean} true if the object is a Buffer, false otherwise.
 */
isBuffer : function(b){
    return Buffer.isBuffer(b);
},

isStream : function (obj) {
    return obj &&
        typeof obj.on === "function" &&
        typeof obj.pause === "function" &&
        typeof obj.resume === "function";
...
```

#### <a name="apidoc.element.jszip.nodejsUtils.isStream"></a>[function <span class="apidocSignatureSpan">jszip.nodejsUtils.</span>isStream (obj)](#apidoc.element.jszip.nodejsUtils.isStream)
- description and source-code
```javascript
isStream = function (obj) {
    return obj &&
        typeof obj.on === "function" &&
        typeof obj.pause === "function" &&
        typeof obj.resume === "function";
}
```
- example usage
```shell
...
    base64: false,
    checkCRC32: false,
    optimizedBinaryString: false,
    createFolders: false,
    decodeFileName: utf8.utf8decode
});

if (nodejsUtils.isNode && nodejsUtils.isStream(data)) {
    return external.Promise.reject(new Error("JSZip can't accept a stream when loading a zip file."));
}

return utils.prepareContent("the loaded zip file", data, true, options.optimizedBinaryString, options.base64)
.then(function(data) {
    var zipEntries = new ZipEntries(options);
    zipEntries.load(data);
...
```

#### <a name="apidoc.element.jszip.nodejsUtils.newBuffer"></a>[function <span class="apidocSignatureSpan">jszip.nodejsUtils.</span>newBuffer (data, encoding)](#apidoc.element.jszip.nodejsUtils.newBuffer)
- description and source-code
```javascript
newBuffer = function (data, encoding){
    return new Buffer(data, encoding);
}
```
- example usage
```shell
...
 * Transform a javascript string into an array (typed if possible) of bytes,
 * UTF-8 encoded.
 * @param {String} str the string to encode
 * @return {Array|Uint8Array|Buffer} the UTF-8 encoded string.
 */
exports.utf8encode = function utf8encode(str) {
    if (support.nodebuffer) {
        return nodejsUtils.newBuffer(str, "utf-8");
    }

    return string2buf(str);
};


/**
...
```



# <a name="apidoc.module.jszip.utf8"></a>[module jszip.utf8](#apidoc.module.jszip.utf8)

#### <a name="apidoc.element.jszip.utf8.Utf8DecodeWorker"></a>[function <span class="apidocSignatureSpan">jszip.utf8.</span>Utf8DecodeWorker ()](#apidoc.element.jszip.utf8.Utf8DecodeWorker)
- description and source-code
```javascript
function Utf8DecodeWorker() {
    GenericWorker.call(this, "utf-8 decode");
    // the last bytes if a chunk didn't end with a complete codepoint.
    this.leftOver = null;
}
```
- example usage
```shell
...

    var isUnicodeString = !this._dataBinary;

    if (isUnicodeString && !askUnicodeString) {
        result = result.pipe(new utf8.Utf8EncodeWorker());
    }
    if (!isUnicodeString && askUnicodeString) {
        result = result.pipe(new utf8.Utf8DecodeWorker());
    }

    return new StreamHelper(result, outputType, "");
},

/**
 * Prepare the content in the asked type.
...
```

#### <a name="apidoc.element.jszip.utf8.Utf8EncodeWorker"></a>[function <span class="apidocSignatureSpan">jszip.utf8.</span>Utf8EncodeWorker ()](#apidoc.element.jszip.utf8.Utf8EncodeWorker)
- description and source-code
```javascript
function Utf8EncodeWorker() {
    GenericWorker.call(this, "utf-8 encode");
}
```
- example usage
```shell
...
        outputType = "string";
    }
    var result = this._decompressWorker();

    var isUnicodeString = !this._dataBinary;

    if (isUnicodeString && !askUnicodeString) {
        result = result.pipe(new utf8.Utf8EncodeWorker());
    }
    if (!isUnicodeString && askUnicodeString) {
        result = result.pipe(new utf8.Utf8DecodeWorker());
    }

    return new StreamHelper(result, outputType, "");
},
...
```

#### <a name="apidoc.element.jszip.utf8.utf8decode"></a>[function <span class="apidocSignatureSpan">jszip.utf8.</span>utf8decode (buf)](#apidoc.element.jszip.utf8.utf8decode)
- description and source-code
```javascript
function utf8decode(buf) {
    if (support.nodebuffer) {
        return utils.transformTo("nodebuffer", buf).toString("utf-8");
    }

    buf = utils.transformTo(support.uint8array ? "uint8array" : "array", buf);

    return buf2string(buf);
}
```
- example usage
```shell
...
       } else {
           usableData = data.slice(0, nextBoundary);
           this.leftOver = data.slice(nextBoundary, data.length);
       }
   }

   this.push({
       data : exports.utf8decode(usableData),
       meta : chunk.meta
   });
};

/**
* @see GenericWorker.flush
*/
...
```

#### <a name="apidoc.element.jszip.utf8.utf8encode"></a>[function <span class="apidocSignatureSpan">jszip.utf8.</span>utf8encode (str)](#apidoc.element.jszip.utf8.utf8encode)
- description and source-code
```javascript
function utf8encode(str) {
    if (support.nodebuffer) {
        return nodejsUtils.newBuffer(str, "utf-8");
    }

    return string2buf(str);
}
```
- example usage
```shell
...
utils.inherits(Utf8EncodeWorker, GenericWorker);

/**
 * @see GenericWorker.processChunk
 */
Utf8EncodeWorker.prototype.processChunk = function (chunk) {
    this.push({
        data : exports.utf8encode(chunk.data),
        meta : chunk.meta
    });
};
exports.Utf8EncodeWorker = Utf8EncodeWorker;
...
```



# <a name="apidoc.module.jszip.utils"></a>[module jszip.utils](#apidoc.module.jszip.utils)

#### <a name="apidoc.element.jszip.utils.applyFromCharCode"></a>[function <span class="apidocSignatureSpan">jszip.utils.</span>applyFromCharCode (array)](#apidoc.element.jszip.utils.applyFromCharCode)
- description and source-code
```javascript
function arrayLikeToString(array) {
    // Performances notes :
    // --------------------
    // String.fromCharCode.apply(null, array) is the fastest, see
    // see http://jsperf.com/converting-a-uint8array-to-a-string/2
    // but the stack is limited (and we can get huge arrays !).
    //
    // result += String.fromCharCode(array[i]); generate too many strings !
    //
    // This code is inspired by http://jsperf.com/arraybuffer-to-string-apply-performance/2
    // TODO : we now have workers that split the work. Do we still need that ?
    var chunk = 65536,
        type = exports.getTypeOf(array),
        canUseApply = true;
    if (type === "uint8array") {
        canUseApply = arrayToStringHelper.applyCanBeUsed.uint8array;
    } else if (type === "nodebuffer") {
        canUseApply = arrayToStringHelper.applyCanBeUsed.nodebuffer;
    }

    if (canUseApply) {
        while (chunk > 1) {
            try {
                return arrayToStringHelper.stringifyByChunk(array, type, chunk);
            } catch (e) {
                chunk = Math.floor(chunk / 2);
            }
        }
    }

    // no apply or chunk error : slow and painful algorithm
    // default browser on android 4.*
    return arrayToStringHelper.stringifyByChar(array);
}
```
- example usage
```shell
...
            utf16buf = utf16buf.subarray(0, out);
        } else {
            utf16buf.length = out;
        }
    }

    // return String.fromCharCode.apply(null, utf16buf);
    return utils.applyFromCharCode(utf16buf);
};


// That's all for the pako functions.


/**
...
```

#### <a name="apidoc.element.jszip.utils.checkSupport"></a>[function <span class="apidocSignatureSpan">jszip.utils.</span>checkSupport (type)](#apidoc.element.jszip.utils.checkSupport)
- description and source-code
```javascript
checkSupport = function (type) {
    var supported = support[type.toLowerCase()];
    if (!supported) {
        throw new Error(type + " is not supported by this platform");
    }
}
```
- example usage
```shell
...
 * @param {Array[String|ArrayBuffer]} parts the content to put in the blob. DO NOT use
 * an Uint8Array because the stock browser of android 4 won't accept it (it
 * will be silently converted to a string, "[object Uint8Array]").
 * @param {String} type the mime type of the blob.
 * @return {Blob} the created blob.
 */
exports.newBlob = function(parts, type) {
exports.checkSupport("blob");

try {
    // Blob constructor
    return new Blob(parts, {
        type: type
    });
}
...
```

#### <a name="apidoc.element.jszip.utils.delay"></a>[function <span class="apidocSignatureSpan">jszip.utils.</span>delay (callback, args, self)](#apidoc.element.jszip.utils.delay)
- description and source-code
```javascript
delay = function (callback, args, self) {
    setImmediate(function () {
        callback.apply(self || null, args || []);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jszip.utils.extend"></a>[function <span class="apidocSignatureSpan">jszip.utils.</span>extend ()](#apidoc.element.jszip.utils.extend)
- description and source-code
```javascript
extend = function () {
    var result = {}, i, attr;
    for (i = 0; i < arguments.length; i++) { // arguments is not enumerable in some browsers
        for (attr in arguments[i]) {
            if (arguments[i].hasOwnProperty(attr) && typeof result[attr] === "undefined") {
                result[attr] = arguments[i][attr];
            }
        }
    }
    return result;
}
```
- example usage
```shell
...
    })
    .resume();
});
}

module.exports = function(data, options) {
var zip = this;
options = utils.extend(options || {}, {
    base64: false,
    checkCRC32: false,
    optimizedBinaryString: false,
    createFolders: false,
    decodeFileName: utf8.utf8decode
});
...
```

#### <a name="apidoc.element.jszip.utils.getTypeOf"></a>[function <span class="apidocSignatureSpan">jszip.utils.</span>getTypeOf (input)](#apidoc.element.jszip.utils.getTypeOf)
- description and source-code
```javascript
getTypeOf = function (input) {
    if (typeof input === "string") {
        return "string";
    }
    if (Object.prototype.toString.call(input) === "[object Array]") {
        return "array";
    }
    if (support.nodebuffer && nodejsUtils.isBuffer(input)) {
        return "nodebuffer";
    }
    if (support.uint8array && input instanceof Uint8Array) {
        return "uint8array";
    }
    if (support.arraybuffer && input instanceof ArrayBuffer) {
        return "arraybuffer";
    }
}
```
- example usage
```shell
...

// public method for encoding
exports.encode = function(input) {
    var output = [];
    var chr1, chr2, chr3, enc1, enc2, enc3, enc4;
    var i = 0, len = input.length, remainingBytes = len;

    var isArray = utils.getTypeOf(input) !== "string";
    while (i < input.length) {
remainingBytes = len - i;

if (!isArray) {
    chr1 = input.charCodeAt(i++);
    chr2 = i < len ? input.charCodeAt(i++) : 0;
    chr3 = i < len ? input.charCodeAt(i++) : 0;
...
```

#### <a name="apidoc.element.jszip.utils.inherits"></a>[function <span class="apidocSignatureSpan">jszip.utils.</span>inherits (ctor, superCtor)](#apidoc.element.jszip.utils.inherits)
- description and source-code
```javascript
inherits = function (ctor, superCtor) {
    var Obj = function() {};
    Obj.prototype = superCtor.prototype;
    ctor.prototype = new Obj();
}
```
- example usage
```shell
...
    self.push({
        data : data,
        meta : self.meta
    });
};
}

utils.inherits(FlateWorker, GenericWorker);

/**
 * @see GenericWorker.processChunk
 */
FlateWorker.prototype.processChunk = function (chunk) {
this.meta = chunk.meta;
this._pako.push(utils.transformTo(ARRAY_TYPE, chunk.data), false);
...
```

#### <a name="apidoc.element.jszip.utils.newBlob"></a>[function <span class="apidocSignatureSpan">jszip.utils.</span>newBlob (parts, type)](#apidoc.element.jszip.utils.newBlob)
- description and source-code
```javascript
newBlob = function (parts, type) {
    exports.checkSupport("blob");

    try {
        // Blob constructor
        return new Blob(parts, {
            type: type
        });
    }
    catch (e) {

        try {
            // deprecated, browser only, old way
            var Builder = window.BlobBuilder || window.WebKitBlobBuilder || window.MozBlobBuilder || window.MSBlobBuilder;
            var builder = new Builder();
            for (var i = 0; i < parts.length; i++) {
                builder.append(parts[i]);
            }
            return builder.getBlob(type);
        }
        catch (e) {

            // well, fuck ?!
            throw new Error("Bug : can't construct the Blob.");
        }
    }


}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jszip.utils.prepareContent"></a>[function <span class="apidocSignatureSpan">jszip.utils.</span>prepareContent (name, inputData, isBinary, isOptimizedBinaryString, isBase64)](#apidoc.element.jszip.utils.prepareContent)
- description and source-code
```javascript
prepareContent = function (name, inputData, isBinary, isOptimizedBinaryString, isBase64) {

    // if inputData is already a promise, this flatten it.
    var promise = external.Promise.resolve(inputData).then(function(data) {


        var isBlob = support.blob && (data instanceof Blob || ['[object File]', '[object Blob]'].indexOf(Object.prototype.toString
.call(data)) !== -1);

        if (isBlob && typeof FileReader !== "undefined") {
            return new external.Promise(function (resolve, reject) {
                var reader = new FileReader();

                reader.onload = function(e) {
                    resolve(e.target.result);
                };
                reader.onerror = function(e) {
                    reject(e.target.error);
                };
                reader.readAsArrayBuffer(data);
            });
        } else {
            return data;
        }
    });

    return promise.then(function(data) {
        var dataType = exports.getTypeOf(data);

        if (!dataType) {
            return external.Promise.reject(
                new Error("The data of '" + name + "' is in an unsupported format !")
            );
        }
        // special case : it's way easier to work with Uint8Array than with ArrayBuffer
        if (dataType === "arraybuffer") {
            data = exports.transformTo("uint8array", data);
        } else if (dataType === "string") {
            if (isBase64) {
                data = base64.decode(data);
            }
            else if (isBinary) {
                // optimizedBinaryString === true means that the file has already been filtered with a 0xFF mask
                if (isOptimizedBinaryString !== true) {
                    // this is a string, not in a base64 format.
                    // Be sure that this is a correct "binary string"
                    data = string2binary(data);
                }
            }
        }
        return data;
    });
}
```
- example usage
```shell
...
    decodeFileName: utf8.utf8decode
});

if (nodejsUtils.isNode && nodejsUtils.isStream(data)) {
    return external.Promise.reject(new Error("JSZip can't accept a stream when loading a zip file."));
}

return utils.prepareContent("the loaded zip file", data, true, options.optimizedBinaryString, options.base64)
.then(function(data) {
    var zipEntries = new ZipEntries(options);
    zipEntries.load(data);
    return zipEntries;
}).then(function checkCRC32(zipEntries) {
    var promises = [external.Promise.resolve(zipEntries)];
    var files = zipEntries.files;
...
```

#### <a name="apidoc.element.jszip.utils.pretty"></a>[function <span class="apidocSignatureSpan">jszip.utils.</span>pretty (str)](#apidoc.element.jszip.utils.pretty)
- description and source-code
```javascript
pretty = function (str) {
    var res = '',
        code, i;
    for (i = 0; i < (str || "").length; i++) {
        code = str.charCodeAt(i);
        res += '\\x' + (code < 16 ? "0" : "") + code.toString(16).toUpperCase();
    }
    return res;
}
```
- example usage
```shell
...
 * @param {string} expectedSignature the expected signature.
 * @throws {Error} if it is an other signature.
 */
checkSignature: function(expectedSignature) {
    if (!this.reader.readAndCheckSignature(expectedSignature)) {
        this.reader.index -= 4;
        var signature = this.reader.readString(4);
        throw new Error("Corrupted zip or bug : unexpected signature " + "(" + utils.pretty(signature) + ", expected " + utils.pretty
(expectedSignature) + ")");
    }
},
/**
 * Check if the given signature is at the given index.
 * @param {number} askedIndex the index to check.
 * @param {string} expectedSignature the signature to expect.
 * @return {boolean} true if the signature is here, false otherwise.
...
```

#### <a name="apidoc.element.jszip.utils.transformTo"></a>[function <span class="apidocSignatureSpan">jszip.utils.</span>transformTo (outputType, input)](#apidoc.element.jszip.utils.transformTo)
- description and source-code
```javascript
transformTo = function (outputType, input) {
    if (!input) {
        // undefined, null, etc
        // an empty string won't harm.
        input = "";
    }
    if (!outputType) {
        return input;
    }
    exports.checkSupport(outputType);
    var inputType = exports.getTypeOf(input);
    var result = transform[inputType][outputType](input);
    return result;
}
```
- example usage
```shell
...
utils.inherits(FlateWorker, GenericWorker);

/**
 * @see GenericWorker.processChunk
 */
FlateWorker.prototype.processChunk = function (chunk) {
this.meta = chunk.meta;
this._pako.push(utils.transformTo(ARRAY_TYPE, chunk.data), false);
};

/**
 * @see GenericWorker.flush
 */
FlateWorker.prototype.flush = function () {
GenericWorker.prototype.flush.call(this);
...
```



# <a name="apidoc.module.jszip.zipEntries"></a>[module jszip.zipEntries](#apidoc.module.jszip.zipEntries)

#### <a name="apidoc.element.jszip.zipEntries.zipEntries"></a>[function <span class="apidocSignatureSpan">jszip.</span>zipEntries (loadOptions)](#apidoc.element.jszip.zipEntries.zipEntries)
- description and source-code
```javascript
function ZipEntries(loadOptions) {
    this.files = [];
    this.loadOptions = loadOptions;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jszip.zipEntries.prototype"></a>[module jszip.zipEntries.prototype](#apidoc.module.jszip.zipEntries.prototype)

#### <a name="apidoc.element.jszip.zipEntries.prototype.checkSignature"></a>[function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>checkSignature (expectedSignature)](#apidoc.element.jszip.zipEntries.prototype.checkSignature)
- description and source-code
```javascript
checkSignature = function (expectedSignature) {
    if (!this.reader.readAndCheckSignature(expectedSignature)) {
        this.reader.index -= 4;
        var signature = this.reader.readString(4);
        throw new Error("Corrupted zip or bug : unexpected signature " + "(" + utils.pretty(signature) + ", expected " + utils.pretty
(expectedSignature) + ")");
    }
}
```
- example usage
```shell
...
 * Read the local files, based on the offset read in the central part.
 */
readLocalFiles: function() {
    var i, file;
    for (i = 0; i < this.files.length; i++) {
        file = this.files[i];
        this.reader.setIndex(file.localHeaderOffset);
        this.checkSignature(sig.LOCAL_FILE_HEADER);
        file.readLocalPart(this.reader);
        file.handleUTF8();
        file.processAttributes();
    }
},
/**
 * Read the central directory.
...
```

#### <a name="apidoc.element.jszip.zipEntries.prototype.isSignature"></a>[function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>isSignature (askedIndex, expectedSignature)](#apidoc.element.jszip.zipEntries.prototype.isSignature)
- description and source-code
```javascript
isSignature = function (askedIndex, expectedSignature) {
    var currentIndex = this.reader.index;
    this.reader.setIndex(askedIndex);
    var signature = this.reader.readString(4);
    var result = signature === expectedSignature;
    this.reader.setIndex(currentIndex);
    return result;
}
```
- example usage
```shell
...
        var offset = this.reader.lastIndexOfSignature(sig.CENTRAL_DIRECTORY_END);
        if (offset < 0) {
// Check if the content is a truncated zip or complete garbage.
// A "LOCAL_FILE_HEADER" is not required at the beginning (auto
// extractible zip for example) but it can give a good hint.
// If an ajax request was used without responseType, we will also
// get unreadable data.
var isGarbage = !this.isSignature(0, sig.LOCAL_FILE_HEADER);

if (isGarbage) {
    throw new Error("Can't find end of central directory : is this a zip file ? " +
                    "If it is, see http://stuk.github.io/jszip/documentation/howto/read_zip.html");
} else {
    throw new Error("Corrupted zip : can't find end of central directory");
}
...
```

#### <a name="apidoc.element.jszip.zipEntries.prototype.load"></a>[function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>load (data)](#apidoc.element.jszip.zipEntries.prototype.load)
- description and source-code
```javascript
load = function (data) {
    this.prepareReader(data);
    this.readEndOfCentral();
    this.readCentralDir();
    this.readLocalFiles();
}
```
- example usage
```shell
...
if (nodejsUtils.isNode && nodejsUtils.isStream(data)) {
    return external.Promise.reject(new Error("JSZip can't accept a stream when loading a zip file."));
}

return utils.prepareContent("the loaded zip file", data, true, options.optimizedBinaryString, options.base64)
.then(function(data) {
    var zipEntries = new ZipEntries(options);
    zipEntries.load(data);
    return zipEntries;
}).then(function checkCRC32(zipEntries) {
    var promises = [external.Promise.resolve(zipEntries)];
    var files = zipEntries.files;
    if (options.checkCRC32) {
        for (var i = 0; i < files.length; i++) {
            promises.push(checkEntryCRC32(files[i]));
...
```

#### <a name="apidoc.element.jszip.zipEntries.prototype.prepareReader"></a>[function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>prepareReader (data)](#apidoc.element.jszip.zipEntries.prototype.prepareReader)
- description and source-code
```javascript
prepareReader = function (data) {
    this.reader = readerFor(data);
}
```
- example usage
```shell
...
        this.reader = readerFor(data);
    },
    /**
     * Read a zip file and create ZipEntries.
     * @param {String|ArrayBuffer|Uint8Array|Buffer} data the binary string representing a zip file.
     */
    load: function(data) {
        this.prepareReader(data);
        this.readEndOfCentral();
        this.readCentralDir();
        this.readLocalFiles();
    }
};
// }}} end of ZipEntries
module.exports = ZipEntries;
...
```

#### <a name="apidoc.element.jszip.zipEntries.prototype.readBlockEndOfCentral"></a>[function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>readBlockEndOfCentral ()](#apidoc.element.jszip.zipEntries.prototype.readBlockEndOfCentral)
- description and source-code
```javascript
readBlockEndOfCentral = function () {
    this.diskNumber = this.reader.readInt(2);
    this.diskWithCentralDirStart = this.reader.readInt(2);
    this.centralDirRecordsOnThisDisk = this.reader.readInt(2);
    this.centralDirRecords = this.reader.readInt(2);
    this.centralDirSize = this.reader.readInt(4);
    this.centralDirOffset = this.reader.readInt(4);

    this.zipCommentLength = this.reader.readInt(2);
    // warning : the encoding depends of the system locale
    // On a linux machine with LANG=en_US.utf8, this field is utf8 encoded.
    // On a windows machine, this field is encoded with the localized windows code page.
    var zipComment = this.reader.readData(this.zipCommentLength);
    var decodeParamType = support.uint8array ? "uint8array" : "array";
    // To get consistent behavior with the generation part, we will assume that
    // this is utf8 encoded unless specified otherwise.
    var decodeContent = utils.transformTo(decodeParamType, zipComment);
    this.zipComment = this.loadOptions.decodeFileName(decodeContent);
}
```
- example usage
```shell
...
        throw new Error("Corrupted zip : can't find end of central directory");
    }

}
this.reader.setIndex(offset);
var endOfCentralDirOffset = offset;
this.checkSignature(sig.CENTRAL_DIRECTORY_END);
this.readBlockEndOfCentral();


/* extract from the zip spec :
    4)  If one of the fields in the end of central directory
        record is too small to hold required data, the field
        should be set to -1 (0xFFFF or 0xFFFFFFFF) and the
        ZIP64 format record should be created.
...
```

#### <a name="apidoc.element.jszip.zipEntries.prototype.readBlockZip64EndOfCentral"></a>[function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>readBlockZip64EndOfCentral ()](#apidoc.element.jszip.zipEntries.prototype.readBlockZip64EndOfCentral)
- description and source-code
```javascript
readBlockZip64EndOfCentral = function () {
    this.zip64EndOfCentralSize = this.reader.readInt(8);
    this.reader.skip(4);
    // this.versionMadeBy = this.reader.readString(2);
    // this.versionNeeded = this.reader.readInt(2);
    this.diskNumber = this.reader.readInt(4);
    this.diskWithCentralDirStart = this.reader.readInt(4);
    this.centralDirRecordsOnThisDisk = this.reader.readInt(8);
    this.centralDirRecords = this.reader.readInt(8);
    this.centralDirSize = this.reader.readInt(8);
    this.centralDirOffset = this.reader.readInt(8);

    this.zip64ExtensibleData = {};
    var extraDataSize = this.zip64EndOfCentralSize - 44,
        index = 0,
        extraFieldId,
        extraFieldLength,
        extraFieldValue;
    while (index < extraDataSize) {
        extraFieldId = this.reader.readInt(2);
        extraFieldLength = this.reader.readInt(4);
        extraFieldValue = this.reader.readData(extraFieldLength);
        this.zip64ExtensibleData[extraFieldId] = {
            id: extraFieldId,
            length: extraFieldLength,
            value: extraFieldValue
        };
    }
}
```
- example usage
```shell
...
        this.relativeOffsetEndOfZip64CentralDir = this.reader.lastIndexOfSignature(sig.ZIP64_CENTRAL_DIRECTORY_END);
        if (this.relativeOffsetEndOfZip64CentralDir < 0) {
            throw new Error("Corrupted zip : can't find the ZIP64 end of central directory");
        }
    }
    this.reader.setIndex(this.relativeOffsetEndOfZip64CentralDir);
    this.checkSignature(sig.ZIP64_CENTRAL_DIRECTORY_END);
    this.readBlockZip64EndOfCentral();
}

var expectedEndOfCentralDirOffset = this.centralDirOffset + this.centralDirSize;
if (this.zip64) {
    expectedEndOfCentralDirOffset += 20; // end of central dir 64 locator
    expectedEndOfCentralDirOffset += 12 /* should not include the leading 12 bytes */ + this.zip64EndOfCentralSize;
}
...
```

#### <a name="apidoc.element.jszip.zipEntries.prototype.readBlockZip64EndOfCentralLocator"></a>[function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>readBlockZip64EndOfCentralLocator ()](#apidoc.element.jszip.zipEntries.prototype.readBlockZip64EndOfCentralLocator)
- description and source-code
```javascript
readBlockZip64EndOfCentralLocator = function () {
    this.diskWithZip64CentralDirStart = this.reader.readInt(4);
    this.relativeOffsetEndOfZip64CentralDir = this.reader.readInt(8);
    this.disksCount = this.reader.readInt(4);
    if (this.disksCount > 1) {
        throw new Error("Multi-volumes zip are not supported");
    }
}
```
- example usage
```shell
...
// should look for a zip64 EOCD locator
offset = this.reader.lastIndexOfSignature(sig.ZIP64_CENTRAL_DIRECTORY_LOCATOR);
if (offset < 0) {
    throw new Error("Corrupted zip : can't find the ZIP64 end of central directory locator");
}
this.reader.setIndex(offset);
this.checkSignature(sig.ZIP64_CENTRAL_DIRECTORY_LOCATOR);
this.readBlockZip64EndOfCentralLocator();

// now the zip64 EOCD record
if (!this.isSignature(this.relativeOffsetEndOfZip64CentralDir, sig.ZIP64_CENTRAL_DIRECTORY_END)) {
    // console.warn("ZIP64 end of central directory not where expected.");
    this.relativeOffsetEndOfZip64CentralDir = this.reader.lastIndexOfSignature(sig.ZIP64_CENTRAL_DIRECTORY_END);
    if (this.relativeOffsetEndOfZip64CentralDir < 0) {
        throw new Error("Corrupted zip : can't find the ZIP64 end of central directory");
...
```

#### <a name="apidoc.element.jszip.zipEntries.prototype.readCentralDir"></a>[function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>readCentralDir ()](#apidoc.element.jszip.zipEntries.prototype.readCentralDir)
- description and source-code
```javascript
readCentralDir = function () {
    var file;

    this.reader.setIndex(this.centralDirOffset);
    while (this.reader.readAndCheckSignature(sig.CENTRAL_FILE_HEADER)) {
        file = new ZipEntry({
            zip64: this.zip64
        }, this.loadOptions);
        file.readCentralPart(this.reader);
        this.files.push(file);
    }

    if (this.centralDirRecords !== this.files.length) {
        if (this.centralDirRecords !== 0 && this.files.length === 0) {
            // We expected some records but couldn't find ANY.
            // This is really suspicious, as if something went wrong.
            throw new Error("Corrupted zip or bug: expected " + this.centralDirRecords + " records in central dir, got " + this.
files.length);
        } else {
            // We found some records but not all.
            // Something is wrong but we got something for the user: no error here.
            // console.warn("expected", this.centralDirRecords, "records in central dir, got", this.files.length);
        }
    }
}
```
- example usage
```shell
...
    /**
     * Read a zip file and create ZipEntries.
     * @param {String|ArrayBuffer|Uint8Array|Buffer} data the binary string representing a zip file.
     */
    load: function(data) {
        this.prepareReader(data);
        this.readEndOfCentral();
        this.readCentralDir();
        this.readLocalFiles();
    }
};
// }}} end of ZipEntries
module.exports = ZipEntries;
...
```

#### <a name="apidoc.element.jszip.zipEntries.prototype.readEndOfCentral"></a>[function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>readEndOfCentral ()](#apidoc.element.jszip.zipEntries.prototype.readEndOfCentral)
- description and source-code
```javascript
readEndOfCentral = function () {
    var offset = this.reader.lastIndexOfSignature(sig.CENTRAL_DIRECTORY_END);
    if (offset < 0) {
        // Check if the content is a truncated zip or complete garbage.
        // A "LOCAL_FILE_HEADER" is not required at the beginning (auto
        // extractible zip for example) but it can give a good hint.
        // If an ajax request was used without responseType, we will also
        // get unreadable data.
        var isGarbage = !this.isSignature(0, sig.LOCAL_FILE_HEADER);

        if (isGarbage) {
            throw new Error("Can't find end of central directory : is this a zip file ? " +
                            "If it is, see http://stuk.github.io/jszip/documentation/howto/read_zip.html");
        } else {
            throw new Error("Corrupted zip : can't find end of central directory");
        }

    }
    this.reader.setIndex(offset);
    var endOfCentralDirOffset = offset;
    this.checkSignature(sig.CENTRAL_DIRECTORY_END);
    this.readBlockEndOfCentral();


<span class="apidocCodeCommentSpan">    /* extract from the zip spec :
        4)  If one of the fields in the end of central directory
            record is too small to hold required data, the field
            should be set to -1 (0xFFFF or 0xFFFFFFFF) and the
            ZIP64 format record should be created.
        5)  The end of central directory record and the
            Zip64 end of central directory locator record must
            reside on the same disk when splitting or spanning
            an archive.
     */
</span>    if (this.diskNumber === utils.MAX_VALUE_16BITS || this.diskWithCentralDirStart === utils.MAX_VALUE_16BITS || this.centralDirRecordsOnThisDisk
 === utils.MAX_VALUE_16BITS || this.centralDirRecords === utils.MAX_VALUE_16BITS || this.centralDirSize === utils.MAX_VALUE_32BITS
 || this.centralDirOffset === utils.MAX_VALUE_32BITS) {
        this.zip64 = true;

        /*
        Warning : the zip64 extension is supported, but ONLY if the 64bits integer read from
        the zip file can fit into a 32bits integer. This cannot be solved : Javascript represents
        all numbers as 64-bit double precision IEEE 754 floating point numbers.
        So, we have 53bits for integers and bitwise operations treat everything as 32bits.
        see https://developer.mozilla.org/en-US/docs/JavaScript/Reference/Operators/Bitwise_Operators
        and http://www.ecma-international.org/publications/files/ECMA-ST/ECMA-262.pdf section 8.5
        */

        // should look for a zip64 EOCD locator
        offset = this.reader.lastIndexOfSignature(sig.ZIP64_CENTRAL_DIRECTORY_LOCATOR);
        if (offset < 0) {
            throw new Error("Corrupted zip : can't find the ZIP64 end of central directory locator");
        }
        this.reader.setIndex(offset);
        this.checkSignature(sig.ZIP64_CENTRAL_DIRECTORY_LOCATOR);
        this.readBlockZip64EndOfCentralLocator();

        // now the zip64 EOCD record
        if (!this.isSignature(this.relativeOffsetEndOfZip64CentralDir, sig.ZIP64_CENTRAL_DIRECTORY_END)) {
            // console.warn("ZIP64 end of central directory not where expected.");
            this.relativeOffsetEndOfZip64CentralDir = this.reader.lastIndexOfSignature(sig.ZIP64_CENTRAL_DIRECTORY_END);
            if (this.relativeOffsetEndOfZip64CentralDir < 0) {
                throw new Error("Corrupted zip : can't find the ZIP64 end of central directory");
            }
        }
        this.reader.setIndex(this.relativeOffsetEndOfZip64CentralDir);
        this.checkSignature(sig.ZIP64_CENTRAL_DIRECTORY_END);
        this.readBlockZip64EndOfCentral();
    }

    var expectedEndOfCentralDirOffset = this.centralDirOffset + this.centralDirSize;
    if (this.zip64) {
        expectedEndOfCentralDirOffset += 20; // end of central dir 64 locator
        expectedEndOfCentralDirOffset += 12 /* should not include the leading 12 bytes */ + this.zip64EndOfCentralSize;
    }

    var extraBytes = endOfCentralDirOffset - expectedEndOfCentralDirOffset;

    if (extraBytes > 0) {
        // console.warn(extraBytes, "extra bytes at beginning or within zipfile"); ...
```
- example usage
```shell
...
    },
    /**
     * Read a zip file and create ZipEntries.
     * @param {String|ArrayBuffer|Uint8Array|Buffer} data the binary string representing a zip file.
     */
    load: function(data) {
        this.prepareReader(data);
        this.readEndOfCentral();
        this.readCentralDir();
        this.readLocalFiles();
    }
};
// }}} end of ZipEntries
module.exports = ZipEntries;
...
```

#### <a name="apidoc.element.jszip.zipEntries.prototype.readLocalFiles"></a>[function <span class="apidocSignatureSpan">jszip.zipEntries.prototype.</span>readLocalFiles ()](#apidoc.element.jszip.zipEntries.prototype.readLocalFiles)
- description and source-code
```javascript
readLocalFiles = function () {
    var i, file;
    for (i = 0; i < this.files.length; i++) {
        file = this.files[i];
        this.reader.setIndex(file.localHeaderOffset);
        this.checkSignature(sig.LOCAL_FILE_HEADER);
        file.readLocalPart(this.reader);
        file.handleUTF8();
        file.processAttributes();
    }
}
```
- example usage
```shell
...
     * Read a zip file and create ZipEntries.
     * @param {String|ArrayBuffer|Uint8Array|Buffer} data the binary string representing a zip file.
     */
    load: function(data) {
        this.prepareReader(data);
        this.readEndOfCentral();
        this.readCentralDir();
        this.readLocalFiles();
    }
};
// }}} end of ZipEntries
module.exports = ZipEntries;
...
```



# <a name="apidoc.module.jszip.zipEntry"></a>[module jszip.zipEntry](#apidoc.module.jszip.zipEntry)

#### <a name="apidoc.element.jszip.zipEntry.zipEntry"></a>[function <span class="apidocSignatureSpan">jszip.</span>zipEntry (options, loadOptions)](#apidoc.element.jszip.zipEntry.zipEntry)
- description and source-code
```javascript
function ZipEntry(options, loadOptions) {
    this.options = options;
    this.loadOptions = loadOptions;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jszip.zipEntry.prototype"></a>[module jszip.zipEntry.prototype](#apidoc.module.jszip.zipEntry.prototype)

#### <a name="apidoc.element.jszip.zipEntry.prototype.findExtraFieldUnicodeComment"></a>[function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>findExtraFieldUnicodeComment ()](#apidoc.element.jszip.zipEntry.prototype.findExtraFieldUnicodeComment)
- description and source-code
```javascript
findExtraFieldUnicodeComment = function () {
    var ucommentField = this.extraFields[0x6375];
    if (ucommentField) {
        var extraReader = readerFor(ucommentField.value);

        // wrong version
        if (extraReader.readInt(1) !== 1) {
            return null;
        }

        // the crc of the comment changed, this field is out of date.
        if (crc32fn(this.fileComment) !== extraReader.readInt(4)) {
            return null;
        }

        return utf8.utf8decode(extraReader.readData(ucommentField.length - 5));
    }
    return null;
}
```
- example usage
```shell
...
    this.fileNameStr = upath;
} else {
    // ASCII text or unsupported code page
    var fileNameByteArray =  utils.transformTo(decodeParamType, this.fileName);
    this.fileNameStr = this.loadOptions.decodeFileName(fileNameByteArray);
}

var ucomment = this.findExtraFieldUnicodeComment();
if (ucomment !== null) {
    this.fileCommentStr = ucomment;
} else {
    // ASCII text or unsupported code page
    var commentByteArray =  utils.transformTo(decodeParamType, this.fileComment);
    this.fileCommentStr = this.loadOptions.decodeFileName(commentByteArray);
}
...
```

#### <a name="apidoc.element.jszip.zipEntry.prototype.findExtraFieldUnicodePath"></a>[function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>findExtraFieldUnicodePath ()](#apidoc.element.jszip.zipEntry.prototype.findExtraFieldUnicodePath)
- description and source-code
```javascript
findExtraFieldUnicodePath = function () {
    var upathField = this.extraFields[0x7075];
    if (upathField) {
        var extraReader = readerFor(upathField.value);

        // wrong version
        if (extraReader.readInt(1) !== 1) {
            return null;
        }

        // the crc of the filename changed, this field is out of date.
        if (crc32fn(this.fileName) !== extraReader.readInt(4)) {
            return null;
        }

        return utf8.utf8decode(extraReader.readData(upathField.length - 5));
    }
    return null;
}
```
- example usage
```shell
...
 */
handleUTF8: function() {
    var decodeParamType = support.uint8array ? "uint8array" : "array";
    if (this.useUTF8()) {
        this.fileNameStr = utf8.utf8decode(this.fileName);
        this.fileCommentStr = utf8.utf8decode(this.fileComment);
    } else {
        var upath = this.findExtraFieldUnicodePath();
        if (upath !== null) {
            this.fileNameStr = upath;
        } else {
            // ASCII text or unsupported code page
            var fileNameByteArray =  utils.transformTo(decodeParamType, this.fileName);
            this.fileNameStr = this.loadOptions.decodeFileName(fileNameByteArray);
        }
...
```

#### <a name="apidoc.element.jszip.zipEntry.prototype.handleUTF8"></a>[function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>handleUTF8 ()](#apidoc.element.jszip.zipEntry.prototype.handleUTF8)
- description and source-code
```javascript
handleUTF8 = function () {
    var decodeParamType = support.uint8array ? "uint8array" : "array";
    if (this.useUTF8()) {
        this.fileNameStr = utf8.utf8decode(this.fileName);
        this.fileCommentStr = utf8.utf8decode(this.fileComment);
    } else {
        var upath = this.findExtraFieldUnicodePath();
        if (upath !== null) {
            this.fileNameStr = upath;
        } else {
            // ASCII text or unsupported code page
            var fileNameByteArray =  utils.transformTo(decodeParamType, this.fileName);
            this.fileNameStr = this.loadOptions.decodeFileName(fileNameByteArray);
        }

        var ucomment = this.findExtraFieldUnicodeComment();
        if (ucomment !== null) {
            this.fileCommentStr = ucomment;
        } else {
            // ASCII text or unsupported code page
            var commentByteArray =  utils.transformTo(decodeParamType, this.fileComment);
            this.fileCommentStr = this.loadOptions.decodeFileName(commentByteArray);
        }
    }
}
```
- example usage
```shell
...
readLocalFiles: function() {
    var i, file;
    for (i = 0; i < this.files.length; i++) {
        file = this.files[i];
        this.reader.setIndex(file.localHeaderOffset);
        this.checkSignature(sig.LOCAL_FILE_HEADER);
        file.readLocalPart(this.reader);
        file.handleUTF8();
        file.processAttributes();
    }
},
/**
 * Read the central directory.
 */
readCentralDir: function() {
...
```

#### <a name="apidoc.element.jszip.zipEntry.prototype.isEncrypted"></a>[function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>isEncrypted ()](#apidoc.element.jszip.zipEntry.prototype.isEncrypted)
- description and source-code
```javascript
isEncrypted = function () {
    // bit 1 is set
    return (this.bitFlag & 0x0001) === 0x0001;
}
```
- example usage
```shell
...
this.extraFieldsLength = reader.readInt(2);
this.fileCommentLength = reader.readInt(2);
this.diskNumberStart = reader.readInt(2);
this.internalFileAttributes = reader.readInt(2);
this.externalFileAttributes = reader.readInt(4);
this.localHeaderOffset = reader.readInt(4);

if (this.isEncrypted()) {
    throw new Error("Encrypted zip are not supported");
}

// will be read in the local part, see the comments there
reader.skip(fileNameLength);
this.readExtraFields(reader);
this.parseZIP64ExtraField(reader);
...
```

#### <a name="apidoc.element.jszip.zipEntry.prototype.parseZIP64ExtraField"></a>[function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>parseZIP64ExtraField (reader)](#apidoc.element.jszip.zipEntry.prototype.parseZIP64ExtraField)
- description and source-code
```javascript
parseZIP64ExtraField = function (reader) {

    if (!this.extraFields[0x0001]) {
        return;
    }

    // should be something, preparing the extra reader
    var extraReader = readerFor(this.extraFields[0x0001].value);

    // I really hope that these 64bits integer can fit in 32 bits integer, because js
    // won't let us have more.
    if (this.uncompressedSize === utils.MAX_VALUE_32BITS) {
        this.uncompressedSize = extraReader.readInt(8);
    }
    if (this.compressedSize === utils.MAX_VALUE_32BITS) {
        this.compressedSize = extraReader.readInt(8);
    }
    if (this.localHeaderOffset === utils.MAX_VALUE_32BITS) {
        this.localHeaderOffset = extraReader.readInt(8);
    }
    if (this.diskNumberStart === utils.MAX_VALUE_32BITS) {
        this.diskNumberStart = extraReader.readInt(4);
    }
}
```
- example usage
```shell
...
    if (this.isEncrypted()) {
        throw new Error("Encrypted zip are not supported");
    }

    // will be read in the local part, see the comments there
    reader.skip(fileNameLength);
    this.readExtraFields(reader);
    this.parseZIP64ExtraField(reader);
    this.fileComment = reader.readData(this.fileCommentLength);
},

/**
 * Parse the external file attributes and get the unix/dos permissions.
 */
processAttributes: function () {
...
```

#### <a name="apidoc.element.jszip.zipEntry.prototype.processAttributes"></a>[function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>processAttributes ()](#apidoc.element.jszip.zipEntry.prototype.processAttributes)
- description and source-code
```javascript
processAttributes = function () {
    this.unixPermissions = null;
    this.dosPermissions = null;
    var madeBy = this.versionMadeBy >> 8;

    // Check if we have the DOS directory flag set.
    // We look for it in the DOS and UNIX permissions
    // but some unknown platform could set it as a compatibility flag.
    this.dir = this.externalFileAttributes & 0x0010 ? true : false;

    if(madeBy === MADE_BY_DOS) {
        // first 6 bits (0 to 5)
        this.dosPermissions = this.externalFileAttributes & 0x3F;
    }

    if(madeBy === MADE_BY_UNIX) {
        this.unixPermissions = (this.externalFileAttributes >> 16) & 0xFFFF;
        // the octal permissions are in (this.unixPermissions & 0x01FF).toString(8);
    }

    // fail safe : if the name ends with a / it probably means a folder
    if (!this.dir && this.fileNameStr.slice(-1) === '/') {
        this.dir = true;
    }
}
```
- example usage
```shell
...
    var i, file;
    for (i = 0; i < this.files.length; i++) {
        file = this.files[i];
        this.reader.setIndex(file.localHeaderOffset);
        this.checkSignature(sig.LOCAL_FILE_HEADER);
        file.readLocalPart(this.reader);
        file.handleUTF8();
        file.processAttributes();
    }
},
/**
 * Read the central directory.
 */
readCentralDir: function() {
    var file;
...
```

#### <a name="apidoc.element.jszip.zipEntry.prototype.readCentralPart"></a>[function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>readCentralPart (reader)](#apidoc.element.jszip.zipEntry.prototype.readCentralPart)
- description and source-code
```javascript
readCentralPart = function (reader) {
    this.versionMadeBy = reader.readInt(2);
    reader.skip(2);
    // this.versionNeeded = reader.readInt(2);
    this.bitFlag = reader.readInt(2);
    this.compressionMethod = reader.readString(2);
    this.date = reader.readDate();
    this.crc32 = reader.readInt(4);
    this.compressedSize = reader.readInt(4);
    this.uncompressedSize = reader.readInt(4);
    var fileNameLength = reader.readInt(2);
    this.extraFieldsLength = reader.readInt(2);
    this.fileCommentLength = reader.readInt(2);
    this.diskNumberStart = reader.readInt(2);
    this.internalFileAttributes = reader.readInt(2);
    this.externalFileAttributes = reader.readInt(4);
    this.localHeaderOffset = reader.readInt(4);

    if (this.isEncrypted()) {
        throw new Error("Encrypted zip are not supported");
    }

    // will be read in the local part, see the comments there
    reader.skip(fileNameLength);
    this.readExtraFields(reader);
    this.parseZIP64ExtraField(reader);
    this.fileComment = reader.readData(this.fileCommentLength);
}
```
- example usage
```shell
...
var file;

this.reader.setIndex(this.centralDirOffset);
while (this.reader.readAndCheckSignature(sig.CENTRAL_FILE_HEADER)) {
    file = new ZipEntry({
        zip64: this.zip64
    }, this.loadOptions);
    file.readCentralPart(this.reader);
    this.files.push(file);
}

if (this.centralDirRecords !== this.files.length) {
    if (this.centralDirRecords !== 0 && this.files.length === 0) {
        // We expected some records but couldn't find ANY.
        // This is really suspicious, as if something went wrong.
...
```

#### <a name="apidoc.element.jszip.zipEntry.prototype.readExtraFields"></a>[function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>readExtraFields (reader)](#apidoc.element.jszip.zipEntry.prototype.readExtraFields)
- description and source-code
```javascript
readExtraFields = function (reader) {
    var end = reader.index + this.extraFieldsLength,
        extraFieldId,
        extraFieldLength,
        extraFieldValue;

    if (!this.extraFields) {
        this.extraFields = {};
    }

    while (reader.index < end) {
        extraFieldId = reader.readInt(2);
        extraFieldLength = reader.readInt(2);
        extraFieldValue = reader.readData(extraFieldLength);

        this.extraFields[extraFieldId] = {
            id: extraFieldId,
            length: extraFieldLength,
            value: extraFieldValue
        };
    }
}
```
- example usage
```shell
...

    if (this.isEncrypted()) {
        throw new Error("Encrypted zip are not supported");
    }

    // will be read in the local part, see the comments there
    reader.skip(fileNameLength);
    this.readExtraFields(reader);
    this.parseZIP64ExtraField(reader);
    this.fileComment = reader.readData(this.fileCommentLength);
},

/**
 * Parse the external file attributes and get the unix/dos permissions.
 */
...
```

#### <a name="apidoc.element.jszip.zipEntry.prototype.readLocalPart"></a>[function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>readLocalPart (reader)](#apidoc.element.jszip.zipEntry.prototype.readLocalPart)
- description and source-code
```javascript
readLocalPart = function (reader) {
    var compression, localExtraFieldsLength;

    // we already know everything from the central dir !
    // If the central dir data are false, we are doomed.
    // On the bright side, the local part is scary  : zip64, data descriptors, both, etc.
    // The less data we get here, the more reliable this should be.
    // Let's skip the whole header and dash to the data !
    reader.skip(22);
    // in some zip created on windows, the filename stored in the central dir contains \ instead of /.
    // Strangely, the filename here is OK.
    // I would love to treat these zip files as corrupted (see http://www.info-zip.org/FAQ.html#backslashes
    // or APPNOTE#4.4.17.1, "All slashes MUST be forward slashes '/'") but there are a lot of bad zip generators...
    // Search "unzip mismatching "local" filename continuing with "central" filename version" on
    // the internet.
    //
    // I think I see the logic here : the central directory is used to display
    // content and the local directory is used to extract the files. Mixing / and \
    // may be used to display \ to windows users and use / when extracting the files.
    // Unfortunately, this lead also to some issues : http://seclists.org/fulldisclosure/2009/Sep/394
    this.fileNameLength = reader.readInt(2);
    localExtraFieldsLength = reader.readInt(2); // can't be sure this will be the same as the central dir
    // the fileName is stored as binary data, the handleUTF8 method will take care of the encoding.
    this.fileName = reader.readData(this.fileNameLength);
    reader.skip(localExtraFieldsLength);

    if (this.compressedSize === -1 || this.uncompressedSize === -1) {
        throw new Error("Bug or corrupted zip : didn't get enough informations from the central directory " + "(compressedSize === -
1 || uncompressedSize === -1)");
    }

    compression = findCompression(this.compressionMethod);
    if (compression === null) { // no compression found
        throw new Error("Corrupted zip : compression " + utils.pretty(this.compressionMethod) + " unknown (inner file : " + utils
.transformTo("string", this.fileName) + ")");
    }
    this.decompressed = new CompressedObject(this.compressedSize, this.uncompressedSize, this.crc32, compression, reader.readData
(this.compressedSize));
}
```
- example usage
```shell
...
 */
readLocalFiles: function() {
    var i, file;
    for (i = 0; i < this.files.length; i++) {
        file = this.files[i];
        this.reader.setIndex(file.localHeaderOffset);
        this.checkSignature(sig.LOCAL_FILE_HEADER);
        file.readLocalPart(this.reader);
        file.handleUTF8();
        file.processAttributes();
    }
},
/**
 * Read the central directory.
 */
...
```

#### <a name="apidoc.element.jszip.zipEntry.prototype.useUTF8"></a>[function <span class="apidocSignatureSpan">jszip.zipEntry.prototype.</span>useUTF8 ()](#apidoc.element.jszip.zipEntry.prototype.useUTF8)
- description and source-code
```javascript
useUTF8 = function () {
    // bit 11 is set
    return (this.bitFlag & 0x0800) === 0x0800;
}
```
- example usage
```shell
...
    }
},
/**
 * Apply an UTF8 transformation if needed.
 */
handleUTF8: function() {
    var decodeParamType = support.uint8array ? "uint8array" : "array";
    if (this.useUTF8()) {
        this.fileNameStr = utf8.utf8decode(this.fileName);
        this.fileCommentStr = utf8.utf8decode(this.fileComment);
    } else {
        var upath = this.findExtraFieldUnicodePath();
        if (upath !== null) {
            this.fileNameStr = upath;
        } else {
...
```



# <a name="apidoc.module.jszip.zipObject"></a>[module jszip.zipObject](#apidoc.module.jszip.zipObject)

#### <a name="apidoc.element.jszip.zipObject.zipObject"></a>[function <span class="apidocSignatureSpan">jszip.</span>zipObject (name, data, options)](#apidoc.element.jszip.zipObject.zipObject)
- description and source-code
```javascript
zipObject = function (name, data, options) {
    this.name = name;
    this.dir = options.dir;
    this.date = options.date;
    this.comment = options.comment;
    this.unixPermissions = options.unixPermissions;
    this.dosPermissions = options.dosPermissions;

    this._data = data;
    this._dataBinary = options.binary;
    // keep only the compression
    this.options = {
        compression : options.compression,
        compressionOptions : options.compressionOptions
    };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jszip.zipObject.prototype"></a>[module jszip.zipObject.prototype](#apidoc.module.jszip.zipObject.prototype)

#### <a name="apidoc.element.jszip.zipObject.prototype._compressWorker"></a>[function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>_compressWorker (compression, compressionOptions)](#apidoc.element.jszip.zipObject.prototype._compressWorker)
- description and source-code
```javascript
_compressWorker = function (compression, compressionOptions) {
    if (
        this._data instanceof CompressedObject &&
        this._data.compression.magic === compression.magic
    ) {
        return this._data.getCompressedWorker();
    } else {
        var result = this._decompressWorker();
        if(!this._dataBinary) {
            result = result.pipe(new utf8.Utf8EncodeWorker());
        }
        return CompressedObject.createWorkerFrom(result, compression, compressionOptions);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jszip.zipObject.prototype._decompressWorker"></a>[function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>_decompressWorker ()](#apidoc.element.jszip.zipObject.prototype._decompressWorker)
- description and source-code
```javascript
_decompressWorker = function () {
    if (this._data instanceof CompressedObject) {
        return this._data.getContentWorker();
    } else if (this._data instanceof GenericWorker) {
        return this._data;
    } else {
        return new DataWorker(this._data);
    }
}
```
- example usage
```shell
...
     */
    internalStream: function (type) {
var outputType = type.toLowerCase();
var askUnicodeString = outputType === "string" || outputType === "text";
if (outputType === "binarystring" || outputType === "text") {
    outputType = "string";
}
var result = this._decompressWorker();

var isUnicodeString = !this._dataBinary;

if (isUnicodeString && !askUnicodeString) {
    result = result.pipe(new utf8.Utf8EncodeWorker());
}
if (!isUnicodeString && askUnicodeString) {
...
```

#### <a name="apidoc.element.jszip.zipObject.prototype.asArrayBuffer"></a>[function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>asArrayBuffer ()](#apidoc.element.jszip.zipObject.prototype.asArrayBuffer)
- description and source-code
```javascript
asArrayBuffer = function () {
    throw new Error("This method has been removed in JSZip 3.0, please check the upgrade guide.");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jszip.zipObject.prototype.asBinary"></a>[function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>asBinary ()](#apidoc.element.jszip.zipObject.prototype.asBinary)
- description and source-code
```javascript
asBinary = function () {
    throw new Error("This method has been removed in JSZip 3.0, please check the upgrade guide.");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jszip.zipObject.prototype.asNodeBuffer"></a>[function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>asNodeBuffer ()](#apidoc.element.jszip.zipObject.prototype.asNodeBuffer)
- description and source-code
```javascript
asNodeBuffer = function () {
    throw new Error("This method has been removed in JSZip 3.0, please check the upgrade guide.");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jszip.zipObject.prototype.asText"></a>[function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>asText ()](#apidoc.element.jszip.zipObject.prototype.asText)
- description and source-code
```javascript
asText = function () {
    throw new Error("This method has been removed in JSZip 3.0, please check the upgrade guide.");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jszip.zipObject.prototype.asUint8Array"></a>[function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>asUint8Array ()](#apidoc.element.jszip.zipObject.prototype.asUint8Array)
- description and source-code
```javascript
asUint8Array = function () {
    throw new Error("This method has been removed in JSZip 3.0, please check the upgrade guide.");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jszip.zipObject.prototype.async"></a>[function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>async (type, onUpdate)](#apidoc.element.jszip.zipObject.prototype.async)
- description and source-code
```javascript
async = function (type, onUpdate) {
    return this.internalStream(type).accumulate(onUpdate);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jszip.zipObject.prototype.internalStream"></a>[function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>internalStream (type)](#apidoc.element.jszip.zipObject.prototype.internalStream)
- description and source-code
```javascript
internalStream = function (type) {
    var outputType = type.toLowerCase();
    var askUnicodeString = outputType === "string" || outputType === "text";
    if (outputType === "binarystring" || outputType === "text") {
        outputType = "string";
    }
    var result = this._decompressWorker();

    var isUnicodeString = !this._dataBinary;

    if (isUnicodeString && !askUnicodeString) {
        result = result.pipe(new utf8.Utf8EncodeWorker());
    }
    if (!isUnicodeString && askUnicodeString) {
        result = result.pipe(new utf8.Utf8DecodeWorker());
    }

    return new StreamHelper(result, outputType, "");
}
```
- example usage
```shell
...
/**
 * Prepare the content in the asked type.
 * @param {String} type the type of the result.
 * @param {Function} onUpdate a function to call on each internal update.
 * @return Promise the promise of the result.
 */
async: function (type, onUpdate) {
    return this.internalStream(type).accumulate(onUpdate);
},

/**
 * Prepare the content as a nodejs stream.
 * @param {String} type the type of each chunk.
 * @param {Function} onUpdate a function to call on each internal update.
 * @return Stream the stream.
...
```

#### <a name="apidoc.element.jszip.zipObject.prototype.nodeStream"></a>[function <span class="apidocSignatureSpan">jszip.zipObject.prototype.</span>nodeStream (type, onUpdate)](#apidoc.element.jszip.zipObject.prototype.nodeStream)
- description and source-code
```javascript
nodeStream = function (type, onUpdate) {
    return this.internalStream(type || "nodebuffer").toNodejsStream(onUpdate);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
