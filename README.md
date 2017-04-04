# api documentation for  [tedious (v2.0.0)](https://github.com/tediousjs/tedious)  [![npm package](https://img.shields.io/npm/v/npmdoc-tedious.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-tedious) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-tedious.svg)](https://travis-ci.org/npmdoc/node-npmdoc-tedious)
#### A TDS driver, for connecting to MS SQLServer databases.

[![NPM](https://nodei.co/npm/tedious.png?downloads=true)](https://www.npmjs.com/package/tedious)

[![apidoc](https://npmdoc.github.io/node-npmdoc-tedious/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-tedious_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-tedious/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-tedious/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-tedious/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mike D Pilsbury",
        "email": "mike.pilsbury@gmail.com"
    },
    "babel": {
        "presets": [
            [
                "env",
                {
                    "targets": {
                        "node": 4
                    }
                }
            ]
        ],
        "plugins": [
            "transform-runtime"
        ]
    },
    "bugs": {
        "url": "https://github.com/tediousjs/tedious/issues"
    },
    "contributors": [
        {
            "name": "Alex Robson"
        },
        {
            "name": "Arthur Schreiber"
        },
        {
            "name": "Bret Copeland",
            "email": "bret@atlantisflight.org",
            "url": "https://github.com/bretcope"
        },
        {
            "name": "Bryan Ross",
            "email": "bryan@rossipedia.com",
            "url": "https://github.com/rossipedia"
        },
        {
            "name": "Ciaran Jessup",
            "email": "ciaranj@gmail.com"
        },
        {
            "name": "Cort Fritz",
            "email": "cfritz@caa.com"
        },
        {
            "name": "lastonesky"
        },
        {
            "name": "Patrik Simek",
            "email": "patrik@patriksimek.cz"
        },
        {
            "name": "Phil Dodderidge",
            "email": "pdodde@poyntz.com"
        },
        {
            "name": "Zach Aller"
        }
    ],
    "dependencies": {
        "babel-runtime": "^6.23.0",
        "big-number": "0.3.1",
        "bl": "^1.2.0",
        "iconv-lite": "^0.4.11",
        "readable-stream": "^2.2.6",
        "sprintf": "0.1.5"
    },
    "description": "A TDS driver, for connecting to MS SQLServer databases.",
    "devDependencies": {
        "async": "^1.4.0",
        "babel-cli": "^6.24.0",
        "babel-plugin-transform-runtime": "^6.23.0",
        "babel-preset-env": "^1.2.2",
        "babel-register": "^6.24.0",
        "benchmark": "^2.1.0",
        "coffee-script": "^1.9.3",
        "eslint": "^3.18.0",
        "mitm": "^1.3.2",
        "nodeunit": "^0.11.0",
        "sinon": "^1.17.5"
    },
    "directories": {},
    "dist": {
        "shasum": "2765e9c8684f62631d85e6a88055ebb82dc8f57d",
        "tarball": "https://registry.npmjs.org/tedious/-/tedious-2.0.0.tgz"
    },
    "engines": {
        "node": ">= 4"
    },
    "gitHead": "3609d0bda1971724062a98c9d99353fc66f09da5",
    "homepage": "https://github.com/tediousjs/tedious",
    "keywords": [
        "sql",
        "database",
        "mssql",
        "sqlserver",
        "sql-server",
        "tds",
        "msnodesql",
        "azure"
    ],
    "license": "MIT",
    "main": "./lib/tedious.js",
    "maintainers": [
        {
            "name": "pekim",
            "email": "mike.pilsbury@gmail.com"
        },
        {
            "name": "patriksimek",
            "email": "patrik@patriksimek.cz"
        },
        {
            "name": "bretcope",
            "email": "bret@atlantisflight.org"
        },
        {
            "name": "rossipedia",
            "email": "bryan@rossipedia.com"
        },
        {
            "name": "arthurschreiber",
            "email": "schreiber.arthur@googlemail.com"
        }
    ],
    "name": "tedious",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tediousjs/tedious.git"
    },
    "scripts": {
        "prepublish": "coffee scripts/build.coffee",
        "pretest": "eslint src test",
        "pretest-all": "eslint src test",
        "pretest-integration": "eslint src test",
        "test": "nodeunit --reporter minimal test/setup.js test/unit/ test/unit/token/ test/unit/tracking-buffer",
        "test-all": "nodeunit --reporter minimal test/setup.js test/unit/ test/unit/token/ test/unit/tracking-buffer test/integration/",
        "test-integration": "nodeunit --reporter minimal test/setup.js test/integration/"
    },
    "version": "2.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module tedious](#apidoc.module.tedious)
1.  [function <span class="apidocSignatureSpan">tedious.</span>BulkLoad (table, options1, callback)](#apidoc.element.tedious.BulkLoad)
1.  [function <span class="apidocSignatureSpan">tedious.</span>Connection (config)](#apidoc.element.tedious.Connection)
1.  [function <span class="apidocSignatureSpan">tedious.</span>ConnectionError (message, code)](#apidoc.element.tedious.ConnectionError)
1.  [function <span class="apidocSignatureSpan">tedious.</span>ConnectionError.super_ ()](#apidoc.element.tedious.ConnectionError.super_)
1.  [function <span class="apidocSignatureSpan">tedious.</span>Request (sqlTextOrProcedure, callback)](#apidoc.element.tedious.Request)
1.  [function <span class="apidocSignatureSpan">tedious.</span>RequestError (message, code)](#apidoc.element.tedious.RequestError)
1.  [function <span class="apidocSignatureSpan">tedious.</span>metadata_parser (parser, options, callback)](#apidoc.element.tedious.metadata_parser)
1.  object <span class="apidocSignatureSpan">tedious.</span>ISOLATION_LEVEL
1.  object <span class="apidocSignatureSpan">tedious.</span>TDS_VERSION
1.  object <span class="apidocSignatureSpan">tedious.</span>TYPES
1.  object <span class="apidocSignatureSpan">tedious.</span>all_headers
1.  object <span class="apidocSignatureSpan">tedious.</span>connector
1.  object <span class="apidocSignatureSpan">tedious.</span>errors
1.  object <span class="apidocSignatureSpan">tedious.</span>guid_parser
1.  object <span class="apidocSignatureSpan">tedious.</span>instance_lookup
1.  object <span class="apidocSignatureSpan">tedious.</span>library
1.  object <span class="apidocSignatureSpan">tedious.</span>packet
1.  object <span class="apidocSignatureSpan">tedious.</span>sender
1.  object <span class="apidocSignatureSpan">tedious.</span>transaction

#### [module tedious.ConnectionError](#apidoc.module.tedious.ConnectionError)
1.  [function <span class="apidocSignatureSpan">tedious.</span>ConnectionError (message, code)](#apidoc.element.tedious.ConnectionError.ConnectionError)
1.  [function <span class="apidocSignatureSpan">tedious.ConnectionError.</span>super_ ()](#apidoc.element.tedious.ConnectionError.super_)

#### [module tedious.ConnectionError.super_](#apidoc.module.tedious.ConnectionError.super_)
1.  [function <span class="apidocSignatureSpan">tedious.ConnectionError.</span>super_ ()](#apidoc.element.tedious.ConnectionError.super_.super_)
1.  [function <span class="apidocSignatureSpan">tedious.ConnectionError.super_.</span>captureStackTrace ()](#apidoc.element.tedious.ConnectionError.super_.captureStackTrace)
1.  number <span class="apidocSignatureSpan">tedious.ConnectionError.super_.</span>stackTraceLimit

#### [module tedious.RequestError](#apidoc.module.tedious.RequestError)
1.  [function <span class="apidocSignatureSpan">tedious.</span>RequestError (message, code)](#apidoc.element.tedious.RequestError.RequestError)
1.  [function <span class="apidocSignatureSpan">tedious.RequestError.</span>super_ ()](#apidoc.element.tedious.RequestError.super_)

#### [module tedious.all_headers](#apidoc.module.tedious.all_headers)
1.  [function <span class="apidocSignatureSpan">tedious.all_headers.</span>writeToTrackingBuffer (buffer, txnDescriptor, outstandingRequestCount)](#apidoc.element.tedious.all_headers.writeToTrackingBuffer)

#### [module tedious.connector](#apidoc.module.tedious.connector)
1.  [function <span class="apidocSignatureSpan">tedious.connector.</span>Connector (options, multiSubnetFailover)](#apidoc.element.tedious.connector.Connector)
1.  [function <span class="apidocSignatureSpan">tedious.connector.</span>ParallelConnectionStrategy (addresses, options)](#apidoc.element.tedious.connector.ParallelConnectionStrategy)
1.  [function <span class="apidocSignatureSpan">tedious.connector.</span>SequentialConnectionStrategy (addresses, options)](#apidoc.element.tedious.connector.SequentialConnectionStrategy)

#### [module tedious.errors](#apidoc.module.tedious.errors)
1.  [function <span class="apidocSignatureSpan">tedious.errors.</span>ConnectionError (message, code)](#apidoc.element.tedious.errors.ConnectionError)
1.  [function <span class="apidocSignatureSpan">tedious.errors.</span>RequestError (message, code)](#apidoc.element.tedious.errors.RequestError)

#### [module tedious.guid_parser](#apidoc.module.tedious.guid_parser)
1.  [function <span class="apidocSignatureSpan">tedious.guid_parser.</span>arrayToGuid (array)](#apidoc.element.tedious.guid_parser.arrayToGuid)
1.  [function <span class="apidocSignatureSpan">tedious.guid_parser.</span>guidToArray (guid)](#apidoc.element.tedious.guid_parser.guidToArray)

#### [module tedious.instance_lookup](#apidoc.module.tedious.instance_lookup)
1.  [function <span class="apidocSignatureSpan">tedious.instance_lookup.</span>InstanceLookup ()](#apidoc.element.tedious.instance_lookup.InstanceLookup)

#### [module tedious.metadata_parser](#apidoc.module.tedious.metadata_parser)
1.  [function <span class="apidocSignatureSpan">tedious.</span>metadata_parser (parser, options, callback)](#apidoc.element.tedious.metadata_parser.metadata_parser)
1.  [function <span class="apidocSignatureSpan">tedious.metadata_parser.</span>readCollation (parser, type, callback)](#apidoc.element.tedious.metadata_parser.readCollation)
1.  [function <span class="apidocSignatureSpan">tedious.metadata_parser.</span>readPrecision (parser, type, callback)](#apidoc.element.tedious.metadata_parser.readPrecision)
1.  [function <span class="apidocSignatureSpan">tedious.metadata_parser.</span>readScale (parser, type, callback)](#apidoc.element.tedious.metadata_parser.readScale)

#### [module tedious.packet](#apidoc.module.tedious.packet)
1.  [function <span class="apidocSignatureSpan">tedious.packet.</span>Packet (typeOrBuffer)](#apidoc.element.tedious.packet.Packet)
1.  [function <span class="apidocSignatureSpan">tedious.packet.</span>isPacketComplete (potentialPacketBuffer)](#apidoc.element.tedious.packet.isPacketComplete)
1.  [function <span class="apidocSignatureSpan">tedious.packet.</span>packetLength (potentialPacketBuffer)](#apidoc.element.tedious.packet.packetLength)
1.  number <span class="apidocSignatureSpan">tedious.packet.</span>HEADER_LENGTH
1.  object <span class="apidocSignatureSpan">tedious.packet.</span>OFFSET
1.  object <span class="apidocSignatureSpan">tedious.packet.</span>TYPE

#### [module tedious.sender](#apidoc.module.tedious.sender)
1.  [function <span class="apidocSignatureSpan">tedious.sender.</span>ParallelSendStrategy (addresses, port, request)](#apidoc.element.tedious.sender.ParallelSendStrategy)
1.  [function <span class="apidocSignatureSpan">tedious.sender.</span>Sender (host, port, request)](#apidoc.element.tedious.sender.Sender)

#### [module tedious.transaction](#apidoc.module.tedious.transaction)
1.  [function <span class="apidocSignatureSpan">tedious.transaction.</span>Transaction (name, isolationLevel)](#apidoc.element.tedious.transaction.Transaction)
1.  object <span class="apidocSignatureSpan">tedious.transaction.</span>ISOLATION_LEVEL
1.  object <span class="apidocSignatureSpan">tedious.transaction.</span>OPERATION_TYPE



# <a name="apidoc.module.tedious"></a>[module tedious](#apidoc.module.tedious)

#### <a name="apidoc.element.tedious.BulkLoad"></a>[function <span class="apidocSignatureSpan">tedious.</span>BulkLoad (table, options1, callback)](#apidoc.element.tedious.BulkLoad)
- description and source-code
```javascript
function BulkLoad(table, options1, callback) {
  (0, _classCallCheck3.default)(this, BulkLoad);

  var _this = (0, _possibleConstructorReturn3.default)(this, (BulkLoad.__proto__ || (0, _getPrototypeOf2.default)(BulkLoad)).call
(this));

  _this.error = undefined;
  _this.canceled = false;

  _this.table = table;
  _this.options = options1;
  _this.callback = callback;
  _this.columns = [];
  _this.columnsByName = {};
  _this.rowsData = new WritableTrackingBuffer(1024, 'ucs2', true);
  _this.firstRowWritten = false;
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.Connection"></a>[function <span class="apidocSignatureSpan">tedious.</span>Connection (config)](#apidoc.element.tedious.Connection)
- description and source-code
```javascript
function Connection(config) {
  (0, _classCallCheck3.default)(this, Connection);

  var _this = (0, _possibleConstructorReturn3.default)(this, (Connection.__proto__ || (0, _getPrototypeOf2.default)(Connection)).
call(this));

  if (!config) {
    throw new TypeError('No connection configuration given');
  }

  if (typeof config.server !== 'string') {
    throw new TypeError('Invalid server: ' + config.server);
  }

  _this.config = {
    server: config.server,
    userName: config.userName,
    password: config.password,
    domain: config.domain && config.domain.toUpperCase(),
    options: {
      abortTransactionOnError: false,
      appName: undefined,
      camelCaseColumns: false,
      cancelTimeout: DEFAULT_CANCEL_TIMEOUT,
      columnNameReplacer: undefined,
      connectTimeout: DEFAULT_CONNECT_TIMEOUT,
      connectionIsolationLevel: ISOLATION_LEVEL.READ_COMMITTED,
      cryptoCredentialsDetails: {},
      database: undefined,
      datefirst: DEFAULT_DATEFIRST,
      debug: {
        data: false,
        packet: false,
        payload: false,
        token: false
      },
      enableArithAbort: false,
      enableAnsiNullDefault: true,
      encrypt: false,
      fallbackToDefaultDb: false,
      instanceName: undefined,
      isolationLevel: ISOLATION_LEVEL.READ_COMMITTED,
      localAddress: undefined,
      multiSubnetFailover: false,
      packetSize: DEFAULT_PACKET_SIZE,
      port: DEFAULT_PORT,
      readOnlyIntent: false,
      requestTimeout: DEFAULT_CLIENT_REQUEST_TIMEOUT,
      rowCollectionOnDone: false,
      rowCollectionOnRequestCompletion: false,
      tdsVersion: DEFAULT_TDS_VERSION,
      textsize: DEFAULT_TEXTSIZE,
      trustServerCertificate: true,
      useColumnNames: false,
      useUTC: true
    }
  };

  if (config.options) {
    if (config.options.port && config.options.instanceName) {
      throw new Error('Port and instanceName are mutually exclusive, but ' + config.options.port + ' and ' + config.options.instanceName
 + ' provided');
    }

    if (config.options.abortTransactionOnError != undefined) {
      _this.config.options.abortTransactionOnError = config.options.abortTransactionOnError;
    }

    if (config.options.appName != undefined) {
      _this.config.options.appName = config.options.appName;
    }

    if (config.options.camelCaseColumns != undefined) {
      _this.config.options.camelCaseColumns = config.options.camelCaseColumns;
    }

    if (config.options.cancelTimeout != undefined) {
      _this.config.options.cancelTimeout = config.options.cancelTimeout;
    }

    if (config.options.columnNameReplacer) {
      if (typeof config.options.columnNameReplacer !== 'function') {
        throw new TypeError('options.columnNameReplacer must be a function or null.');
      }

      _this.config.options.columnNameReplacer = config.options.columnNameReplacer;
    }

    if (config.options.connectTimeout) {
      _this.config.options.connectTimeout = config.options.connectTimeout;
    }

    if (config.options.connectionIsolationLevel) {
      _this.config.options.connectionIsolationLevel = config.options.connectionIsolationLevel;
    }

    if (config.options.cryptoCredentialsDetails) {
      _this.config.options.cryptoCredentialsDetails = config.options.cryptoCredentialsDetails;
    }

    if (config.options.database != undefined) {
      _this.config.options.database = config.options.database;
    }

    if (config.options.datefirst) {
      if (config.options.datefirst < 1 || config.options.datefirst > 7) {
        throw new RangeError('DateFirst should be >= 1 and <= 7');
      }

      _this.config.options.datefirst = config.options.datefirst;
    }

    if (config.options.debug) {
      if (config.options.debug.data != undefined) {
        _this.config.options.debug.data = config.options.debug.data;
      }
      if (config.options.debug.packet != undefined) {
        _this.config.options.debug.packet = config.options.debug.packet;
      }
      if (config.options.debug.payload != undefined) {
        _this.config.options.debug.payload = config.options.debug.payl ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.ConnectionError"></a>[function <span class="apidocSignatureSpan">tedious.</span>ConnectionError (message, code)](#apidoc.element.tedious.ConnectionError)
- description and source-code
```javascript
function ConnectionError(message, code) {
  if (!(this instanceof ConnectionError)) {
    if (message instanceof ConnectionError) {
      return message;
    }

    return new ConnectionError(message, code);
  }

  Error.call(this);

  this.message = message;
  this.code = code;

  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.ConnectionError.super_"></a>[function <span class="apidocSignatureSpan">tedious.</span>ConnectionError.super_ ()](#apidoc.element.tedious.ConnectionError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.Request"></a>[function <span class="apidocSignatureSpan">tedious.</span>Request (sqlTextOrProcedure, callback)](#apidoc.element.tedious.Request)
- description and source-code
```javascript
function Request(sqlTextOrProcedure, callback) {
  (0, _classCallCheck3.default)(this, Request);

  var _this = (0, _possibleConstructorReturn3.default)(this, (Request.__proto__ || (0, _getPrototypeOf2.default)(Request)).call(
this));

  _this.sqlTextOrProcedure = sqlTextOrProcedure;
  _this.callback = callback;
  _this.parameters = [];
  _this.parametersByName = {};
  _this.userCallback = _this.callback;
  _this.callback = function () {
    if (this.preparing) {
      this.emit('prepared');
      return this.preparing = false;
    } else {
      this.userCallback.apply(this, arguments);
      return this.emit('requestCompleted');
    }
  };
  return _this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.RequestError"></a>[function <span class="apidocSignatureSpan">tedious.</span>RequestError (message, code)](#apidoc.element.tedious.RequestError)
- description and source-code
```javascript
function RequestError(message, code) {
  if (!(this instanceof RequestError)) {
    if (message instanceof RequestError) {
      return message;
    }

    return new RequestError(message, code);
  }

  Error.call(this);

  this.message = message;
  this.code = code;

  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.metadata_parser"></a>[function <span class="apidocSignatureSpan">tedious.</span>metadata_parser (parser, options, callback)](#apidoc.element.tedious.metadata_parser)
- description and source-code
```javascript
function metadataParse(parser, options, callback) {
  (options.tdsVersion < '7_2' ? parser.readUInt16LE : parser.readUInt32LE).call(parser, function (userType) {
    parser.readUInt16LE(function (flags) {
      parser.readUInt8(function (typeNumber) {
        var type = TYPE[typeNumber];

        if (!type) {
          return parser.emit(new Error(sprintf('Unrecognised data type 0x%02X', typeNumber)));
        }

        readDataLength(parser, type, function (dataLength) {
          readPrecision(parser, type, function (precision) {
            readScale(parser, type, function (scale) {
              if (scale && type.dataLengthFromScale) {
                dataLength = type.dataLengthFromScale(scale);
              }

              readCollation(parser, type, function (collation) {
                readSchema(parser, type, function (schema) {
                  readUDTInfo(parser, type, function (udtInfo) {
                    callback({
                      userType: userType,
                      flags: flags,
                      type: type,
                      collation: collation,
                      precision: precision,
                      scale: scale,
                      dataLength: dataLength,
                      schema: schema,
                      udtInfo: udtInfo
                    });
                  });
                });
              });
            });
          });
        });
      });
    });
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tedious.ConnectionError"></a>[module tedious.ConnectionError](#apidoc.module.tedious.ConnectionError)

#### <a name="apidoc.element.tedious.ConnectionError.ConnectionError"></a>[function <span class="apidocSignatureSpan">tedious.</span>ConnectionError (message, code)](#apidoc.element.tedious.ConnectionError.ConnectionError)
- description and source-code
```javascript
function ConnectionError(message, code) {
  if (!(this instanceof ConnectionError)) {
    if (message instanceof ConnectionError) {
      return message;
    }

    return new ConnectionError(message, code);
  }

  Error.call(this);

  this.message = message;
  this.code = code;

  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.ConnectionError.super_"></a>[function <span class="apidocSignatureSpan">tedious.ConnectionError.</span>super_ ()](#apidoc.element.tedious.ConnectionError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tedious.ConnectionError.super_"></a>[module tedious.ConnectionError.super_](#apidoc.module.tedious.ConnectionError.super_)

#### <a name="apidoc.element.tedious.ConnectionError.super_.super_"></a>[function <span class="apidocSignatureSpan">tedious.ConnectionError.</span>super_ ()](#apidoc.element.tedious.ConnectionError.super_.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.ConnectionError.super_.captureStackTrace"></a>[function <span class="apidocSignatureSpan">tedious.ConnectionError.super_.</span>captureStackTrace ()](#apidoc.element.tedious.ConnectionError.super_.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
...
  }

  Error.call(this);

  this.message = message;
  this.code = code;

  Error.captureStackTrace(this, this.constructor);
}

util.inherits(ConnectionError, Error);

ConnectionError.prototype.name = 'ConnectionError';

module.exports.RequestError = RequestError;
...
```



# <a name="apidoc.module.tedious.RequestError"></a>[module tedious.RequestError](#apidoc.module.tedious.RequestError)

#### <a name="apidoc.element.tedious.RequestError.RequestError"></a>[function <span class="apidocSignatureSpan">tedious.</span>RequestError (message, code)](#apidoc.element.tedious.RequestError.RequestError)
- description and source-code
```javascript
function RequestError(message, code) {
  if (!(this instanceof RequestError)) {
    if (message instanceof RequestError) {
      return message;
    }

    return new RequestError(message, code);
  }

  Error.call(this);

  this.message = message;
  this.code = code;

  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.RequestError.super_"></a>[function <span class="apidocSignatureSpan">tedious.RequestError.</span>super_ ()](#apidoc.element.tedious.RequestError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tedious.all_headers"></a>[module tedious.all_headers](#apidoc.module.tedious.all_headers)

#### <a name="apidoc.element.tedious.all_headers.writeToTrackingBuffer"></a>[function <span class="apidocSignatureSpan">tedious.all_headers.</span>writeToTrackingBuffer (buffer, txnDescriptor, outstandingRequestCount)](#apidoc.element.tedious.all_headers.writeToTrackingBuffer)
- description and source-code
```javascript
function writeToTrackingBuffer(buffer, txnDescriptor, outstandingRequestCount) {
  buffer.writeUInt32LE(0);
  buffer.writeUInt32LE(TXNDESCRIPTOR_HEADER_LEN);
  buffer.writeUInt16LE(TYPE.TXN_DESCRIPTOR);
  buffer.writeBuffer(txnDescriptor);
  buffer.writeUInt32LE(outstandingRequestCount);

  var data = buffer.data;
  data.writeUInt32LE(data.length, 0);
  return buffer;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tedious.connector"></a>[module tedious.connector](#apidoc.module.tedious.connector)

#### <a name="apidoc.element.tedious.connector.Connector"></a>[function <span class="apidocSignatureSpan">tedious.connector.</span>Connector (options, multiSubnetFailover)](#apidoc.element.tedious.connector.Connector)
- description and source-code
```javascript
function Connector(options, multiSubnetFailover) {
  (0, _classCallCheck3.default)(this, Connector);

  this.options = options;
  this.multiSubnetFailover = multiSubnetFailover;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.connector.ParallelConnectionStrategy"></a>[function <span class="apidocSignatureSpan">tedious.connector.</span>ParallelConnectionStrategy (addresses, options)](#apidoc.element.tedious.connector.ParallelConnectionStrategy)
- description and source-code
```javascript
function ParallelConnectionStrategy(addresses, options) {
  (0, _classCallCheck3.default)(this, ParallelConnectionStrategy);

  this.addresses = addresses;
  this.options = options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.connector.SequentialConnectionStrategy"></a>[function <span class="apidocSignatureSpan">tedious.connector.</span>SequentialConnectionStrategy (addresses, options)](#apidoc.element.tedious.connector.SequentialConnectionStrategy)
- description and source-code
```javascript
function SequentialConnectionStrategy(addresses, options) {
  (0, _classCallCheck3.default)(this, SequentialConnectionStrategy);

  this.addresses = addresses;
  this.options = options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tedious.errors"></a>[module tedious.errors](#apidoc.module.tedious.errors)

#### <a name="apidoc.element.tedious.errors.ConnectionError"></a>[function <span class="apidocSignatureSpan">tedious.errors.</span>ConnectionError (message, code)](#apidoc.element.tedious.errors.ConnectionError)
- description and source-code
```javascript
function ConnectionError(message, code) {
  if (!(this instanceof ConnectionError)) {
    if (message instanceof ConnectionError) {
      return message;
    }

    return new ConnectionError(message, code);
  }

  Error.call(this);

  this.message = message;
  this.code = code;

  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.errors.RequestError"></a>[function <span class="apidocSignatureSpan">tedious.errors.</span>RequestError (message, code)](#apidoc.element.tedious.errors.RequestError)
- description and source-code
```javascript
function RequestError(message, code) {
  if (!(this instanceof RequestError)) {
    if (message instanceof RequestError) {
      return message;
    }

    return new RequestError(message, code);
  }

  Error.call(this);

  this.message = message;
  this.code = code;

  Error.captureStackTrace(this, this.constructor);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tedious.guid_parser"></a>[module tedious.guid_parser](#apidoc.module.tedious.guid_parser)

#### <a name="apidoc.element.tedious.guid_parser.arrayToGuid"></a>[function <span class="apidocSignatureSpan">tedious.guid_parser.</span>arrayToGuid (array)](#apidoc.element.tedious.guid_parser.arrayToGuid)
- description and source-code
```javascript
function arrayToGuid(array) {
  return MAP[array[3]] + MAP[array[2]] + MAP[array[1]] + MAP[array[0]] + '-' + MAP[array[5]] + MAP[array[4]] + '-' + MAP[array[7
]] + MAP[array[6]] + '-' + MAP[array[8]] + MAP[array[9]] + '-' + MAP[array[10]] + MAP[array[11]] + MAP[array[12]] + MAP[array[13
]] + MAP[array[14]] + MAP[array[15]];
}
```
- example usage
```shell
...

case 'UniqueIdentifierN':
  switch (dataLength) {
    case 0:
      return callback(null);
    case 0x10:
      return parser.readBuffer(0x10, function (data) {
        callback(guidParser.arrayToGuid(data));
      });

    default:
      return parser.emit('error', new Error(sprintf('Unsupported guid size %d', dataLength - 1)));
  }

case 'UDT':
...
```

#### <a name="apidoc.element.tedious.guid_parser.guidToArray"></a>[function <span class="apidocSignatureSpan">tedious.guid_parser.</span>guidToArray (guid)](#apidoc.element.tedious.guid_parser.guidToArray)
- description and source-code
```javascript
function guidToArray(guid) {
  return [CHARCODEMAP[guid.charCodeAt(6)][guid.charCodeAt(7)], CHARCODEMAP[guid.charCodeAt(4)][guid.charCodeAt(5)], CHARCODEMAP[
guid.charCodeAt(2)][guid.charCodeAt(3)], CHARCODEMAP[guid.charCodeAt(0)][guid.charCodeAt(1)], CHARCODEMAP[guid.charCodeAt(11)][guid
.charCodeAt(12)], CHARCODEMAP[guid.charCodeAt(9)][guid.charCodeAt(10)], CHARCODEMAP[guid.charCodeAt(16)][guid.charCodeAt(17)], CHARCODEMAP
[guid.charCodeAt(14)][guid.charCodeAt(15)], CHARCODEMAP[guid.charCodeAt(19)][guid.charCodeAt(20)], CHARCODEMAP[guid.charCodeAt(21
)][guid.charCodeAt(22)], CHARCODEMAP[guid.charCodeAt(24)][guid.charCodeAt(25)], CHARCODEMAP[guid.charCodeAt(26)][guid.charCodeAt
(27)], CHARCODEMAP[guid.charCodeAt(28)][guid.charCodeAt(29)], CHARCODEMAP[guid.charCodeAt(30)][guid.charCodeAt(31)], CHARCODEMAP
[guid.charCodeAt(32)][guid.charCodeAt(33)], CHARCODEMAP[guid.charCodeAt(34)][guid.charCodeAt(35)]];
}
```
- example usage
```shell
...
  buffer.writeUInt8(typeByName.UniqueIdentifierN.id);
  return buffer.writeUInt8(0x10);
},

writeParameterData: function writeParameterData(buffer, parameter) {
  if (parameter.value != null) {
    buffer.writeUInt8(0x10);
    return buffer.writeBuffer(new Buffer(guidParser.guidToArray(parameter.value)));
  } else {
    return buffer.writeUInt8(0);
  }
},

validate: function validate(value) {
  if (value == null) {
...
```



# <a name="apidoc.module.tedious.instance_lookup"></a>[module tedious.instance_lookup](#apidoc.module.tedious.instance_lookup)

#### <a name="apidoc.element.tedious.instance_lookup.InstanceLookup"></a>[function <span class="apidocSignatureSpan">tedious.instance_lookup.</span>InstanceLookup ()](#apidoc.element.tedious.instance_lookup.InstanceLookup)
- description and source-code
```javascript
function InstanceLookup() {
  (0, _classCallCheck3.default)(this, InstanceLookup);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tedious.metadata_parser"></a>[module tedious.metadata_parser](#apidoc.module.tedious.metadata_parser)

#### <a name="apidoc.element.tedious.metadata_parser.metadata_parser"></a>[function <span class="apidocSignatureSpan">tedious.</span>metadata_parser (parser, options, callback)](#apidoc.element.tedious.metadata_parser.metadata_parser)
- description and source-code
```javascript
function metadataParse(parser, options, callback) {
  (options.tdsVersion < '7_2' ? parser.readUInt16LE : parser.readUInt32LE).call(parser, function (userType) {
    parser.readUInt16LE(function (flags) {
      parser.readUInt8(function (typeNumber) {
        var type = TYPE[typeNumber];

        if (!type) {
          return parser.emit(new Error(sprintf('Unrecognised data type 0x%02X', typeNumber)));
        }

        readDataLength(parser, type, function (dataLength) {
          readPrecision(parser, type, function (precision) {
            readScale(parser, type, function (scale) {
              if (scale && type.dataLengthFromScale) {
                dataLength = type.dataLengthFromScale(scale);
              }

              readCollation(parser, type, function (collation) {
                readSchema(parser, type, function (schema) {
                  readUDTInfo(parser, type, function (udtInfo) {
                    callback({
                      userType: userType,
                      flags: flags,
                      type: type,
                      collation: collation,
                      precision: precision,
                      scale: scale,
                      dataLength: dataLength,
                      schema: schema,
                      udtInfo: udtInfo
                    });
                  });
                });
              });
            });
          });
        });
      });
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.metadata_parser.readCollation"></a>[function <span class="apidocSignatureSpan">tedious.metadata_parser.</span>readCollation (parser, type, callback)](#apidoc.element.tedious.metadata_parser.readCollation)
- description and source-code
```javascript
function readCollation(parser, type, callback) {
  if (type.hasCollation) {
    // s2.2.5.1.2
    parser.readBuffer(5, function (collationData) {
      var collation = {};

      collation.lcid = (collationData[2] & 0x0F) << 16;
      collation.lcid |= collationData[1] << 8;
      collation.lcid |= collationData[0];

      // This may not be extracting the correct nibbles in the correct order.
      collation.flags = collationData[3] >> 4;
      collation.flags |= collationData[2] & 0xF0;

      // This may not be extracting the correct nibble.
      collation.version = collationData[3] & 0x0F;

      collation.sortId = collationData[4];

      collation.codepage = codepageBySortId[collation.sortId] || codepageByLcid[collation.lcid] || 'CP1252';

      callback(collation);
    });
  } else {
    callback(undefined);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.metadata_parser.readPrecision"></a>[function <span class="apidocSignatureSpan">tedious.metadata_parser.</span>readPrecision (parser, type, callback)](#apidoc.element.tedious.metadata_parser.readPrecision)
- description and source-code
```javascript
function readPrecision(parser, type, callback) {
  if (type.hasPrecision) {
    parser.readUInt8(callback);
  } else {
    callback(undefined);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.metadata_parser.readScale"></a>[function <span class="apidocSignatureSpan">tedious.metadata_parser.</span>readScale (parser, type, callback)](#apidoc.element.tedious.metadata_parser.readScale)
- description and source-code
```javascript
function readScale(parser, type, callback) {
  if (type.hasScale) {
    parser.readUInt8(callback);
  } else {
    callback(undefined);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tedious.packet"></a>[module tedious.packet](#apidoc.module.tedious.packet)

#### <a name="apidoc.element.tedious.packet.Packet"></a>[function <span class="apidocSignatureSpan">tedious.packet.</span>Packet (typeOrBuffer)](#apidoc.element.tedious.packet.Packet)
- description and source-code
```javascript
function Packet(typeOrBuffer) {
  (0, _classCallCheck3.default)(this, Packet);

  if (typeOrBuffer instanceof Buffer) {
    this.buffer = typeOrBuffer;
  } else {
    var type = typeOrBuffer;
    this.buffer = new Buffer(HEADER_LENGTH);
    this.buffer.writeUInt8(type, OFFSET.Type);
    this.buffer.writeUInt8(STATUS.NORMAL, OFFSET.Status);
    this.buffer.writeUInt16BE(DEFAULT_SPID, OFFSET.SPID);
    this.buffer.writeUInt8(DEFAULT_PACKETID, OFFSET.PacketID);
    this.buffer.writeUInt8(DEFAULT_WINDOW, OFFSET.Window);
    this.setLength();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.packet.isPacketComplete"></a>[function <span class="apidocSignatureSpan">tedious.packet.</span>isPacketComplete (potentialPacketBuffer)](#apidoc.element.tedious.packet.isPacketComplete)
- description and source-code
```javascript
function isPacketComplete(potentialPacketBuffer) {
  if (potentialPacketBuffer.length < HEADER_LENGTH) {
    return false;
  } else {
    return potentialPacketBuffer.length >= potentialPacketBuffer.readUInt16BE(OFFSET.Length);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.packet.packetLength"></a>[function <span class="apidocSignatureSpan">tedious.packet.</span>packetLength (potentialPacketBuffer)](#apidoc.element.tedious.packet.packetLength)
- description and source-code
```javascript
function packetLength(potentialPacketBuffer) {
  return potentialPacketBuffer.readUInt16BE(OFFSET.Length);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tedious.sender"></a>[module tedious.sender](#apidoc.module.tedious.sender)

#### <a name="apidoc.element.tedious.sender.ParallelSendStrategy"></a>[function <span class="apidocSignatureSpan">tedious.sender.</span>ParallelSendStrategy (addresses, port, request)](#apidoc.element.tedious.sender.ParallelSendStrategy)
- description and source-code
```javascript
function ParallelSendStrategy(addresses, port, request) {
  (0, _classCallCheck3.default)(this, ParallelSendStrategy);

  this.addresses = addresses;
  this.port = port;
  this.request = request;

  this.socketV4 = null;
  this.socketV6 = null;
  this.onError = null;
  this.onMessage = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tedious.sender.Sender"></a>[function <span class="apidocSignatureSpan">tedious.sender.</span>Sender (host, port, request)](#apidoc.element.tedious.sender.Sender)
- description and source-code
```javascript
function Sender(host, port, request) {
  (0, _classCallCheck3.default)(this, Sender);

  this.host = host;
  this.port = port;
  this.request = request;

  this.parallelSendStrategy = null;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tedious.transaction"></a>[module tedious.transaction](#apidoc.module.tedious.transaction)

#### <a name="apidoc.element.tedious.transaction.Transaction"></a>[function <span class="apidocSignatureSpan">tedious.transaction.</span>Transaction (name, isolationLevel)](#apidoc.element.tedious.transaction.Transaction)
- description and source-code
```javascript
function Transaction(name, isolationLevel) {
  (0, _classCallCheck3.default)(this, Transaction);

  this.name = name;
  this.isolationLevel = isolationLevel;
  this.outstandingRequestCount = 1;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
