# api documentation for  [rethinkdbdash (v2.3.28)](https://github.com/neumino/rethinkdbdash#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-rethinkdbdash.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-rethinkdbdash) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-rethinkdbdash.svg)](https://travis-ci.org/npmdoc/node-npmdoc-rethinkdbdash)
#### A Node.js driver for RethinkDB with promises and a connection pool

[![NPM](https://nodei.co/npm/rethinkdbdash.png?downloads=true)](https://www.npmjs.com/package/rethinkdbdash)

[![apidoc](https://npmdoc.github.io/node-npmdoc-rethinkdbdash/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-rethinkdbdash_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-rethinkdbdash/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-rethinkdbdash/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-rethinkdbdash/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Michel Tu",
        "email": "orphee@gmail.com",
        "url": "http://justonepixel.com/"
    },
    "bugs": {
        "url": "https://github.com/neumino/rethinkdbdash/issues"
    },
    "dependencies": {
        "bluebird": ">= 3.0.1"
    },
    "description": "A Node.js driver for RethinkDB with promises and a connection pool",
    "devDependencies": {
        "dev-null": ">= 0.1.1",
        "mocha": ">= 1.20.0"
    },
    "directories": {
        "test": "test"
    },
    "dist": {
        "shasum": "f15fed3a2f0c178155fcadb6fc212b3df80f73df",
        "tarball": "https://registry.npmjs.org/rethinkdbdash/-/rethinkdbdash-2.3.28.tgz"
    },
    "gitHead": "71d512b1285a8b75239f9203e5cbedfd3f263dd2",
    "homepage": "https://github.com/neumino/rethinkdbdash#readme",
    "keywords": [
        "rethinkdb",
        "driver",
        "nodejs"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "neumino",
            "email": "orphee@gmail.com"
        }
    ],
    "name": "rethinkdbdash",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/neumino/rethinkdbdash.git"
    },
    "scripts": {
        "browserify": "node browserify.js",
        "test": "mocha --check-leaks -t 20000"
    },
    "version": "2.3.28"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module rethinkdbdash](#apidoc.module.rethinkdbdash)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>connection (r, options, resolve, reject)](#apidoc.element.rethinkdbdash.connection)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>cursor (connection, token, options, type)](#apidoc.element.rethinkdbdash.cursor)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>dequeue (size)](#apidoc.element.rethinkdbdash.dequeue)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>metadata (resolve, reject, query, options)](#apidoc.element.rethinkdbdash.metadata)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>pool (r, options)](#apidoc.element.rethinkdbdash.pool)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>pool_master (r, options)](#apidoc.element.rethinkdbdash.pool_master)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>stream (options, cursor)](#apidoc.element.rethinkdbdash.stream)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>term (r, value, error)](#apidoc.element.rethinkdbdash.term)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>transform_stream (table, options, connection)](#apidoc.element.rethinkdbdash.transform_stream)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>writable_stream (table, options, connection)](#apidoc.element.rethinkdbdash.writable_stream)
1.  object <span class="apidocSignatureSpan">rethinkdbdash.</span>connection.prototype
1.  object <span class="apidocSignatureSpan">rethinkdbdash.</span>cursor.prototype
1.  object <span class="apidocSignatureSpan">rethinkdbdash.</span>dequeue.prototype
1.  object <span class="apidocSignatureSpan">rethinkdbdash.</span>error
1.  object <span class="apidocSignatureSpan">rethinkdbdash.</span>helper
1.  object <span class="apidocSignatureSpan">rethinkdbdash.</span>metadata.prototype
1.  object <span class="apidocSignatureSpan">rethinkdbdash.</span>pool.prototype
1.  object <span class="apidocSignatureSpan">rethinkdbdash.</span>pool_master.prototype
1.  object <span class="apidocSignatureSpan">rethinkdbdash.</span>stream.prototype
1.  object <span class="apidocSignatureSpan">rethinkdbdash.</span>term.prototype
1.  object <span class="apidocSignatureSpan">rethinkdbdash.</span>transform_stream.prototype
1.  object <span class="apidocSignatureSpan">rethinkdbdash.</span>writable_stream.prototype

#### [module rethinkdbdash.connection](#apidoc.module.rethinkdbdash.connection)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>connection (r, options, resolve, reject)](#apidoc.element.rethinkdbdash.connection.connection)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.</span>super_ ()](#apidoc.element.rethinkdbdash.connection.super_)

#### [module rethinkdbdash.connection.prototype](#apidoc.module.rethinkdbdash.connection.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_abort ()](#apidoc.element.rethinkdbdash.connection.prototype._abort)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_checkProtocolVersion (messageServer, reject)](#apidoc.element.rethinkdbdash.connection.prototype._checkProtocolVersion)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_compareDigest (messageServer, resolve, reject)](#apidoc.element.rethinkdbdash.connection.prototype._compareDigest)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_computeSaltedPassword (messageServer, reject)](#apidoc.element.rethinkdbdash.connection.prototype._computeSaltedPassword)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_continue (token, resolve, reject)](#apidoc.element.rethinkdbdash.connection.prototype._continue)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_end (token, resolve, reject)](#apidoc.element.rethinkdbdash.connection.prototype._end)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_flush ()](#apidoc.element.rethinkdbdash.connection.prototype._flush)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_getToken ()](#apidoc.element.rethinkdbdash.connection.prototype._getToken)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_isConnection ()](#apidoc.element.rethinkdbdash.connection.prototype._isConnection)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_isOpen ()](#apidoc.element.rethinkdbdash.connection.prototype._isOpen)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_processResponse (response, token)](#apidoc.element.rethinkdbdash.connection.prototype._processResponse)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_send (query, token, resolve, reject, originalQuery, options, end)](#apidoc.element.rethinkdbdash.connection.prototype._send)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_sendProof (authentication, randomNonce, saltedPassword)](#apidoc.element.rethinkdbdash.connection.prototype._sendProof)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>close (options, callback)](#apidoc.element.rethinkdbdash.connection.prototype.close)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>noReplyWait ()](#apidoc.element.rethinkdbdash.connection.prototype.noReplyWait)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>noreplyWait (callback)](#apidoc.element.rethinkdbdash.connection.prototype.noreplyWait)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>reconnect (options, callback)](#apidoc.element.rethinkdbdash.connection.prototype.reconnect)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>server (callback)](#apidoc.element.rethinkdbdash.connection.prototype.server)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>use (db)](#apidoc.element.rethinkdbdash.connection.prototype.use)

#### [module rethinkdbdash.cursor](#apidoc.module.rethinkdbdash.cursor)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>cursor (connection, token, options, type)](#apidoc.element.rethinkdbdash.cursor.cursor)

#### [module rethinkdbdash.cursor.prototype](#apidoc.module.rethinkdbdash.cursor.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_done ()](#apidoc.element.rethinkdbdash.cursor.prototype._done)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_each (callback, onFinish)](#apidoc.element.rethinkdbdash.cursor.prototype._each)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_eachAsync (callback)](#apidoc.element.rethinkdbdash.cursor.prototype._eachAsync)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_eachAsyncInternal (callback, finalResolve, finalReject)](#apidoc.element.rethinkdbdash.cursor.prototype._eachAsyncInternal)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_eachCb (err, data)](#apidoc.element.rethinkdbdash.cursor.prototype._eachCb)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_fetch ()](#apidoc.element.rethinkdbdash.cursor.prototype._fetch)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_flush ()](#apidoc.element.rethinkdbdash.cursor.prototype._flush)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_makeEmitter ()](#apidoc.element.rethinkdbdash.cursor.prototype._makeEmitter)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_next (callback)](#apidoc.element.rethinkdbdash.cursor.prototype._next)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_push (data)](#apidoc.element.rethinkdbdash.cursor.prototype._push)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_pushError (error)](#apidoc.element.rethinkdbdash.cursor.prototype._pushError)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_set (ar)](#apidoc.element.rethinkdbdash.cursor.prototype._set)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_unsupportedToArray ()](#apidoc.element.rethinkdbdash.cursor.prototype._unsupportedToArray)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>addListener ()](#apidoc.element.rethinkdbdash.cursor.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>close (callback)](#apidoc.element.rethinkdbdash.cursor.prototype.close)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>each (callback, onFinish)](#apidoc.element.rethinkdbdash.cursor.prototype.each)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>eachAsync (callback)](#apidoc.element.rethinkdbdash.cursor.prototype.eachAsync)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>emit ()](#apidoc.element.rethinkdbdash.cursor.prototype.emit)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>getType ()](#apidoc.element.rethinkdbdash.cursor.prototype.getType)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>hasNext ()](#apidoc.element.rethinkdbdash.cursor.prototype.hasNext)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>includesStates ()](#apidoc.element.rethinkdbdash.cursor.prototype.includesStates)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>listeners ()](#apidoc.element.rethinkdbdash.cursor.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>next (callback)](#apidoc.element.rethinkdbdash.cursor.prototype.next)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>on ()](#apidoc.element.rethinkdbdash.cursor.prototype.on)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>once ()](#apidoc.element.rethinkdbdash.cursor.prototype.once)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>removeAllListeners ()](#apidoc.element.rethinkdbdash.cursor.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>removeListener ()](#apidoc.element.rethinkdbdash.cursor.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>setIncludesStates ()](#apidoc.element.rethinkdbdash.cursor.prototype.setIncludesStates)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>setMaxListeners ()](#apidoc.element.rethinkdbdash.cursor.prototype.setMaxListeners)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>toArray (callback)](#apidoc.element.rethinkdbdash.cursor.prototype.toArray)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>toJSON ()](#apidoc.element.rethinkdbdash.cursor.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>toString ()](#apidoc.element.rethinkdbdash.cursor.prototype.toString)

#### [module rethinkdbdash.dequeue](#apidoc.module.rethinkdbdash.dequeue)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>dequeue (size)](#apidoc.element.rethinkdbdash.dequeue.dequeue)

#### [module rethinkdbdash.dequeue.prototype](#apidoc.module.rethinkdbdash.dequeue.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>delete (index)](#apidoc.element.rethinkdbdash.dequeue.prototype.delete)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>get (index)](#apidoc.element.rethinkdbdash.dequeue.prototype.get)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>getLength ()](#apidoc.element.rethinkdbdash.dequeue.prototype.getLength)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>pop (element)](#apidoc.element.rethinkdbdash.dequeue.prototype.pop)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>push (element)](#apidoc.element.rethinkdbdash.dequeue.prototype.push)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>shift ()](#apidoc.element.rethinkdbdash.dequeue.prototype.shift)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>toArray (index)](#apidoc.element.rethinkdbdash.dequeue.prototype.toArray)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>unshift (element)](#apidoc.element.rethinkdbdash.dequeue.prototype.unshift)

#### [module rethinkdbdash.error](#apidoc.module.rethinkdbdash.error)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.error.</span>ReqlClientError (message)](#apidoc.element.rethinkdbdash.error.ReqlClientError)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.error.</span>ReqlCompileError (message, query, frames)](#apidoc.element.rethinkdbdash.error.ReqlCompileError)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.error.</span>ReqlDriverError (message, query, secondMessage)](#apidoc.element.rethinkdbdash.error.ReqlDriverError)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.error.</span>ReqlRuntimeError (message, query, frames)](#apidoc.element.rethinkdbdash.error.ReqlRuntimeError)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.error.</span>ReqlServerError (message, query)](#apidoc.element.rethinkdbdash.error.ReqlServerError)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.error.</span>generateBacktrace (term, index, father, frames, options)](#apidoc.element.rethinkdbdash.error.generateBacktrace)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.error.</span>setOperational (error)](#apidoc.element.rethinkdbdash.error.setOperational)

#### [module rethinkdbdash.helper](#apidoc.module.rethinkdbdash.helper)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>changeProto (object, other)](#apidoc.element.rethinkdbdash.helper.changeProto)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>compareDigest (a, b)](#apidoc.element.rethinkdbdash.helper.compareDigest)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>createLogger (poolMaster, silent)](#apidoc.element.rethinkdbdash.helper.createLogger)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>getCanonicalAddress (addresses)](#apidoc.element.rethinkdbdash.helper.getCanonicalAddress)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>hasImplicit (arg)](#apidoc.element.rethinkdbdash.helper.hasImplicit)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>isPlainObject (obj)](#apidoc.element.rethinkdbdash.helper.isPlainObject)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>loopKeys (obj, fn)](#apidoc.element.rethinkdbdash.helper.loopKeys)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>makeAtom (response, options)](#apidoc.element.rethinkdbdash.helper.makeAtom)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>makeSequence (response, options)](#apidoc.element.rethinkdbdash.helper.makeSequence)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>splitCommaEqual (message)](#apidoc.element.rethinkdbdash.helper.splitCommaEqual)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>toArray (args)](#apidoc.element.rethinkdbdash.helper.toArray)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>tryCatch (toTry, handleError)](#apidoc.element.rethinkdbdash.helper.tryCatch)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>xorBuffer (a, b)](#apidoc.element.rethinkdbdash.helper.xorBuffer)
1.  object <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>localhostAliases

#### [module rethinkdbdash.metadata](#apidoc.module.rethinkdbdash.metadata)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>metadata (resolve, reject, query, options)](#apidoc.element.rethinkdbdash.metadata.metadata)

#### [module rethinkdbdash.metadata.prototype](#apidoc.module.rethinkdbdash.metadata.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.metadata.prototype.</span>removeCallbacks ()](#apidoc.element.rethinkdbdash.metadata.prototype.removeCallbacks)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.metadata.prototype.</span>removeEndCallbacks ()](#apidoc.element.rethinkdbdash.metadata.prototype.removeEndCallbacks)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.metadata.prototype.</span>setCallbacks (resolve, reject)](#apidoc.element.rethinkdbdash.metadata.prototype.setCallbacks)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.metadata.prototype.</span>setCursor ()](#apidoc.element.rethinkdbdash.metadata.prototype.setCursor)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.metadata.prototype.</span>setEnd (resolve, reject)](#apidoc.element.rethinkdbdash.metadata.prototype.setEnd)

#### [module rethinkdbdash.pool](#apidoc.module.rethinkdbdash.pool)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>pool (r, options)](#apidoc.element.rethinkdbdash.pool.pool)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool.</span>super_ ()](#apidoc.element.rethinkdbdash.pool.super_)

#### [module rethinkdbdash.pool.prototype](#apidoc.module.rethinkdbdash.pool.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>_aggressivelyExpandBuffer ()](#apidoc.element.rethinkdbdash.pool.prototype._aggressivelyExpandBuffer)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>_decreaseNumConnections ()](#apidoc.element.rethinkdbdash.pool.prototype._decreaseNumConnections)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>_expandBuffer ()](#apidoc.element.rethinkdbdash.pool.prototype._expandBuffer)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>_increaseNumConnections ()](#apidoc.element.rethinkdbdash.pool.prototype._increaseNumConnections)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>createConnection ()](#apidoc.element.rethinkdbdash.pool.prototype.createConnection)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>drain ()](#apidoc.element.rethinkdbdash.pool.prototype.drain)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>drainLocalhost ()](#apidoc.element.rethinkdbdash.pool.prototype.drainLocalhost)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>getAddress ()](#apidoc.element.rethinkdbdash.pool.prototype.getAddress)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>getAvailableLength ()](#apidoc.element.rethinkdbdash.pool.prototype.getAvailableLength)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>getConnection ()](#apidoc.element.rethinkdbdash.pool.prototype.getConnection)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>getLength ()](#apidoc.element.rethinkdbdash.pool.prototype.getLength)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>putConnection (connection)](#apidoc.element.rethinkdbdash.pool.prototype.putConnection)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>setOptions (options)](#apidoc.element.rethinkdbdash.pool.prototype.setOptions)

#### [module rethinkdbdash.pool_master](#apidoc.module.rethinkdbdash.pool_master)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>pool_master (r, options)](#apidoc.element.rethinkdbdash.pool_master.pool_master)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.</span>super_ ()](#apidoc.element.rethinkdbdash.pool_master.super_)

#### [module rethinkdbdash.pool_master.prototype](#apidoc.module.rethinkdbdash.pool_master.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>_expandAll ()](#apidoc.element.rethinkdbdash.pool_master.prototype._expandAll)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>_flushErrors ()](#apidoc.element.rethinkdbdash.pool_master.prototype._flushErrors)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>createPool (server)](#apidoc.element.rethinkdbdash.pool_master.prototype.createPool)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>createPoolSettings (globalOptions, serverOptions, log)](#apidoc.element.rethinkdbdash.pool_master.prototype.createPoolSettings)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>deletePool (key)](#apidoc.element.rethinkdbdash.pool_master.prototype.deletePool)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>drain ()](#apidoc.element.rethinkdbdash.pool_master.prototype.drain)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>emitStatus ()](#apidoc.element.rethinkdbdash.pool_master.prototype.emitStatus)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>fetchServers (useSeeds)](#apidoc.element.rethinkdbdash.pool_master.prototype.fetchServers)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>getAvailableLength ()](#apidoc.element.rethinkdbdash.pool_master.prototype.getAvailableLength)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>getConnection ()](#apidoc.element.rethinkdbdash.pool_master.prototype.getConnection)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>getLength ()](#apidoc.element.rethinkdbdash.pool_master.prototype.getLength)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>getNumAvailableConnections ()](#apidoc.element.rethinkdbdash.pool_master.prototype.getNumAvailableConnections)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>getNumConnections ()](#apidoc.element.rethinkdbdash.pool_master.prototype.getNumConnections)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>getPools ()](#apidoc.element.rethinkdbdash.pool_master.prototype.getPools)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>handleAllServersResponse (servers)](#apidoc.element.rethinkdbdash.pool_master.prototype.handleAllServersResponse)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>initPool (pool)](#apidoc.element.rethinkdbdash.pool_master.prototype.initPool)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>resetBufferParameters ()](#apidoc.element.rethinkdbdash.pool_master.prototype.resetBufferParameters)

#### [module rethinkdbdash.stream](#apidoc.module.rethinkdbdash.stream)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>stream (options, cursor)](#apidoc.element.rethinkdbdash.stream.stream)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.stream.</span>super_ (options)](#apidoc.element.rethinkdbdash.stream.super_)

#### [module rethinkdbdash.stream.prototype](#apidoc.module.rethinkdbdash.stream.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.stream.prototype.</span>_fetch ()](#apidoc.element.rethinkdbdash.stream.prototype._fetch)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.stream.prototype.</span>_fetchAndDecrement ()](#apidoc.element.rethinkdbdash.stream.prototype._fetchAndDecrement)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.stream.prototype.</span>_read (size)](#apidoc.element.rethinkdbdash.stream.prototype._read)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.stream.prototype.</span>_setCursor (cursor)](#apidoc.element.rethinkdbdash.stream.prototype._setCursor)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.stream.prototype.</span>close ()](#apidoc.element.rethinkdbdash.stream.prototype.close)

#### [module rethinkdbdash.term](#apidoc.module.rethinkdbdash.term)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>term (r, value, error)](#apidoc.element.rethinkdbdash.term.term)

#### [module rethinkdbdash.term.prototype](#apidoc.module.rethinkdbdash.term.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>ISO8601 (isoTime, options)](#apidoc.element.rethinkdbdash.term.prototype.ISO8601)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_arity (args, num, method, term)](#apidoc.element.rethinkdbdash.term.prototype._arity)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_arityRange (args, min, max, method, term)](#apidoc.element.rethinkdbdash.term.prototype._arityRange)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_fastArity (len, num)](#apidoc.element.rethinkdbdash.term.prototype._fastArity)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_fastArityRange (len, min, max)](#apidoc.element.rethinkdbdash.term.prototype._fastArityRange)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_fillArgs (args)](#apidoc.element.rethinkdbdash.term.prototype._fillArgs)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_noPrefix (term, method)](#apidoc.element.rethinkdbdash.term.prototype._noPrefix)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_setArrayLimit (arrayLimit)](#apidoc.element.rethinkdbdash.term.prototype._setArrayLimit)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_setNestingLevel (nestingLevel)](#apidoc.element.rethinkdbdash.term.prototype._setNestingLevel)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_toReadableStream (connection, options)](#apidoc.element.rethinkdbdash.term.prototype._toReadableStream)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_toTransformStream (connection, options)](#apidoc.element.rethinkdbdash.term.prototype._toTransformStream)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_toWritableStream (connection, options)](#apidoc.element.rethinkdbdash.term.prototype._toWritableStream)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_wrap ()](#apidoc.element.rethinkdbdash.term.prototype._wrap)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>add ()](#apidoc.element.rethinkdbdash.term.prototype.add)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>and ()](#apidoc.element.rethinkdbdash.term.prototype.and)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>append (value)](#apidoc.element.rethinkdbdash.term.prototype.append)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>april ()](#apidoc.element.rethinkdbdash.term.prototype.april)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>args ()](#apidoc.element.rethinkdbdash.term.prototype.args)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>asc (field)](#apidoc.element.rethinkdbdash.term.prototype.asc)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>august ()](#apidoc.element.rethinkdbdash.term.prototype.august)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>avg (field)](#apidoc.element.rethinkdbdash.term.prototype.avg)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>between (start, end, options)](#apidoc.element.rethinkdbdash.term.prototype.between)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>binary (bin)](#apidoc.element.rethinkdbdash.term.prototype.binary)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>bracket (field)](#apidoc.element.rethinkdbdash.term.prototype.bracket)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>branch ()](#apidoc.element.rethinkdbdash.term.prototype.branch)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>catch (reject)](#apidoc.element.rethinkdbdash.term.prototype.catch)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>ceil ()](#apidoc.element.rethinkdbdash.term.prototype.ceil)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>changeAt (index, value)](#apidoc.element.rethinkdbdash.term.prototype.changeAt)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>changes (options)](#apidoc.element.rethinkdbdash.term.prototype.changes)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>circle (center, radius, options)](#apidoc.element.rethinkdbdash.term.prototype.circle)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>coerceTo (type)](#apidoc.element.rethinkdbdash.term.prototype.coerceTo)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>concatMap (transformation)](#apidoc.element.rethinkdbdash.term.prototype.concatMap)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>config ()](#apidoc.element.rethinkdbdash.term.prototype.config)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>contains ()](#apidoc.element.rethinkdbdash.term.prototype.contains)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>count (filter)](#apidoc.element.rethinkdbdash.term.prototype.count)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>date ()](#apidoc.element.rethinkdbdash.term.prototype.date)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>day ()](#apidoc.element.rethinkdbdash.term.prototype.day)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>dayOfWeek ()](#apidoc.element.rethinkdbdash.term.prototype.dayOfWeek)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>dayOfYear ()](#apidoc.element.rethinkdbdash.term.prototype.dayOfYear)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>db (db)](#apidoc.element.rethinkdbdash.term.prototype.db)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>dbCreate (db)](#apidoc.element.rethinkdbdash.term.prototype.dbCreate)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>dbDrop (db)](#apidoc.element.rethinkdbdash.term.prototype.dbDrop)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>dbList ()](#apidoc.element.rethinkdbdash.term.prototype.dbList)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>december ()](#apidoc.element.rethinkdbdash.term.prototype.december)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>default (expression)](#apidoc.element.rethinkdbdash.term.prototype.default)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>delay (msecs)](#apidoc.element.rethinkdbdash.term.prototype.delay)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>delete (options)](#apidoc.element.rethinkdbdash.term.prototype.delete)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>deleteAt (start, end)](#apidoc.element.rethinkdbdash.term.prototype.deleteAt)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>desc (field)](#apidoc.element.rethinkdbdash.term.prototype.desc)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>difference (other)](#apidoc.element.rethinkdbdash.term.prototype.difference)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>distance (geometry, options)](#apidoc.element.rethinkdbdash.term.prototype.distance)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>distinct (options)](#apidoc.element.rethinkdbdash.term.prototype.distinct)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>div ()](#apidoc.element.rethinkdbdash.term.prototype.div)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>do ()](#apidoc.element.rethinkdbdash.term.prototype.do)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>downcase (regex)](#apidoc.element.rethinkdbdash.term.prototype.downcase)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>during (left, right, options)](#apidoc.element.rethinkdbdash.term.prototype.during)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>epochTime (epochTime)](#apidoc.element.rethinkdbdash.term.prototype.epochTime)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>eq ()](#apidoc.element.rethinkdbdash.term.prototype.eq)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>eqJoin (rightKey, sequence, options)](#apidoc.element.rethinkdbdash.term.prototype.eqJoin)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>error (reject)](#apidoc.element.rethinkdbdash.term.prototype.error)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>expr (expression, nestingLevel)](#apidoc.element.rethinkdbdash.term.prototype.expr)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>february ()](#apidoc.element.rethinkdbdash.term.prototype.february)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>fill ()](#apidoc.element.rethinkdbdash.term.prototype.fill)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>filter (filter, options)](#apidoc.element.rethinkdbdash.term.prototype.filter)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>finally (handler)](#apidoc.element.rethinkdbdash.term.prototype.finally)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>floor ()](#apidoc.element.rethinkdbdash.term.prototype.floor)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>fold (base, func, options)](#apidoc.element.rethinkdbdash.term.prototype.fold)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>forEach (func)](#apidoc.element.rethinkdbdash.term.prototype.forEach)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>friday ()](#apidoc.element.rethinkdbdash.term.prototype.friday)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>ge (other)](#apidoc.element.rethinkdbdash.term.prototype.ge)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>geojson (geometry)](#apidoc.element.rethinkdbdash.term.prototype.geojson)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>get (primaryKey)](#apidoc.element.rethinkdbdash.term.prototype.get)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>getAll ()](#apidoc.element.rethinkdbdash.term.prototype.getAll)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>getField (field)](#apidoc.element.rethinkdbdash.term.prototype.getField)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>getIntersecting (geometry, options)](#apidoc.element.rethinkdbdash.term.prototype.getIntersecting)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>getNearest (geometry, options)](#apidoc.element.rethinkdbdash.term.prototype.getNearest)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>grant (name, access)](#apidoc.element.rethinkdbdash.term.prototype.grant)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>group ()](#apidoc.element.rethinkdbdash.term.prototype.group)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>gt (other)](#apidoc.element.rethinkdbdash.term.prototype.gt)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>hasFields ()](#apidoc.element.rethinkdbdash.term.prototype.hasFields)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>hours ()](#apidoc.element.rethinkdbdash.term.prototype.hours)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>http (url, options)](#apidoc.element.rethinkdbdash.term.prototype.http)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>inTimezone (timezone)](#apidoc.element.rethinkdbdash.term.prototype.inTimezone)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>includes (geometry)](#apidoc.element.rethinkdbdash.term.prototype.includes)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>indexCreate (name, fn, options)](#apidoc.element.rethinkdbdash.term.prototype.indexCreate)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>indexDrop (name)](#apidoc.element.rethinkdbdash.term.prototype.indexDrop)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>indexList ()](#apidoc.element.rethinkdbdash.term.prototype.indexList)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>indexRename (oldName, newName, options)](#apidoc.element.rethinkdbdash.term.prototype.indexRename)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>indexStatus ()](#apidoc.element.rethinkdbdash.term.prototype.indexStatus)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>indexWait ()](#apidoc.element.rethinkdbdash.term.prototype.indexWait)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>indexesOf (predicate)](#apidoc.element.rethinkdbdash.term.prototype.indexesOf)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>info ()](#apidoc.element.rethinkdbdash.term.prototype.info)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>innerJoin (sequence, predicate)](#apidoc.element.rethinkdbdash.term.prototype.innerJoin)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>insert (documents, options)](#apidoc.element.rethinkdbdash.term.prototype.insert)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>insertAt (index, value)](#apidoc.element.rethinkdbdash.term.prototype.insertAt)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>intersects (geometry)](#apidoc.element.rethinkdbdash.term.prototype.intersects)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>isEmpty ()](#apidoc.element.rethinkdbdash.term.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>january ()](#apidoc.element.rethinkdbdash.term.prototype.january)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>js (arg, options)](#apidoc.element.rethinkdbdash.term.prototype.js)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>json (json)](#apidoc.element.rethinkdbdash.term.prototype.json)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>july ()](#apidoc.element.rethinkdbdash.term.prototype.july)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>june ()](#apidoc.element.rethinkdbdash.term.prototype.june)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>keys ()](#apidoc.element.rethinkdbdash.term.prototype.keys)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>le (other)](#apidoc.element.rethinkdbdash.term.prototype.le)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>limit (value)](#apidoc.element.rethinkdbdash.term.prototype.limit)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>line ()](#apidoc.element.rethinkdbdash.term.prototype.line)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>literal (obj)](#apidoc.element.rethinkdbdash.term.prototype.literal)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>lt (other)](#apidoc.element.rethinkdbdash.term.prototype.lt)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>map ()](#apidoc.element.rethinkdbdash.term.prototype.map)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>march ()](#apidoc.element.rethinkdbdash.term.prototype.march)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>match (regex)](#apidoc.element.rethinkdbdash.term.prototype.match)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>max (field)](#apidoc.element.rethinkdbdash.term.prototype.max)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>maxval ()](#apidoc.element.rethinkdbdash.term.prototype.maxval)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>may ()](#apidoc.element.rethinkdbdash.term.prototype.may)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>merge (arg)](#apidoc.element.rethinkdbdash.term.prototype.merge)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>min (field)](#apidoc.element.rethinkdbdash.term.prototype.min)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>minutes ()](#apidoc.element.rethinkdbdash.term.prototype.minutes)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>minval ()](#apidoc.element.rethinkdbdash.term.prototype.minval)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>mod (b)](#apidoc.element.rethinkdbdash.term.prototype.mod)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>monday ()](#apidoc.element.rethinkdbdash.term.prototype.monday)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>month ()](#apidoc.element.rethinkdbdash.term.prototype.month)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>mul ()](#apidoc.element.rethinkdbdash.term.prototype.mul)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>ne ()](#apidoc.element.rethinkdbdash.term.prototype.ne)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>not ()](#apidoc.element.rethinkdbdash.term.prototype.not)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>november ()](#apidoc.element.rethinkdbdash.term.prototype.november)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>now ()](#apidoc.element.rethinkdbdash.term.prototype.now)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>nth (value)](#apidoc.element.rethinkdbdash.term.prototype.nth)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>object ()](#apidoc.element.rethinkdbdash.term.prototype.object)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>october ()](#apidoc.element.rethinkdbdash.term.prototype.october)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>offsetsOf (predicate)](#apidoc.element.rethinkdbdash.term.prototype.offsetsOf)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>or ()](#apidoc.element.rethinkdbdash.term.prototype.or)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>orderBy ()](#apidoc.element.rethinkdbdash.term.prototype.orderBy)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>outerJoin (sequence, predicate)](#apidoc.element.rethinkdbdash.term.prototype.outerJoin)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>pluck ()](#apidoc.element.rethinkdbdash.term.prototype.pluck)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>point (longitude, latitude)](#apidoc.element.rethinkdbdash.term.prototype.point)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>polygon ()](#apidoc.element.rethinkdbdash.term.prototype.polygon)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>polygonSub (geometry)](#apidoc.element.rethinkdbdash.term.prototype.polygonSub)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>prepend (value)](#apidoc.element.rethinkdbdash.term.prototype.prepend)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>random ()](#apidoc.element.rethinkdbdash.term.prototype.random)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>range (start, end)](#apidoc.element.rethinkdbdash.term.prototype.range)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>rebalance ()](#apidoc.element.rethinkdbdash.term.prototype.rebalance)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>reconfigure (config)](#apidoc.element.rethinkdbdash.term.prototype.reconfigure)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>reduce (func)](#apidoc.element.rethinkdbdash.term.prototype.reduce)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>replace (newValue, options)](#apidoc.element.rethinkdbdash.term.prototype.replace)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>round ()](#apidoc.element.rethinkdbdash.term.prototype.round)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>row ()](#apidoc.element.rethinkdbdash.term.prototype.row)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>run (connection, options, callback)](#apidoc.element.rethinkdbdash.term.prototype.run)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>sample (size)](#apidoc.element.rethinkdbdash.term.prototype.sample)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>saturday ()](#apidoc.element.rethinkdbdash.term.prototype.saturday)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>seconds ()](#apidoc.element.rethinkdbdash.term.prototype.seconds)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>september ()](#apidoc.element.rethinkdbdash.term.prototype.september)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>setDifference (other)](#apidoc.element.rethinkdbdash.term.prototype.setDifference)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>setInsert (other)](#apidoc.element.rethinkdbdash.term.prototype.setInsert)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>setIntersection (other)](#apidoc.element.rethinkdbdash.term.prototype.setIntersection)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>setUnion (other)](#apidoc.element.rethinkdbdash.term.prototype.setUnion)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>skip (value)](#apidoc.element.rethinkdbdash.term.prototype.skip)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>slice (start, end, options)](#apidoc.element.rethinkdbdash.term.prototype.slice)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>spliceAt (index, array)](#apidoc.element.rethinkdbdash.term.prototype.spliceAt)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>split (separator, max)](#apidoc.element.rethinkdbdash.term.prototype.split)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>status ()](#apidoc.element.rethinkdbdash.term.prototype.status)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>sub ()](#apidoc.element.rethinkdbdash.term.prototype.sub)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>sum (field)](#apidoc.element.rethinkdbdash.term.prototype.sum)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>sunday ()](#apidoc.element.rethinkdbdash.term.prototype.sunday)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>sync ()](#apidoc.element.rethinkdbdash.term.prototype.sync)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>table (table, options)](#apidoc.element.rethinkdbdash.term.prototype.table)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>tableCreate (table, options)](#apidoc.element.rethinkdbdash.term.prototype.tableCreate)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>tableDrop (table)](#apidoc.element.rethinkdbdash.term.prototype.tableDrop)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>tableList ()](#apidoc.element.rethinkdbdash.term.prototype.tableList)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>then (resolve, reject)](#apidoc.element.rethinkdbdash.term.prototype.then)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>thursday ()](#apidoc.element.rethinkdbdash.term.prototype.thursday)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>time ()](#apidoc.element.rethinkdbdash.term.prototype.time)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>timeOfDay ()](#apidoc.element.rethinkdbdash.term.prototype.timeOfDay)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>timezone ()](#apidoc.element.rethinkdbdash.term.prototype.timezone)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>toEpochTime ()](#apidoc.element.rethinkdbdash.term.prototype.toEpochTime)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>toGeojson ()](#apidoc.element.rethinkdbdash.term.prototype.toGeojson)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>toISO8601 ()](#apidoc.element.rethinkdbdash.term.prototype.toISO8601)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>toJSON ()](#apidoc.element.rethinkdbdash.term.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>toJsonString ()](#apidoc.element.rethinkdbdash.term.prototype.toJsonString)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>toStream (connection, options)](#apidoc.element.rethinkdbdash.term.prototype.toStream)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>toString ()](#apidoc.element.rethinkdbdash.term.prototype.toString)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>tuesday ()](#apidoc.element.rethinkdbdash.term.prototype.tuesday)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>typeOf ()](#apidoc.element.rethinkdbdash.term.prototype.typeOf)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>ungroup ()](#apidoc.element.rethinkdbdash.term.prototype.ungroup)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>union ()](#apidoc.element.rethinkdbdash.term.prototype.union)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>upcase (regex)](#apidoc.element.rethinkdbdash.term.prototype.upcase)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>update (newValue, options)](#apidoc.element.rethinkdbdash.term.prototype.update)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>uuid (str)](#apidoc.element.rethinkdbdash.term.prototype.uuid)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>values ()](#apidoc.element.rethinkdbdash.term.prototype.values)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>wait (options)](#apidoc.element.rethinkdbdash.term.prototype.wait)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>wednesday ()](#apidoc.element.rethinkdbdash.term.prototype.wednesday)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>withFields ()](#apidoc.element.rethinkdbdash.term.prototype.withFields)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>without ()](#apidoc.element.rethinkdbdash.term.prototype.without)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>year ()](#apidoc.element.rethinkdbdash.term.prototype.year)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>zip ()](#apidoc.element.rethinkdbdash.term.prototype.zip)
1.  object <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_translateArgs

#### [module rethinkdbdash.transform_stream](#apidoc.module.rethinkdbdash.transform_stream)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>transform_stream (table, options, connection)](#apidoc.element.rethinkdbdash.transform_stream.transform_stream)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.transform_stream.</span>super_ (options)](#apidoc.element.rethinkdbdash.transform_stream.super_)

#### [module rethinkdbdash.transform_stream.prototype](#apidoc.module.rethinkdbdash.transform_stream.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.transform_stream.prototype.</span>_flush (done)](#apidoc.element.rethinkdbdash.transform_stream.prototype._flush)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.transform_stream.prototype.</span>_insert ()](#apidoc.element.rethinkdbdash.transform_stream.prototype._insert)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.transform_stream.prototype.</span>_next (value, encoding, done)](#apidoc.element.rethinkdbdash.transform_stream.prototype._next)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.transform_stream.prototype.</span>_transform (value, encoding, done)](#apidoc.element.rethinkdbdash.transform_stream.prototype._transform)

#### [module rethinkdbdash.writable_stream](#apidoc.module.rethinkdbdash.writable_stream)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.</span>writable_stream (table, options, connection)](#apidoc.element.rethinkdbdash.writable_stream.writable_stream)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.writable_stream.</span>super_ (options)](#apidoc.element.rethinkdbdash.writable_stream.super_)

#### [module rethinkdbdash.writable_stream.prototype](#apidoc.module.rethinkdbdash.writable_stream.prototype)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.writable_stream.prototype.</span>_insert ()](#apidoc.element.rethinkdbdash.writable_stream.prototype._insert)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.writable_stream.prototype.</span>_next (value, encoding, done)](#apidoc.element.rethinkdbdash.writable_stream.prototype._next)
1.  [function <span class="apidocSignatureSpan">rethinkdbdash.writable_stream.prototype.</span>_write (value, encoding, done)](#apidoc.element.rethinkdbdash.writable_stream.prototype._write)



# <a name="apidoc.module.rethinkdbdash"></a>[module rethinkdbdash](#apidoc.module.rethinkdbdash)

#### <a name="apidoc.element.rethinkdbdash.connection"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>connection (r, options, resolve, reject)](#apidoc.element.rethinkdbdash.connection)
- description and source-code
```javascript
function Connection(r, options, resolve, reject) {
  var self = this;
  this.r = r;
  this.state = 0; // Track the progress of the handshake. -1 will be used for an error state.

  // Set default options - We have to save them in case the user tries to reconnect
  if (!helper.isPlainObject(options)) options = {};
  this.host = options.host || r._host;
  this.port = options.port || r._port;
  if (options.authKey != null) {
    if (options.user != null || options.password != null) {
      throw new Err.ReqlDriverError('Cannot use both authKey and password');
    }
    this.user = r._user;
    this.password = options.authKey;
  } else {
    if (options.user === undefined) {
      this.user = r._user;
    } else {
      this.user = options.user;
    }
    if (options.password === undefined) {
      this.password = r._password;
    } else {
      this.password = options.password;
    }
  }

  this.authKey = options.authKey || r._authKey;
  // period in *seconds* for the connection to be opened
  this.timeoutConnect = options.timeout || r._timeoutConnect;
  // The connection will be pinged every <pingInterval> seconds
  this.pingInterval = options.pingInterval || r._pingInterval;

  if (options.db) this.db = options.db; // Pass to each query

  this.token = 1;
  this.buffer = new Buffer(0);

  this.metadata = {}

  this.open = false; // true only if the user can write on the socket
  this.timeout = null;

  if (options.connection) {
    this.connection = options.connection;
  }
  else {
    var family = 'IPv4';
    if (net.isIPv6(self.host)) {
      family = 'IPv6';
    }

    var connectionArgs = {
      host: self.host,
      port: self.port,
      family: family
    }

    var tlsOptions = options.ssl || false;
    if (tlsOptions === false) {
      self.connection = net.connect(connectionArgs);
    } else {
      if (helper.isPlainObject(tlsOptions)) {
        // Copy the TLS options in connectionArgs
        helper.loopKeys(tlsOptions, function(tlsOptions, key) {
          connectionArgs[key] = tlsOptions[key];
        });
      }
      self.connection = tls.connect(connectionArgs);
    }
  }

  self.connection.setKeepAlive(true);

  self.timeoutOpen = setTimeout(function() {
    self.connection.end(); // Send a FIN packet
    reject(new Err.ReqlDriverError('Failed to connect to '+self.host+':'+self.port+' in less than '+self.timeoutConnect+'s').setOperational
());
  }, self.timeoutConnect*1000);

  self.connection.on('end', function() {
    self.open = false;
    self.emit('end');
    // We got a FIN packet, so we'll just flush
    self._flush();
  });
  self.connection.on('close', function() {
    // We emit end or close just once
    clearTimeout(self.timeoutOpen)
    clearInterval(self.pingIntervalId);
    self.connection.removeAllListeners();
    self.open = false;
    self.emit('closed');
    // The connection is fully closed, flush (in case 'end' was not triggered)
    self._flush();
  });
  self.connection.setNoDelay();
  self.connection.once('error', function(error) {
    reject(new Err.ReqlDriverError('Failed to connect to '+self.host+':'+self.port+'\nFull error:\n'+JSON.stringify(error)).setOperational
());
  });
  self.connection.on('connect', function() {
    self.connection.removeAllListeners('error');
    self.connection.on('error', function(error) {
      self.emit('error', error);
    });

    var versionBuffer = new Buffer(4)
    versionBuffer.writeUInt32LE(protodef.VersionDummy.Version.V1_0, 0)

    self.randomString = new Buffer(crypto.randomBytes(18)).toString('base64')
    var authBuffer = new Buffer(JSON.stringify({
      protocol_version: PROTOCOL_VERSION,
      authentication_method: AUTHENTIFICATION_METHOD,
      authentication: "n,,n=" + self.user + ",r=" + self.randomString
    }));

    helper.tryCatch(function() {
      self.connection.write(Buffer.concat([versionBuffer, authBuffer, NULL_BUFFER]));
    }, function(err) {
      // The TCP connection is open, but the ReQL connection wasn't established.
      // We can just abort the whole thing
      self.open = false;
      reject(new Err.ReqlD ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>cursor (connection, token, options, type)](#apidoc.element.rethinkdbdash.cursor)
- description and source-code
```javascript
function Cursor(connection, token, options, type) {
  this.connection = connection;
  this.token = token;

  this._stackSize = 0; // Estimation of our call stack.
  this._index = 0; // Position in this._data[0]
  this._data = []; // Array of non empty arrays
  this._fetching = false; // Are we fetching data
  this._canFetch = true; // Can we fetch more data?
  this._pendingPromises = []; // Pending promises' resolve/reject
  this.options = options || {};
  this._closed = false;
  this._closingPromise = null; // Promise returned by close
  this._type = type;
  this._setIncludesStates = false;
  if ((type === 'feed') || (type === 'atomFeed')) {
    this.toArray = _unsupportedToArray;
  }
  this._emittedEnd = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.dequeue"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>dequeue (size)](#apidoc.element.rethinkdbdash.dequeue)
- description and source-code
```javascript
function Dequeue(size) {
  this.start = 0;
  this.end = 0;

  size = size || 50;
  this.buffer = new Array(size);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.metadata"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>metadata (resolve, reject, query, options)](#apidoc.element.rethinkdbdash.metadata)
- description and source-code
```javascript
function Metadata(resolve, reject, query, options) {
  this.resolve = resolve;
  this.reject = reject;
  this.query = query; // The query in case we have to build a backtrace
  this.options = options || {};
  this.cursor = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.pool"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>pool (r, options)](#apidoc.element.rethinkdbdash.pool)
- description and source-code
```javascript
function Pool(r, options) {
  this._r = r;

  if (!helper.isPlainObject(options)) options = {};
  this.options = {};
  this.options.max = options.max || 1000; // 4000 is about the maximum the kernel can take
  var buffer = (typeof options.buffer === 'number') ? options.buffer : 50;
  this.options.buffer = (buffer < this.options.max) ? buffer : this.options.max;
  this.options.timeoutError = options.timeoutError || 1000; // How long should we wait before recreating a connection that failed
?
  this.options.timeoutGb = options.timeoutGb || 60*60*1000; // Default timeout for TCP connection is 2 hours on Linux, we time out
 after one hour.
  this.options.maxExponent = options.maxExponent || 6; // Maximum timeout is 2^maxExponent*timeoutError

  this.options.silent = options.silent || false;

  this.options.connection = {
    host: options.host || this._r._host,
    port: options.port || this._r._port,
    db: options.db || this._r._db,
    timeout: options.timeout || this._r._timeoutConnect,
    authKey: options.authKey,
    user: options.user,
    password: options.password,
    cursor: options.cursor || false,
    stream: options.stream || false,
    ssl: options.ssl || false,
    pingInterval: options.pingInterval || this._r._pingInterval
  }
  this._log = options._log;

  this._pool = new Dequeue(this.options.buffer+1);
  this._draining = false;
  this._drainingHandlers = null; // Store the resolve/reject methods once draining is called
  this._localhostToDrain = 0; // number of connections to "localhost" to remove
  this._connectionToReplace = 0; // number of connections to "localhost" to remove

  this._numConnections = 0;
  this._openingConnections = 0; // Number of connections being opened
  this._consecutiveFails = 0;   // In slow growth, the number of consecutive failures to open a connection
  this._slowGrowth = false;     // Opening one connection at a time
  this._slowlyGrowing = false;  // The next connection to be returned is one opened in slowGrowth mode
  this._extraConnections = 0; // Number of extra connections being opened that we should eventually close

  this._empty = true;

  var self = this;
  // So we can let the pool master bind listeners
  setTimeout(function() {
    if (self._draining === false) {
      for(var i=0; i<self.options.buffer; i++) {
        if (self.getLength() < self.options.max) {
          self.createConnection();
        }
      }
    }
  }, 0);
  this.id = Math.floor(Math.random()*100000);
  this._log('Creating a pool connected to '+this.getAddress());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.pool_master"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>pool_master (r, options)](#apidoc.element.rethinkdbdash.pool_master)
- description and source-code
```javascript
function PoolMaster(r, options) {
  var self = this;
  var options = options || {};
  var lineLength = options.buffer || 50;

  self._r = r;
  self._line = new Dequeue(lineLength);
  self._pools = {};
  self._pools[UNKNOWN_POOLS] = []; // pools for which we do not know the server'id
  self._healthyPools = [];
  self._healthy = false;
  self._init = false;
  self._index = 0; // next pool to used
  self._indexUnknown =  0 // next unknown pool to used
  self._discovery = (typeof options.discovery === 'boolean') ? options.discovery: false; // Whether the pool master is in discovery
 mode or not
  //self._refresh = (typeof options.refresh === 'number') ? options.refresh: 1000*60*60; // Refresh rate for the list of servers
  self._options = options;
  self._options.buffer = options.buffer || 50;
  self._options.max = options.max || 1000;
  self._log = helper.createLogger(self, options.silent || false);
  self._draining = false;
  self._numConnections = 0;
  self._numAvailableConnections = 0;
  self._hasPrintWarningLocalhost = false;
  self._feed = null;
  self._consecutiveFails = -1;
  self._timeoutError = options.timeoutError || 1000; // How long should we wait before recreating a connection that failed?
  self._maxExponent = options.maxExponent || 6; // Maximum timeout is 2^maxExponent*timeoutError

  //TODO
  //self._usingPool = true; // If we have used the pool
  self._seed = 0;

  var pool;
  if (Array.isArray(options.servers)) {
    if (options.servers.length > 0) {
      self._servers = options.servers;
      for(var i=0; i<options.servers.length; i++) {
        var settings = self.createPoolSettings(options, options.servers[i], self._log);
        pool = new Pool(self._r, settings);
        self._pools[UNKNOWN_POOLS].push(pool);
        // A pool is considered healthy by default such that people can do
        // var = require(...)(); query.run();
        self._healthyPools.push(pool);
        self.emitStatus()
      }
    }
    else {
      throw new Err.ReqlDriverError("If 'servers' is an array, it must contain at least one server")
    }
  }
  else {
    self._servers = [{
      host: options.host || 'localhost',
      port: options.port || 28015
    }]
    var settings = self.createPoolSettings(options, {}, self._log);
    pool = new Pool(self._r, settings);
    self._pools[UNKNOWN_POOLS].push(pool);
    self._healthyPools.push(pool);
    self.emitStatus()
  }

  // Initialize all the pools - bind listeners
  for(var i=0; i<self._pools[UNKNOWN_POOLS].length; i++) {
    self.initPool(self._pools[UNKNOWN_POOLS][i]);
  }
  if ((self._discovery === true)) {
    self._timeout = setTimeout(function() { self.fetchServers() }, 0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.stream"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>stream (options, cursor)](#apidoc.element.rethinkdbdash.stream)
- description and source-code
```javascript
function ReadableStream(options, cursor) {
  if (cursor) this._cursor = cursor;
  this._pending = 0; // How many time we called _read while no cursor was available
  this._index = 0;
  this._maxRecursion = 1000; // Hardcoded
  this._highWaterMark = options.highWaterMark;
  this._closed = false;

  Readable.call(this, {
    objectMode: true,
    highWaterMark: this._highWaterMark
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>term (r, value, error)](#apidoc.element.rethinkdbdash.term)
- description and source-code
```javascript
function Term(r, value, error) {
  var self = this;
  var term = function(field) {
    if (Term.prototype._fastArity(arguments.length, 1) === false) {
      var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
      Term.prototype._arity(_args, 1, '(...)', self);
    }
    return term.bracket(field);
  }
  helper.changeProto(term, self);

  if (value === undefined) {
    term._query = [];
  }
  else {
    term._query = value;
  }
  term._r = r; // Keep a reference to r for global settings

  if (error !== undefined) {
    term._error = error;
    term._frames = [];
  }

  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.transform_stream"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>transform_stream (table, options, connection)](#apidoc.element.rethinkdbdash.transform_stream)
- description and source-code
```javascript
function TransformStream(table, options, connection) {
  this._table = table;
  this._r = table._r;
  this._options = options;
  this._cache = [];
  this._pendingCallback = null;
  this._ended = false;
  this._inserting = false;
  this._delayed = false;
  this._connection = connection;
  this._highWaterMark = options.highWaterMark || 100;
  this._insertOptions = {};
  this._insertOptions.durability = options.durability || 'hard';
  this._insertOptions.conflict = options.conflict || 'error';
  this._insertOptions.returnChanges = options.returnChanges || true;

  // Internal option to run some tests
  if (options.debug === true) {
    this._sequence = [];
  }

  Transform.call(this, {
    objectMode: true,
    highWaterMark: this._highWaterMark
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.writable_stream"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>writable_stream (table, options, connection)](#apidoc.element.rethinkdbdash.writable_stream)
- description and source-code
```javascript
function WritableStream(table, options, connection) {
  this._table = table;
  this._options = options;
  this._cache = [];
  this._pendingCallback = null;
  this._inserting = false;
  this._delayed = false;
  this._connection = connection;
  this._highWaterMark = options.highWaterMark || 100;

  this._insertOptions = {};
  this._insertOptions.durability = options.durability || 'hard';
  this._insertOptions.conflict = options.conflict || 'error';

  // Internal option to run some tests
  if (options.debug === true) {
    this._sequence = [];
  }

  Writable.call(this, {
    objectMode: true,
    highWaterMark: this._highWaterMark
  });
  this._i = 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.connection"></a>[module rethinkdbdash.connection](#apidoc.module.rethinkdbdash.connection)

#### <a name="apidoc.element.rethinkdbdash.connection.connection"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>connection (r, options, resolve, reject)](#apidoc.element.rethinkdbdash.connection.connection)
- description and source-code
```javascript
function Connection(r, options, resolve, reject) {
  var self = this;
  this.r = r;
  this.state = 0; // Track the progress of the handshake. -1 will be used for an error state.

  // Set default options - We have to save them in case the user tries to reconnect
  if (!helper.isPlainObject(options)) options = {};
  this.host = options.host || r._host;
  this.port = options.port || r._port;
  if (options.authKey != null) {
    if (options.user != null || options.password != null) {
      throw new Err.ReqlDriverError('Cannot use both authKey and password');
    }
    this.user = r._user;
    this.password = options.authKey;
  } else {
    if (options.user === undefined) {
      this.user = r._user;
    } else {
      this.user = options.user;
    }
    if (options.password === undefined) {
      this.password = r._password;
    } else {
      this.password = options.password;
    }
  }

  this.authKey = options.authKey || r._authKey;
  // period in *seconds* for the connection to be opened
  this.timeoutConnect = options.timeout || r._timeoutConnect;
  // The connection will be pinged every <pingInterval> seconds
  this.pingInterval = options.pingInterval || r._pingInterval;

  if (options.db) this.db = options.db; // Pass to each query

  this.token = 1;
  this.buffer = new Buffer(0);

  this.metadata = {}

  this.open = false; // true only if the user can write on the socket
  this.timeout = null;

  if (options.connection) {
    this.connection = options.connection;
  }
  else {
    var family = 'IPv4';
    if (net.isIPv6(self.host)) {
      family = 'IPv6';
    }

    var connectionArgs = {
      host: self.host,
      port: self.port,
      family: family
    }

    var tlsOptions = options.ssl || false;
    if (tlsOptions === false) {
      self.connection = net.connect(connectionArgs);
    } else {
      if (helper.isPlainObject(tlsOptions)) {
        // Copy the TLS options in connectionArgs
        helper.loopKeys(tlsOptions, function(tlsOptions, key) {
          connectionArgs[key] = tlsOptions[key];
        });
      }
      self.connection = tls.connect(connectionArgs);
    }
  }

  self.connection.setKeepAlive(true);

  self.timeoutOpen = setTimeout(function() {
    self.connection.end(); // Send a FIN packet
    reject(new Err.ReqlDriverError('Failed to connect to '+self.host+':'+self.port+' in less than '+self.timeoutConnect+'s').setOperational
());
  }, self.timeoutConnect*1000);

  self.connection.on('end', function() {
    self.open = false;
    self.emit('end');
    // We got a FIN packet, so we'll just flush
    self._flush();
  });
  self.connection.on('close', function() {
    // We emit end or close just once
    clearTimeout(self.timeoutOpen)
    clearInterval(self.pingIntervalId);
    self.connection.removeAllListeners();
    self.open = false;
    self.emit('closed');
    // The connection is fully closed, flush (in case 'end' was not triggered)
    self._flush();
  });
  self.connection.setNoDelay();
  self.connection.once('error', function(error) {
    reject(new Err.ReqlDriverError('Failed to connect to '+self.host+':'+self.port+'\nFull error:\n'+JSON.stringify(error)).setOperational
());
  });
  self.connection.on('connect', function() {
    self.connection.removeAllListeners('error');
    self.connection.on('error', function(error) {
      self.emit('error', error);
    });

    var versionBuffer = new Buffer(4)
    versionBuffer.writeUInt32LE(protodef.VersionDummy.Version.V1_0, 0)

    self.randomString = new Buffer(crypto.randomBytes(18)).toString('base64')
    var authBuffer = new Buffer(JSON.stringify({
      protocol_version: PROTOCOL_VERSION,
      authentication_method: AUTHENTIFICATION_METHOD,
      authentication: "n,,n=" + self.user + ",r=" + self.randomString
    }));

    helper.tryCatch(function() {
      self.connection.write(Buffer.concat([versionBuffer, authBuffer, NULL_BUFFER]));
    }, function(err) {
      // The TCP connection is open, but the ReQL connection wasn't established.
      // We can just abort the whole thing
      self.open = false;
      reject(new Err.ReqlD ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.connection.super_"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.</span>super_ ()](#apidoc.element.rethinkdbdash.connection.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.connection.prototype"></a>[module rethinkdbdash.connection.prototype](#apidoc.module.rethinkdbdash.connection.prototype)

#### <a name="apidoc.element.rethinkdbdash.connection.prototype._abort"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_abort ()](#apidoc.element.rethinkdbdash.connection.prototype._abort)
- description and source-code
```javascript
_abort = function () {
  this.state = -1;
  this.removeAllListeners();
  this.close();
}
```
- example usage
```shell
...
      for(var i=0; i<self.buffer.length; i++) {
if (self.buffer[i] === 0) {
  var messageServerStr = self.buffer.slice(0, i).toString();
  self.buffer = self.buffer.slice(i+1); // +1 to remove the null byte
  try {
    var messageServer = JSON.parse(messageServerStr);
  } catch(error) {
    self._abort();
    reject(new Err.ReqlDriverError('Could not parse the message sent by the server : \''+messageServerStr+'\'').setOperational());
    return;
  }
  if (messageServer.success !== true) {
    self._abort();
    reject(new Err.ReqlDriverError('Error '+messageServer.error_code+':'+messageServer.error).setOperational());
    return;
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype._checkProtocolVersion"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_checkProtocolVersion (messageServer, reject)](#apidoc.element.rethinkdbdash.connection.prototype._checkProtocolVersion)
- description and source-code
```javascript
_checkProtocolVersion = function (messageServer, reject) {
  // Expect max_protocol_version, min_protocol_version, server_version, success
  var minVersion = messageServer.min_protocol_version
  var maxVersion = messageServer.max_protocol_version

  if (minVersion > PROTOCOL_VERSION || maxVersion < PROTOCOL_VERSION) {
    this._abort();
    reject(new Err.ReqlDriverError('Unsupported protocol version: '+PROTOCOL_VERSION+', expected between '+minVersion+' and '+ maxVersion
).setOperational());
  }
  this.state = 1;
}
```
- example usage
```shell
...
  if (messageServer.success !== true) {
    self._abort();
    reject(new Err.ReqlDriverError('Error '+messageServer.error_code+':'+messageServer.error).setOperational());
    return;
  }

  if (self.state === 0) {
    self._checkProtocolVersion(messageServer, reject);
  } else if (self.state === 1) {
    // Compute salt and send the proof
    self._computeSaltedPassword(messageServer, reject);
  } else if (self.state === 2) {
    self._compareDigest(messageServer, resolve, reject);
  }
}
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype._compareDigest"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_compareDigest (messageServer, resolve, reject)](#apidoc.element.rethinkdbdash.connection.prototype._compareDigest)
- description and source-code
```javascript
_compareDigest = function (messageServer, resolve, reject) {
  var self = this;
  var firstEquals = messageServer.authentication.indexOf('=')
  var serverSignatureValue = messageServer.authentication.slice(firstEquals+1)

  if (!helper.compareDigest(serverSignatureValue, self.serverSignature.toString("base64"))) {
    reject(new Err.ReqlDriverError('Invalid server signature').setOperational());
  }

  self.state = 4
  self.connection.removeAllListeners('error');
  self.open = true;
  self.connection.on('error', function(e) {
    self.open = false;
  });
  clearTimeout(self.timeoutOpen)
  resolve(self);
  if (self.pingInterval > 0) {
    self.pingIntervalId = setInterval(function() {
      self.pendingPing = true;
      self.r.error(PING_VALUE).run(self).error(function(error) {
        self.pendingPing = false;
        if (error.message !== PING_VALUE) {
          self.emit('error', new Err.ReqlDriverError(
                'Could not ping the connection').setOperational());
          self.open = false;
          self.connection.end();
        } else {
        }
      });
    }, self.pingInterval*1000);
  }
}
```
- example usage
```shell
...

      if (self.state === 0) {
        self._checkProtocolVersion(messageServer, reject);
      } else if (self.state === 1) {
        // Compute salt and send the proof
        self._computeSaltedPassword(messageServer, reject);
      } else if (self.state === 2) {
        self._compareDigest(messageServer, resolve, reject);
      }
    }
  }
}
else {
  while(self.buffer.length >= 12) {
    var token = self.buffer.readUInt32LE(0) + 0x100000000 * self.buffer.readUInt32LE(4);
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype._computeSaltedPassword"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_computeSaltedPassword (messageServer, reject)](#apidoc.element.rethinkdbdash.connection.prototype._computeSaltedPassword)
- description and source-code
```javascript
_computeSaltedPassword = function (messageServer, reject) {
  var self = this;
  var authentication = helper.splitCommaEqual(messageServer.authentication);

  var randomNonce = authentication.r
  var salt = new Buffer(authentication.s, 'base64')
  var iterations = parseInt(authentication.i)

  if (randomNonce.substr(0, self.randomString.length) !== self.randomString) {
    self._abort();
    reject(new Err.ReqlDriverError('Invalid nonce from server').setOperational());
  }

  // The salt is constant, so we can cache the salted password.
  var cacheKey = self.password.toString("base64")+','+salt.toString("base64")+','+iterations;
  if (CACHE_PBKDF2.hasOwnProperty(cacheKey)) {
    helper.tryCatch(function() {
      self._sendProof(messageServer.authentication, randomNonce, CACHE_PBKDF2[cacheKey]);
    }, function(err) {
      // The TCP connection is open, but the ReQL connection wasn't established.
      // We can just abort the whole thing
      self.open = false;
      reject(new Err.ReqlDriverError('Failed to perform handshake with '+self.host+':'+self.port).setOperational());
    });
  } else {
    crypto.pbkdf2(self.password, salt, iterations, KEY_LENGTH, "sha256", function(error, saltedPassword) {
      if (error != null) {
        self._abort();
        reject(new Err.ReqlDriverError('Could not derive the key. Error:' + error.toString()).setOperational());
      }
      CACHE_PBKDF2[cacheKey] = saltedPassword;
      helper.tryCatch(function() {
        self._sendProof(messageServer.authentication, randomNonce, saltedPassword);
      }, function(err) {
        // The TCP connection is open, but the ReQL connection wasn't established.
        // We can just abort the whole thing
        self.open = false;
        reject(new Err.ReqlDriverError('Failed to perform handshake with '+self.host+':'+self.port).setOperational());
      });
    })
  }
}
```
- example usage
```shell
...
        return;
      }

      if (self.state === 0) {
        self._checkProtocolVersion(messageServer, reject);
      } else if (self.state === 1) {
        // Compute salt and send the proof
        self._computeSaltedPassword(messageServer, reject);
      } else if (self.state === 2) {
        self._compareDigest(messageServer, resolve, reject);
      }
    }
  }
}
else {
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype._continue"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_continue (token, resolve, reject)](#apidoc.element.rethinkdbdash.connection.prototype._continue)
- description and source-code
```javascript
_continue = function (token, resolve, reject) {
  var query = [protodef.Query.QueryType.CONTINUE];
  this._send(query, token, resolve, reject);
}
```
- example usage
```shell
...
}

Cursor.prototype._fetch = function() {
var self = this;
this._fetching = true;

var p = new Promise(function(resolve, reject) {
  self.connection._continue(self.token, resolve, reject);
}).then(function(response) {
  self._push(response);
  return null;
}).error(function(error) {
  self._fetching = false;
  self._canFetch = false;
  self._pushError(error);
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype._end"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_end (token, resolve, reject)](#apidoc.element.rethinkdbdash.connection.prototype._end)
- description and source-code
```javascript
_end = function (token, resolve, reject) {
  var query = [protodef.Query.QueryType.STOP];
  this._send(query, token, resolve, reject, undefined, undefined, true);
}
```
- example usage
```shell
...
    var endCallback = function() {
      if (self._eventEmitter && (self._emittedEnd === false)) {
        self._emittedEnd = true;
        self._eventEmitter.emit('end');
      }
      resolve();
    }
    self.connection._end(self.token, endCallback, reject);
  }
}).nodeify(callback);
return self._closingPromise;
}
Cursor.prototype._each = function(callback, onFinish) {
if (this._closed === true) {
  return callback(new Err.ReqlDriverError('You cannot retrieve data from a cursor that is closed').setOperational());
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype._flush"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_flush ()](#apidoc.element.rethinkdbdash.connection.prototype._flush)
- description and source-code
```javascript
_flush = function () {
  helper.loopKeys(this.metadata, function(metadata, key) {
    if (typeof metadata[key].reject === 'function') {
      metadata[key].reject(new Err.ReqlServerError(
            'The connection was closed before the query could be completed.',
            metadata[key].query));
    }
    if (typeof metadata[key].endReject === 'function') {
      metadata[key].endReject(new Err.ReqlServerError(
            'The connection was closed before the query could be completed.',
            metadata[key].query));
    }
  });
  this.metadata = {};
}
```
- example usage
```shell
...
  reject(new Err.ReqlDriverError('Failed to connect to '+self.host+':'+self.port+' in less than '+self.timeoutConnect+'s').setOperational
());
}, self.timeoutConnect*1000);

self.connection.on('end', function() {
  self.open = false;
  self.emit('end');
  // We got a FIN packet, so we'll just flush
  self._flush();
});
self.connection.on('close', function() {
  // We emit end or close just once
  clearTimeout(self.timeoutOpen)
  clearInterval(self.pingIntervalId);
  self.connection.removeAllListeners();
  self.open = false;
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype._getToken"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_getToken ()](#apidoc.element.rethinkdbdash.connection.prototype._getToken)
- description and source-code
```javascript
_getToken = function () {
  return this.token++;
}
```
- example usage
```shell
...
  this.db = db;
}

Connection.prototype.server = function(callback) {
  var self = this;
  return new Promise(function(resolve, reject) {
    var query = [protodef.Query.QueryType.SERVER_INFO];
    self._send(query, self._getToken(), resolve, reject, undefined, undefined, true);
  }).nodeify(callback);
}

// Return the next token and update it.
Connection.prototype._getToken = function() {
  return this.token++;
}
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype._isConnection"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_isConnection ()](#apidoc.element.rethinkdbdash.connection.prototype._isConnection)
- description and source-code
```javascript
_isConnection = function () {
  return true;
}
```
- example usage
```shell
...
var self = this;

if (self._error != null) {
  var error = new Error.ReqlRuntimeError(self._error, self._query, {b: self._frames});
  return Promise.reject(error);
}

if (helper.isPlainObject(connection) && (typeof connection._isConnection === 'function') && (connection._isConnection() === true
)) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  else {
    if (!helper.isPlainObject(options)) options = {};
  }
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype._isOpen"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_isOpen ()](#apidoc.element.rethinkdbdash.connection.prototype._isOpen)
- description and source-code
```javascript
_isOpen = function () {
  return this.open;
}
```
- example usage
```shell
...
    }

    clearTimeout(connection.timeout);
    self._decreaseNumConnections();
    self._expandBuffer();
  });
  connection.on('release', function() {
    if (this._isOpen()) self.putConnection(this);
  });
  self.putConnection(connection);
  return null;
}).error(function(error) {
  // We failed to create a connection, we are now going to create connections one by one
  self._openingConnections--;
  self._decreaseNumConnections();
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype._processResponse"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_processResponse (response, token)](#apidoc.element.rethinkdbdash.connection.prototype._processResponse)
- description and source-code
```javascript
_processResponse = function (response, token) {
  //console.log('Connection.prototype._processResponse: '+token);
  //console.log(JSON.stringify(response, null, 2));
  var self = this;

  var type = response.t;
  var result;
  var cursor;
  var stream;
  var currentResolve, currentReject;
  var datum;
  var options;

  if (type === responseTypes.COMPILE_ERROR) {
    self.emit('release');
    if (typeof self.metadata[token].reject === 'function') {
      self.metadata[token].reject(new Err.ReqlCompileError(helper.makeAtom(response), self.metadata[token].query, response));
    }

    delete self.metadata[token]
  }
  else if (type === responseTypes.CLIENT_ERROR) {
    self.emit('release');

    if (typeof self.metadata[token].reject === 'function') {
      currentResolve = self.metadata[token].resolve;
      currentReject = self.metadata[token].reject;
      self.metadata[token].removeCallbacks();
      currentReject(new Err.ReqlClientError(helper.makeAtom(response), self.metadata[token].query, response));
      if (typeof self.metadata[token].endReject !== 'function') {
        // No pending STOP query, we can delete
        delete self.metadata[token]
      }
    }
    else if (typeof self.metadata[token].endResolve === 'function') {
      currentResolve = self.metadata[token].endResolve;
      currentReject = self.metadata[token].endReject;
      self.metadata[token].removeEndCallbacks();
      currentReject(new Err.ReqlClientError(helper.makeAtom(response), self.metadata[token].query, response));
      delete self.metadata[token]
    }
    else if (token === -1) { // This should not happen now since 1.13 took the token out of the query
      var error = new Err.ReqlClientError(helper.makeAtom(response)+'\nClosing all outstanding queries...');
      self.emit('error', error);
      // We don't want a function to yield forever, so we just reject everything
      helper.loopKeys(self.rejectMap, function(rejectMap, key) {
        rejectMap[key](error);
      });
      self.close();
      delete self.metadata[token]
    }
  }
  else if (type === responseTypes.RUNTIME_ERROR) {
    var errorValue = helper.makeAtom(response);
    var error;
    // We don't want to release a connection if we just pinged it.
    if (self.pendingPing === false || (errorValue !== PING_VALUE)) {
      self.emit('release');
      error = new Err.ReqlRuntimeError(errorValue, self.metadata[token].query, response);
    } else {
      error = new Err.ReqlRuntimeError(errorValue);
    }

    if (typeof self.metadata[token].reject === 'function') {
      currentResolve = self.metadata[token].resolve;
      currentReject = self.metadata[token].reject;
      self.metadata[token].removeCallbacks();
      error.setName(response.e);
      currentReject(error);
      if (typeof self.metadata[token].endReject !== 'function') {
        // No pending STOP query, we can delete
        delete self.metadata[token]
      }
    }
    else if (typeof self.metadata[token].endResolve === 'function') {
      currentResolve = self.metadata[token].endResolve;
      currentReject = self.metadata[token].endReject;
      self.metadata[token].removeEndCallbacks();
      delete self.metadata[token]
    }
  }
  else if (type === responseTypes.SUCCESS_ATOM) {
    self.emit('release');
    // self.metadata[token].resolve is always a function
    datum = helper.makeAtom(response, self.metadata[token].options);

    if ((Array.isArray(datum)) &&
        ((self.metadata[token].options.cursor === true) || ((self.metadata[token].options.cursor === undefined) && (self.r._options
.cursor === true)))) {
      cursor = new Cursor(self, token, self.metadata[token].options, 'cursor');
      if (self.metadata[token].options.profile === true) {
        self.metadata[token].resolve({
          profile: response.p,
          result: cursor
        });
      }
      else {
        self.metadata[token].resolve(cursor);
      }

      cursor._push({done: true, response: { r: datum }});
    }
    else if ((Array.isArray(datum)) &&
        ((self.metadata[token].options.stream === true || self.r._options.stream === true) ...
```
- example usage
```shell
...
      var responseLength = self.buffer.readUInt32LE(8);

      if (self.buffer.length < 12+responseLength) break;

      var responseBuffer = self.buffer.slice(12, 12+responseLength);
      var response = JSON.parse(responseBuffer);

      self._processResponse(response, token);

      self.buffer = self.buffer.slice(12+responseLength);
    }
  }
});

self.connection.on('timeout', function(buffer) {
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype._send"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_send (query, token, resolve, reject, originalQuery, options, end)](#apidoc.element.rethinkdbdash.connection.prototype._send)
- description and source-code
```javascript
_send = function (query, token, resolve, reject, originalQuery, options, end) {
  //console.log('Connection.prototype._send: '+token);
  //console.log(JSON.stringify(query, null, 2));

  var self = this;
  if (self.open === false) {
    var err = new Err.ReqlDriverError('The connection was closed by the other party');
    err.setOperational();
    reject(err);
    return;
  }

  var queryStr = JSON.stringify(query);
  var querySize = Buffer.byteLength(queryStr);

  var buffer = new Buffer(8+4+querySize);
  buffer.writeUInt32LE(token & 0xFFFFFFFF, 0)
  buffer.writeUInt32LE(Math.floor(token / 0xFFFFFFFF), 4)

  buffer.writeUInt32LE(querySize, 8);

  buffer.write(queryStr, 12);

  // noreply instead of noReply because the otpions are translated for the server
  if ((!helper.isPlainObject(options)) || (options.noreply != true)) {
    if (!self.metadata[token]) {
      self.metadata[token] = new Metadata(resolve, reject, originalQuery, options);
    }
    else if (end === true) {
      self.metadata[token].setEnd(resolve, reject);
    }
    else {
      self.metadata[token].setCallbacks(resolve, reject);
    }
  }
  else {
    if (typeof resolve === 'function') resolve();
    this.emit('release');
  }

  // This will emit an error if the connection is closed
  helper.tryCatch(function() {
    self.connection.write(buffer);
  }, function(err) {
    self.metadata[token].reject(err);
    delete self.metadata[token]
  });

}
```
- example usage
```shell
...
    delete self.metadata[token]
  });

};

Connection.prototype._continue = function(token, resolve, reject) {
  var query = [protodef.Query.QueryType.CONTINUE];
  this._send(query, token, resolve, reject);
}
Connection.prototype._end = function(token, resolve, reject) {
  var query = [protodef.Query.QueryType.STOP];
  this._send(query, token, resolve, reject, undefined, undefined, true);
}
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype._sendProof"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>_sendProof (authentication, randomNonce, saltedPassword)](#apidoc.element.rethinkdbdash.connection.prototype._sendProof)
- description and source-code
```javascript
_sendProof = function (authentication, randomNonce, saltedPassword) {
  var clientFinalMessageWithoutProof = "c=biws,r=" + randomNonce;
  var clientKey = crypto.createHmac("sha256", saltedPassword).update("Client Key").digest()
  var storedKey = crypto.createHash("sha256").update(clientKey).digest()

  var authMessage =
      "n=" + this.user + ",r=" + this.randomString + "," +
      authentication + "," +
      clientFinalMessageWithoutProof

  var clientSignature = crypto.createHmac("sha256", storedKey).update(authMessage).digest()
  var clientProof = helper.xorBuffer(clientKey, clientSignature)

  var serverKey = crypto.createHmac("sha256", saltedPassword).update("Server Key").digest()
  this.serverSignature = crypto.createHmac("sha256", serverKey).update(authMessage).digest()

  this.state = 2
  var message = JSON.stringify({
    authentication: clientFinalMessageWithoutProof + ",p=" + clientProof.toString("base64")
  })
  this.connection.write(Buffer.concat([new Buffer(message.toString()), NULL_BUFFER]))
}
```
- example usage
```shell
...
  reject(new Err.ReqlDriverError('Invalid nonce from server').setOperational());
}

// The salt is constant, so we can cache the salted password.
var cacheKey = self.password.toString("base64")+','+salt.toString("base64")+','+iterations;
if (CACHE_PBKDF2.hasOwnProperty(cacheKey)) {
  helper.tryCatch(function() {
    self._sendProof(messageServer.authentication, randomNonce, CACHE_PBKDF2[cacheKey]);
  }, function(err) {
    // The TCP connection is open, but the ReQL connection wasn't established.
    // We can just abort the whole thing
    self.open = false;
    reject(new Err.ReqlDriverError('Failed to perform handshake with '+self.host+':'+self.port).setOperational());
  });
} else {
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype.close"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>close (options, callback)](#apidoc.element.rethinkdbdash.connection.prototype.close)
- description and source-code
```javascript
close = function (options, callback) {
  if (typeof options === 'function') {
    callback = options;
    options = {};
  }
  var self = this;

  var p = new Promise(function(resolve, reject) {
    if (!helper.isPlainObject(options)) options = {};
    if (options.noreplyWait === true) {
      self.noreplyWait().then(function(r) {
        self.open = false;
        self.connection.end()
        resolve(r);
      }).error(function(e) {
        reject(e)
      });
    }
    else{
      self.open = false;
      self.connection.end();
      resolve();
    }
  }).nodeify(callback);
  return p;
}
```
- example usage
```shell
...
2. Remove everything related to a connection:

'''js
r.connect({host: ..., port: ...}).then(function(connection) {
  connection.on('error', handleError);
  query.run(connection).then(function(result) {
    // console.log(result);
    connection.close();
  });
});
'''

Becomes:

'''js
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype.noReplyWait"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>noReplyWait ()](#apidoc.element.rethinkdbdash.connection.prototype.noReplyWait)
- description and source-code
```javascript
noReplyWait = function () {
  throw new Err.ReqlDriverError('Did you mean to use 'noreplyWait' instead of 'noReplyWait'?')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype.noreplyWait"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>noreplyWait (callback)](#apidoc.element.rethinkdbdash.connection.prototype.noreplyWait)
- description and source-code
```javascript
noreplyWait = function (callback) {
  var self = this;
  var token = self._getToken();

  var p = new Promise(function(resolve, reject) {
    var query = [protodef.Query.QueryType.NOREPLY_WAIT];

    self._send(query, token, resolve, reject);
  }).nodeify(callback);
  return p;
}
```
- example usage
```shell
...
  options = {};
}
var self = this;

var p = new Promise(function(resolve, reject) {
  if (!helper.isPlainObject(options)) options = {};
  if (options.noreplyWait === true) {
    self.noreplyWait().then(function(r) {
      self.open = false;
      self.connection.end()
      resolve(r);
    }).error(function(e) {
      reject(e)
    });
  }
...
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype.reconnect"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>reconnect (options, callback)](#apidoc.element.rethinkdbdash.connection.prototype.reconnect)
- description and source-code
```javascript
reconnect = function (options, callback) {
  var self = this;

  if (typeof options === 'function') {
    callback = options;
    options = {};
  }

  if (!helper.isPlainObject(options)) options = {};

  if (options.noreplyWait === true) {
    var p = new Promise(function(resolve, reject) {
      self.close(options).then(function() {
        self.r.connect({
          host: self.host,
          port: self.port,
          authKey: self.authKey,
          db: self.db
        }).then(function(c) {
          resolve(c);
        }).error(function(e) {
          reject(e);
        });
      }).error(function(e) {
        reject(e)
      })
    }).nodeify(callback);
  }
  else {
    return self.r.connect({
      host: self.host,
      port: self.port,
      authKey: self.authKey,
      db: self.db
    }, callback);
  }

  return p;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype.server"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>server (callback)](#apidoc.element.rethinkdbdash.connection.prototype.server)
- description and source-code
```javascript
server = function (callback) {
  var self = this;
  return new Promise(function(resolve, reject) {
    var query = [protodef.Query.QueryType.SERVER_INFO];
    self._send(query, self._getToken(), resolve, reject, undefined, undefined, true);
  }).nodeify(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.connection.prototype.use"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.connection.prototype.</span>use (db)](#apidoc.element.rethinkdbdash.connection.prototype.use)
- description and source-code
```javascript
use = function (db) {
  if (typeof db !== 'string') throw new Err.ReqlDriverError('First argument of 'use' must be a string')
  this.db = db;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.cursor"></a>[module rethinkdbdash.cursor](#apidoc.module.rethinkdbdash.cursor)

#### <a name="apidoc.element.rethinkdbdash.cursor.cursor"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>cursor (connection, token, options, type)](#apidoc.element.rethinkdbdash.cursor.cursor)
- description and source-code
```javascript
function Cursor(connection, token, options, type) {
  this.connection = connection;
  this.token = token;

  this._stackSize = 0; // Estimation of our call stack.
  this._index = 0; // Position in this._data[0]
  this._data = []; // Array of non empty arrays
  this._fetching = false; // Are we fetching data
  this._canFetch = true; // Can we fetch more data?
  this._pendingPromises = []; // Pending promises' resolve/reject
  this.options = options || {};
  this._closed = false;
  this._closingPromise = null; // Promise returned by close
  this._type = type;
  this._setIncludesStates = false;
  if ((type === 'feed') || (type === 'atomFeed')) {
    this.toArray = _unsupportedToArray;
  }
  this._emittedEnd = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.cursor.prototype"></a>[module rethinkdbdash.cursor.prototype](#apidoc.module.rethinkdbdash.cursor.prototype)

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype._done"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_done ()](#apidoc.element.rethinkdbdash.cursor.prototype._done)
- description and source-code
```javascript
_done = function () {
  this._canFetch = false;
  if (this._eventEmitter) {
    this._eventEmitter.emit('end');
  }
}
```
- example usage
```shell
...
  self._canFetch = false;
  self._pushError(error);
})
}

Cursor.prototype._push = function(data) {
var couldfetch = this._canFetch;
if (data.done) this._done();
var response = data.response;
this._fetching = false;
// If the cursor was closed, we ignore all following response
if ((response.r.length > 0) && (couldfetch === true)) {
  this._data.push(helper.makeSequence(response, this.options));
}
// this._fetching = false
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype._each"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_each (callback, onFinish)](#apidoc.element.rethinkdbdash.cursor.prototype._each)
- description and source-code
```javascript
_each = function (callback, onFinish) {
  if (this._closed === true) {
    return callback(new Err.ReqlDriverError('You cannot retrieve data from a cursor that is closed').setOperational());
  }
  var self = this;

  var reject = function(err) {
    if (err.message === 'No more rows in the '+self._type.toLowerCase()+'.') {
      if (typeof onFinish === 'function') {
        onFinish();
      }
    }
    else {
      callback(err);
    }
    return null;
  }
  var resolve = function(data) {
    self._stackSize++;
    var keepGoing = callback(null, data);
    if (keepGoing === false) {
      if (typeof onFinish === 'function') {
        onFinish();
      }
    }
    else {
      if (self._closed === false) {
        if (self._stackSize <= MAX_CALL_STACK) {
          self._next().then(resolve).error(function(error) {
            if ((error.message !== 'You cannot retrieve data from a cursor that is closed.') &&
                (error.message.match(/You cannot call 'next' on a closed/) === null)) {
              reject(error);
            }
          });
        }
        else {
          setTimeout(function() {
            self._stackSize = 0;
            self._next().then(resolve).error(function(error) {
              if ((error.message !== 'You cannot retrieve data from a cursor that is closed.') &&
                  (error.message.match(/You cannot call 'next' on a closed/) === null)) {
                reject(error);
              }
            });
          }, 0);
        }
      }
    }
    return null;
  }

  self._next().then(resolve).error(function(error) {
    // We can silence error when the cursor is closed as this
    if ((error.message !== 'You cannot retrieve data from a cursor that is closed.') &&
        (error.message.match(/You cannot call 'next' on a closed/) === null)) {
      reject(error);
    }
  });
  return null;
}
```
- example usage
```shell
...
throw new Error('The 'hasNext' command has been removed in 1.13, please use 'next'.')
}
Cursor.prototype.toArray = function(callback) {
var self = this;
var p = new Promise(function(resolve, reject) {
  var result = [];
  var i =0;
  self._each(function(err, data) {
    if (err) {
      reject(err);
    }
    else {
      result.push(data);
    }
  }, function() {
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype._eachAsync"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_eachAsync (callback)](#apidoc.element.rethinkdbdash.cursor.prototype._eachAsync)
- description and source-code
```javascript
_eachAsync = function (callback) {
  var self = this;
  return new Promise(function(resolve, reject) {
    self._eachAsyncInternal(callback, resolve, reject)
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype._eachAsyncInternal"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_eachAsyncInternal (callback, finalResolve, finalReject)](#apidoc.element.rethinkdbdash.cursor.prototype._eachAsyncInternal)
- description and source-code
```javascript
_eachAsyncInternal = function (callback, finalResolve, finalReject) {
  if (this._closed === true) {
    finalReject(new Err.ReqlDriverError('You cannot retrieve data from a cursor that is closed').setOperational());
    return;
  }
  var self = this;

  var nextCb = function() {
    self._stackSize++;
    self._next().then(function(row) {
      if (self._stackSize <= MAX_CALL_STACK) {
        if (callback.length <= 1) {
          Promise.resolve(callback(row)).then(nextCb)
          return null;
        }
        else {
          new Promise(function(resolve, reject) {
            return callback(row, resolve)
          }).then(nextCb);
          return null;
        }
      }
      else {
        new Promise(function(resolve, reject) {
          setTimeout(function() {
            self._stackSize = 0;
            if (callback.length <= 1) {
              Promise.resolve(callback(row)).then(resolve).catch(reject);
            }
            else {
              new Promise(function(resolve, reject) {
                return callback(row, resolve)
              }).then(resolve).catch(reject);
              return null;
            }
          }, 0)
        }).then(nextCb);
        return null;
      }
    }).error(function(error) {
      if ((error.message === 'No more rows in the '+self._type.toLowerCase()+'.') ||
          (error.message === 'You cannot retrieve data from a cursor that is closed.') ||
          (error.message.match(/You cannot call 'next' on a closed/) !== null)) {
        return finalResolve();
      }
      return finalReject(Err.setOperational(error));
    });
  }
  nextCb();
}
```
- example usage
```shell
...
  }
});
return null;
}
Cursor.prototype._eachAsync = function(callback) {
var self = this;
return new Promise(function(resolve, reject) {
  self._eachAsyncInternal(callback, resolve, reject)
});
}
Cursor.prototype._eachAsyncInternal = function(callback, finalResolve, finalReject) {
if (this._closed === true) {
  finalReject(new Err.ReqlDriverError('You cannot retrieve data from a cursor that is closed').setOperational());
  return;
}
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype._eachCb"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_eachCb (err, data)](#apidoc.element.rethinkdbdash.cursor.prototype._eachCb)
- description and source-code
```javascript
_eachCb = function (err, data) {
  // We should silent things if the cursor/feed is closed
  if (this._closed === false) {
    if (err) {
      this._eventEmitter.emit('error', err);
    }
    else {
      this._eventEmitter.emit('data', data);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype._fetch"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_fetch ()](#apidoc.element.rethinkdbdash.cursor.prototype._fetch)
- description and source-code
```javascript
_fetch = function () {
  var self = this;
  this._fetching = true;

  var p = new Promise(function(resolve, reject) {
    self.connection._continue(self.token, resolve, reject);
  }).then(function(response) {
    self._push(response);
    return null;
  }).error(function(error) {
    self._fetching = false;
    self._canFetch = false;
    self._pushError(error);
  })
}
```
- example usage
```shell
...
    if (self._data[0].length === self._index) {
      self._index = 0;
      self._data.shift();
      if ((self._data.length === 1)
        && (self._canFetch === true)
        && (self._closed === false)
        && (self._fetching === false)) {
          self._fetch();
      }
    }
    return Promise.resolve(result).nodeify(callback);
  }
}
else {
  return new Promise(function(resolve, reject) {
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype._flush"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_flush ()](#apidoc.element.rethinkdbdash.cursor.prototype._flush)
- description and source-code
```javascript
_flush = function () {
  while ((this._pendingPromises.length > 0) && ((this._data.length > 0) || ((this._fetching === false) && (this._canFetch === false
)))) {
    var fullfiller = this._pendingPromises.shift();
    var resolve = fullfiller.resolve;
    var reject = fullfiller.reject;

    if (this._data.length > 0) {
      var result = this._data[0][this._index++];
      if (result instanceof Error) {
        reject(result);
      }
      else {
        resolve(result);
      }

      if (this._data[0].length === this._index) {
        this._index = 0;
        this._data.shift();
        if ((this._data.length <= 1)
          && (this._canFetch === true)
          && (this._closed === false)
          && (this._fetching === false)) {
            this._fetch();
        }
      }
    }
    else {
      reject(new Err.ReqlDriverError('No more rows in the '+this._type.toLowerCase()).setOperational())
    }
  }
}
```
- example usage
```shell
...
  reject(new Err.ReqlDriverError('Failed to connect to '+self.host+':'+self.port+' in less than '+self.timeoutConnect+'s').setOperational
());
}, self.timeoutConnect*1000);

self.connection.on('end', function() {
  self.open = false;
  self.emit('end');
  // We got a FIN packet, so we'll just flush
  self._flush();
});
self.connection.on('close', function() {
  // We emit end or close just once
  clearTimeout(self.timeoutOpen)
  clearInterval(self.pingIntervalId);
  self.connection.removeAllListeners();
  self.open = false;
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype._makeEmitter"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_makeEmitter ()](#apidoc.element.rethinkdbdash.cursor.prototype._makeEmitter)
- description and source-code
```javascript
_makeEmitter = function () {
  this.next = function() {
    throw new Err.ReqlDriverError('You cannot call 'next' once you have bound listeners on the '+this._type)
  }
  this.each = function() {
    throw new Err.ReqlDriverError('You cannot call 'each' once you have bound listeners on the '+this._type)
  }
  this.eachAsync = function() {
    throw new Err.ReqlDriverError('You cannot call 'eachAsync' once you have bound listeners on the '+this._type)
  }
  this.toArray = function() {
    throw new Err.ReqlDriverError('You cannot call 'toArray' once you have bound listeners on the '+this._type)
  }
  this._eventEmitter = new EventEmitter();
}
```
- example usage
```shell
...

for(var i=0; i<methods.length; i++) {
(function(n) {
  var method = methods[n];
  Cursor.prototype[method] = function() {
    var self = this;
    if (self._eventEmitter == null) {
      self._makeEmitter();
      setImmediate(function() {
        self._each(self._eachCb.bind(self), function() {
          if (self._emittedEnd === false) {
            self._emittedEnd = true;
            self._eventEmitter.emit('end');
          }
        });
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype._next"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_next (callback)](#apidoc.element.rethinkdbdash.cursor.prototype._next)
- description and source-code
```javascript
_next = function (callback) {
  var self = this;
  if (self._closed === true) {
    return Promise.reject(new Err.ReqlDriverError(
      'You cannot call 'next' on a closed '+self._type).setOperational()
    ).nodeify(callback);
  }
  else if ((self._data.length === 0) && (self._canFetch === false)) {
    return Promise.reject(new Err.ReqlDriverError(
      'No more rows in the '+self._type.toLowerCase()).setOperational()
    ).nodeify(callback);
  }
  else {
    if ((self._data.length > 0) && (self._data[0].length > self._index)) {
      var result = self._data[0][self._index++];
      if (result instanceof Error) {
        return Promise.reject(result).nodeify(callback);
      }
      else {
        // This could be possible if we get back batch with just one document?
        if (self._data[0].length === self._index) {
          self._index = 0;
          self._data.shift();
          if ((self._data.length === 1)
            && (self._canFetch === true)
            && (self._closed === false)
            && (self._fetching === false)) {
              self._fetch();
          }
        }
        return Promise.resolve(result).nodeify(callback);
      }
    }
    else {
      return new Promise(function(resolve, reject) {
        self._pendingPromises.push({resolve: resolve, reject: reject});
      }).nodeify(callback);
    }
  }
}
```
- example usage
```shell
...
  if (typeof onFinish === 'function') {
    onFinish();
  }
}
else {
  if (self._closed === false) {
    if (self._stackSize <= MAX_CALL_STACK) {
      self._next().then(resolve).error(function(error) {
        if ((error.message !== 'You cannot retrieve data from a cursor that is closed.') &&
            (error.message.match(/You cannot call 'next' on a closed/) === null)) {
          reject(error);
        }
      });
    }
    else {
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype._push"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_push (data)](#apidoc.element.rethinkdbdash.cursor.prototype._push)
- description and source-code
```javascript
_push = function (data) {
  var couldfetch = this._canFetch;
  if (data.done) this._done();
  var response = data.response;
  this._fetching = false;
  // If the cursor was closed, we ignore all following response
  if ((response.r.length > 0) && (couldfetch === true)) {
    this._data.push(helper.makeSequence(response, this.options));
  }
  // this._fetching = false
  if ((this._closed === false) && (this._canFetch) && (this._data.length <= 1)) this._fetch();
  this._flush();
}
```
- example usage
```shell
...
      result: cursor
    });
  }
  else {
    self.metadata[token].resolve(cursor);
  }

  cursor._push({done: true, response: { r: datum }});
}
else if ((Array.isArray(datum)) &&
    ((self.metadata[token].options.stream === true || self.r._options.stream === true))) {
  cursor = new Cursor(self, token, self.metadata[token].options, 'cursor');
  stream = new ReadableStream({}, cursor);
  if (self.metadata[token].options.profile === true) {
    self.metadata[token].resolve({
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype._pushError"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_pushError (error)](#apidoc.element.rethinkdbdash.cursor.prototype._pushError)
- description and source-code
```javascript
_pushError = function (error) {
  this._data.push([error]);
  this._flush();
}
```
- example usage
```shell
...
  self.connection._continue(self.token, resolve, reject);
}).then(function(response) {
  self._push(response);
  return null;
}).error(function(error) {
  self._fetching = false;
  self._canFetch = false;
  self._pushError(error);
})
}

Cursor.prototype._push = function(data) {
var couldfetch = this._canFetch;
if (data.done) this._done();
var response = data.response;
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype._set"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_set (ar)](#apidoc.element.rethinkdbdash.cursor.prototype._set)
- description and source-code
```javascript
_set = function (ar) {
  this._fetching = false;
  this._canFetch = false;
  if (ar.length > 0) {
    this._data.push(ar);
  }
  this._flush();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype._unsupportedToArray"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>_unsupportedToArray ()](#apidoc.element.rethinkdbdash.cursor.prototype._unsupportedToArray)
- description and source-code
```javascript
_unsupportedToArray = function () {
  throw new Error('The 'toArray' method is not available on feeds.')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.addListener"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>addListener ()](#apidoc.element.rethinkdbdash.cursor.prototype.addListener)
- description and source-code
```javascript
addListener = function () {
  var self = this;
  if (self._eventEmitter == null) {
    self._makeEmitter();
    setImmediate(function() {
      self._each(self._eachCb.bind(self), function() {
        if (self._emittedEnd === false) {
          self._emittedEnd = true;
          self._eventEmitter.emit('end');
        }
      });
    });
  }
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  self._eventEmitter[method].apply(self._eventEmitter, _args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.close"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>close (callback)](#apidoc.element.rethinkdbdash.cursor.prototype.close)
- description and source-code
```javascript
close = function (callback) {
  var self = this;
  if (self._closed === true) {
    return self._closingPromise.nodeify(callback);
  }
  self._closed = true;

  self._closingPromise = new Promise(function(resolve, reject) {
    if ((self._canFetch === false) && (self._fetching === false)) {
      resolve()
    }
    else { // since v0_4 (RethinkDB 2.0) we can (must) force a STOP request even if a CONTINUE query is pending
      var endCallback = function() {
        if (self._eventEmitter && (self._emittedEnd === false)) {
          self._emittedEnd = true;
          self._eventEmitter.emit('end');
        }
        resolve();
      }
      self.connection._end(self.token, endCallback, reject);
    }
  }).nodeify(callback);
  return self._closingPromise;
}
```
- example usage
```shell
...
2. Remove everything related to a connection:

'''js
r.connect({host: ..., port: ...}).then(function(connection) {
  connection.on('error', handleError);
  query.run(connection).then(function(result) {
    // console.log(result);
    connection.close();
  });
});
'''

Becomes:

'''js
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.each"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>each (callback, onFinish)](#apidoc.element.rethinkdbdash.cursor.prototype.each)
- description and source-code
```javascript
each = function (callback, onFinish) {
  if (this._closed === true) {
    return callback(new Err.ReqlDriverError('You cannot retrieve data from a cursor that is closed').setOperational());
  }
  var self = this;

  var reject = function(err) {
    if (err.message === 'No more rows in the '+self._type.toLowerCase()+'.') {
      if (typeof onFinish === 'function') {
        onFinish();
      }
    }
    else {
      callback(err);
    }
    return null;
  }
  var resolve = function(data) {
    self._stackSize++;
    var keepGoing = callback(null, data);
    if (keepGoing === false) {
      if (typeof onFinish === 'function') {
        onFinish();
      }
    }
    else {
      if (self._closed === false) {
        if (self._stackSize <= MAX_CALL_STACK) {
          self._next().then(resolve).error(function(error) {
            if ((error.message !== 'You cannot retrieve data from a cursor that is closed.') &&
                (error.message.match(/You cannot call 'next' on a closed/) === null)) {
              reject(error);
            }
          });
        }
        else {
          setTimeout(function() {
            self._stackSize = 0;
            self._next().then(resolve).error(function(error) {
              if ((error.message !== 'You cannot retrieve data from a cursor that is closed.') &&
                  (error.message.match(/You cannot call 'next' on a closed/) === null)) {
                reject(error);
              }
            });
          }, 0);
        }
      }
    }
    return null;
  }

  self._next().then(resolve).error(function(error) {
    // We can silence error when the cursor is closed as this
    if ((error.message !== 'You cannot retrieve data from a cursor that is closed.') &&
        (error.message.match(/You cannot call 'next' on a closed/) === null)) {
      reject(error);
    }
  });
  return null;
}
```
- example usage
```shell
...
if (self._draining === true) {
  // There is no need to close the feed here as we'll close the connections
  return feed.close();
}
self._feed = feed;
var initializing = true;
var servers = [];
feed.each(function(err, change) {
  if (err) {
    self._log('The changefeed on server_status returned an error: '+err.toString());
    // We have to refetch everything as the server that was serving the feed may
    // have died.
    if (!self._draining) {
      setTimeout(function() {
        self.fetchServers();
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.eachAsync"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>eachAsync (callback)](#apidoc.element.rethinkdbdash.cursor.prototype.eachAsync)
- description and source-code
```javascript
eachAsync = function (callback) {
  var self = this;
  return new Promise(function(resolve, reject) {
    self._eachAsyncInternal(callback, resolve, reject)
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.emit"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>emit ()](#apidoc.element.rethinkdbdash.cursor.prototype.emit)
- description and source-code
```javascript
emit = function () {
  var self = this;
  if (self._eventEmitter == null) {
    self._makeEmitter();
    setImmediate(function() {
      self._each(self._eachCb.bind(self), function() {
        if (self._emittedEnd === false) {
          self._emittedEnd = true;
          self._eventEmitter.emit('end');
        }
      });
    });
  }
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  self._eventEmitter[method].apply(self._eventEmitter, _args);
}
```
- example usage
```shell
...
self.timeoutOpen = setTimeout(function() {
  self.connection.end(); // Send a FIN packet
  reject(new Err.ReqlDriverError('Failed to connect to '+self.host+':'+self.port+' in less than '+self.timeoutConnect+'s').setOperational
());
}, self.timeoutConnect*1000);

self.connection.on('end', function() {
  self.open = false;
  self.emit('end');
  // We got a FIN packet, so we'll just flush
  self._flush();
});
self.connection.on('close', function() {
  // We emit end or close just once
  clearTimeout(self.timeoutOpen)
  clearInterval(self.pingIntervalId);
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.getType"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>getType ()](#apidoc.element.rethinkdbdash.cursor.prototype.getType)
- description and source-code
```javascript
getType = function () {
  return this._type;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.hasNext"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>hasNext ()](#apidoc.element.rethinkdbdash.cursor.prototype.hasNext)
- description and source-code
```javascript
hasNext = function () {
  throw new Error('The 'hasNext' command has been removed in 1.13, please use 'next'.')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.includesStates"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>includesStates ()](#apidoc.element.rethinkdbdash.cursor.prototype.includesStates)
- description and source-code
```javascript
includesStates = function () {
  return this._setIncludesStates;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.listeners"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>listeners ()](#apidoc.element.rethinkdbdash.cursor.prototype.listeners)
- description and source-code
```javascript
listeners = function () {
  var self = this;
  if (self._eventEmitter == null) {
    self._makeEmitter();
    setImmediate(function() {
      self._each(self._eachCb.bind(self), function() {
        if (self._emittedEnd === false) {
          self._emittedEnd = true;
          self._eventEmitter.emit('end');
        }
      });
    });
  }
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  self._eventEmitter[method].apply(self._eventEmitter, _args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.next"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>next (callback)](#apidoc.element.rethinkdbdash.cursor.prototype.next)
- description and source-code
```javascript
next = function (callback) {
  var self = this;
  if (self._closed === true) {
    return Promise.reject(new Err.ReqlDriverError(
      'You cannot call 'next' on a closed '+self._type).setOperational()
    ).nodeify(callback);
  }
  else if ((self._data.length === 0) && (self._canFetch === false)) {
    return Promise.reject(new Err.ReqlDriverError(
      'No more rows in the '+self._type.toLowerCase()).setOperational()
    ).nodeify(callback);
  }
  else {
    if ((self._data.length > 0) && (self._data[0].length > self._index)) {
      var result = self._data[0][self._index++];
      if (result instanceof Error) {
        return Promise.reject(result).nodeify(callback);
      }
      else {
        // This could be possible if we get back batch with just one document?
        if (self._data[0].length === self._index) {
          self._index = 0;
          self._data.shift();
          if ((self._data.length === 1)
            && (self._canFetch === true)
            && (self._closed === false)
            && (self._fetching === false)) {
              self._fetch();
          }
        }
        return Promise.resolve(result).nodeify(callback);
      }
    }
    else {
      return new Promise(function(resolve, reject) {
        self._pendingPromises.push({resolve: resolve, reject: reject});
      }).nodeify(callback);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.on"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>on ()](#apidoc.element.rethinkdbdash.cursor.prototype.on)
- description and source-code
```javascript
on = function () {
  var self = this;
  if (self._eventEmitter == null) {
    self._makeEmitter();
    setImmediate(function() {
      self._each(self._eachCb.bind(self), function() {
        if (self._emittedEnd === false) {
          self._emittedEnd = true;
          self._eventEmitter.emit('end');
        }
      });
    });
  }
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  self._eventEmitter[method].apply(self._eventEmitter, _args);
}
```
- example usage
```shell
...
// var r = require('rethinkdbdash')({servers: [{host: ..., port: ...}]});
'''

2. Remove everything related to a connection:

'''js
r.connect({host: ..., port: ...}).then(function(connection) {
  connection.on('error', handleError);
  query.run(connection).then(function(result) {
    // console.log(result);
    connection.close();
  });
});
'''
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.once"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>once ()](#apidoc.element.rethinkdbdash.cursor.prototype.once)
- description and source-code
```javascript
once = function () {
  var self = this;
  if (self._eventEmitter == null) {
    self._makeEmitter();
    setImmediate(function() {
      self._each(self._eachCb.bind(self), function() {
        if (self._emittedEnd === false) {
          self._emittedEnd = true;
          self._eventEmitter.emit('end');
        }
      });
    });
  }
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  self._eventEmitter[method].apply(self._eventEmitter, _args);
}
```
- example usage
```shell
...
  self.connection.removeAllListeners();
  self.open = false;
  self.emit('closed');
  // The connection is fully closed, flush (in case 'end' was not triggered)
  self._flush();
});
self.connection.setNoDelay();
self.connection.once('error', function(error) {
  reject(new Err.ReqlDriverError('Failed to connect to '+self.host+':'+self.port+'\nFull error:\n'+JSON.stringify(error)).setOperational
());
});
self.connection.on('connect', function() {
  self.connection.removeAllListeners('error');
  self.connection.on('error', function(error) {
    self.emit('error', error);
  });
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>removeAllListeners ()](#apidoc.element.rethinkdbdash.cursor.prototype.removeAllListeners)
- description and source-code
```javascript
removeAllListeners = function () {
  var self = this;
  if (self._eventEmitter == null) {
    self._makeEmitter();
    setImmediate(function() {
      self._each(self._eachCb.bind(self), function() {
        if (self._emittedEnd === false) {
          self._emittedEnd = true;
          self._eventEmitter.emit('end');
        }
      });
    });
  }
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  self._eventEmitter[method].apply(self._eventEmitter, _args);
}
```
- example usage
```shell
...
  // We got a FIN packet, so we'll just flush
  self._flush();
});
self.connection.on('close', function() {
  // We emit end or close just once
  clearTimeout(self.timeoutOpen)
  clearInterval(self.pingIntervalId);
  self.connection.removeAllListeners();
  self.open = false;
  self.emit('closed');
  // The connection is fully closed, flush (in case 'end' was not triggered)
  self._flush();
});
self.connection.setNoDelay();
self.connection.once('error', function(error) {
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>removeListener ()](#apidoc.element.rethinkdbdash.cursor.prototype.removeListener)
- description and source-code
```javascript
removeListener = function () {
  var self = this;
  if (self._eventEmitter == null) {
    self._makeEmitter();
    setImmediate(function() {
      self._each(self._eachCb.bind(self), function() {
        if (self._emittedEnd === false) {
          self._emittedEnd = true;
          self._eventEmitter.emit('end');
        }
      });
    });
  }
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  self._eventEmitter[method].apply(self._eventEmitter, _args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.setIncludesStates"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>setIncludesStates ()](#apidoc.element.rethinkdbdash.cursor.prototype.setIncludesStates)
- description and source-code
```javascript
setIncludesStates = function () {
  this._setIncludesStates = true;
}
```
- example usage
```shell
...
      currentReject(new Err.ReqlDriverError('Unknown ResponseNote '+response.n[i]+', the driver is probably out of date.').setOperational
());
      return;
    }
  }
}
cursor = new Cursor(self, token, self.metadata[token].options, typeResult);
if (includesStates === true) {
  cursor.setIncludesStates();
}
if ((self.metadata[token].options.cursor === true) || ((self.metadata[token].options.cursor === undefined) && (self.r._options.cursor
 === true))) {
  // Return a cursor
  if (self.metadata[token].options.profile === true) {
    currentResolve({
      profile: response.p,
      result: cursor
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>setMaxListeners ()](#apidoc.element.rethinkdbdash.cursor.prototype.setMaxListeners)
- description and source-code
```javascript
setMaxListeners = function () {
  var self = this;
  if (self._eventEmitter == null) {
    self._makeEmitter();
    setImmediate(function() {
      self._each(self._eachCb.bind(self), function() {
        if (self._emittedEnd === false) {
          self._emittedEnd = true;
          self._eventEmitter.emit('end');
        }
      });
    });
  }
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  self._eventEmitter[method].apply(self._eventEmitter, _args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.toArray"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>toArray (callback)](#apidoc.element.rethinkdbdash.cursor.prototype.toArray)
- description and source-code
```javascript
toArray = function (callback) {
  var self = this;
  var p = new Promise(function(resolve, reject) {
    var result = [];
    var i =0;
    self._each(function(err, data) {
      if (err) {
        reject(err);
      }
      else {
        result.push(data);
      }
    }, function() {
      resolve(result);
    });
  }).nodeify(callback);
  return p;
}
```
- example usage
```shell
...
- Cursors are coerced to arrays by default

'''js
var r = require('rethinkdbdash')();
r.table('data').run().then(function(result) {
  assert(Array.isArray(result)) // true
  // With the official driver you need to call
  // result.toArray().then(function(result2) {
  //   assert(Array.isArray(result2))
  // })
});
'''

#### Drop in
...
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>toJSON ()](#apidoc.element.rethinkdbdash.cursor.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  if (this._type === 'Cursor') {
    throw new Err.ReqlDriverError('You cannot serialize a Cursor to JSON. Retrieve data from the cursor with 'toArray' or 'next'');
  }
  else {
    throw new Err.ReqlDriverError('You cannot serialize a '+this._type+' to JSON. Retrieve data from the cursor with 'each' or '
next'');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.cursor.prototype.toString"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.cursor.prototype.</span>toString ()](#apidoc.element.rethinkdbdash.cursor.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return '[object '+this._type+']';
}
```
- example usage
```shell
...
self.connection.on('error', function(error) {
  self.emit('error', error);
});

var versionBuffer = new Buffer(4)
versionBuffer.writeUInt32LE(protodef.VersionDummy.Version.V1_0, 0)

self.randomString = new Buffer(crypto.randomBytes(18)).toString('base64')
var authBuffer = new Buffer(JSON.stringify({
  protocol_version: PROTOCOL_VERSION,
  authentication_method: AUTHENTIFICATION_METHOD,
  authentication: "n,,n=" + self.user + ",r=" + self.randomString
}));

helper.tryCatch(function() {
...
```



# <a name="apidoc.module.rethinkdbdash.dequeue"></a>[module rethinkdbdash.dequeue](#apidoc.module.rethinkdbdash.dequeue)

#### <a name="apidoc.element.rethinkdbdash.dequeue.dequeue"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>dequeue (size)](#apidoc.element.rethinkdbdash.dequeue.dequeue)
- description and source-code
```javascript
function Dequeue(size) {
  this.start = 0;
  this.end = 0;

  size = size || 50;
  this.buffer = new Array(size);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.dequeue.prototype"></a>[module rethinkdbdash.dequeue.prototype](#apidoc.module.rethinkdbdash.dequeue.prototype)

#### <a name="apidoc.element.rethinkdbdash.dequeue.prototype.delete"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>delete (index)](#apidoc.element.rethinkdbdash.dequeue.prototype.delete)
- description and source-code
```javascript
delete = function (index) {
  var current, next;
  if (this.start+index >= this.buffer.length) {
    current = this.start+index-this.buffer.length;
    next = this.start+index-this.buffer.length+1;
  }
  else {
    current = this.start+index;
    next = this.start+index+1;
  }

  for(var i=index; i<(this.buffer.length-index); i++) {
    if (next === this.buffer.length) next = 0;
    if (current === this.buffer.length) current = 0;

    this.buffer[current] = this.buffer[next];
    current++;
    next++;
  }

  this.end--;
  if (this.end < 0) this.end = this.buffer.length-1
}
```
- example usage
```shell
...

    connection.on('error', function(error) {
// We are going to close connection, but we don't want another process to use it before
// So we remove it from the pool now (if it's inside)
self._log('Error emitted by a connection: '+JSON.stringify(error));
for(var i=0; i<self.getAvailableLength(); i++) {
  if (self._pool.get(i) === this) {
    self._pool.delete(i);
    self.emit('available-size', self._pool.getLength());
    self.emit('available-size-diff', -1);
    break;
  }
}
// We want to make sure that it's not going to try to reconnect
clearTimeout(connection.timeout);
...
```

#### <a name="apidoc.element.rethinkdbdash.dequeue.prototype.get"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>get (index)](#apidoc.element.rethinkdbdash.dequeue.prototype.get)
- description and source-code
```javascript
get = function (index) {
  if (this.start+index > this.buffer.length) {
    return this.buffer[this.start+index-this.buffer.length]
  }
  else {
    return this.buffer[this.start+index]
  }
}
```
- example usage
```shell
...

- Connections are managed by the driver with an efficient connection pool.
Once you have imported the driver, you can immediately run queries,
you don't need to call 'r.connect', or pass a connection to 'run'.

'''js
var r = require('rethinkdbdash')();
r.table('users').get('orphee@gmail.com').run().then(function(user) {
  // ...
}).error(handleError)
'''

- Cursors are coerced to arrays by default

'''js
...
```

#### <a name="apidoc.element.rethinkdbdash.dequeue.prototype.getLength"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>getLength ()](#apidoc.element.rethinkdbdash.dequeue.prototype.getLength)
- description and source-code
```javascript
getLength = function () {
  if (this.start <= this.end) {
    return this.end-this.start;
  }
  else {
    return this.buffer.length-(this.start-this.end);
  }
}
```
- example usage
```shell
...
- 'draining': when 'drain' is called
- 'queueing': when a query is added/removed from the queue (queries waiting for a connection), the size of the queue is provided
- 'size': when the number of connections changes, the number of connections is provided
- 'available-size': when the number of available connections changes, the number of available connections is provided

You can get the number of connections (opened or being opened).
'''js
r.getPoolMaster().getLength();
'''

You can also get the number of available connections (idle connections, without
a query running on it).

'''js
r.getPoolMaster().getAvailableLength();
...
```

#### <a name="apidoc.element.rethinkdbdash.dequeue.prototype.pop"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>pop (element)](#apidoc.element.rethinkdbdash.dequeue.prototype.pop)
- description and source-code
```javascript
pop = function (element) {
  //TODO: Decrease size when possible/needed? This may not be
  //something we really need/want
  // Return the element in this.end-1
  if (this.getLength() > 0) {
    var pos = this.end-1;
    if (pos < 0) pos = this.buffer.length-1;
    this.end = pos;
    var result = this.buffer[pos];
    this.buffer[pos] = undefined;
    return result;
  }
  else {
    return undefined
  }
}
```
- example usage
```shell
...
Pool.prototype.getConnection = function() {
  var self = this;
  var p = new Promise(function(resolve, reject) {
if (self._draining === true) {
  return reject(new Err.ReqlDriverError('The pool is being drained').setOperational());
}

var connection = self._pool.pop();
self.emit('available-size', self._pool.getLength());
self.emit('available-size-diff', -1);

if (connection) {
  clearTimeout(connection.timeout);
  resolve(connection);
}
...
```

#### <a name="apidoc.element.rethinkdbdash.dequeue.prototype.push"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>push (element)](#apidoc.element.rethinkdbdash.dequeue.prototype.push)
- description and source-code
```javascript
push = function (element) {
  // push on this.end and then increase this.end
  // this.end should NEVER be equal to this.buffer.length
  this.buffer[this.end] = element;
  this.end++;
  if (this.end === this.buffer.length) this.end = 0;

  if (this.start === this.end) {
    // Resize
    var previousBuffer = this.buffer;

    this.buffer = new Array(previousBuffer.length*2);

    var i, k = 0;
    for(i=this.start; i<previousBuffer.length; i++) {
      this.buffer[k++] = previousBuffer[i];
    }
    for(i=0; i<this.start; i++) {
      this.buffer[k++] = previousBuffer[i];
    }
    this.start = 0;
    this.end = previousBuffer.length;
  }
}
```
- example usage
```shell
...
          }
        }
        return Promise.resolve(result).nodeify(callback);
      }
    }
    else {
      return new Promise(function(resolve, reject) {
        self._pendingPromises.push({resolve: resolve, reject: reject});
      }).nodeify(callback);
    }
  }
}
Cursor.prototype.hasNext = function() {
  throw new Error('The 'hasNext' command has been removed in 1.13, please use 'next'.')
}
...
```

#### <a name="apidoc.element.rethinkdbdash.dequeue.prototype.shift"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>shift ()](#apidoc.element.rethinkdbdash.dequeue.prototype.shift)
- description and source-code
```javascript
shift = function () {
  // Return the element in this.start

  if (this.getLength() > 0) {
    var result = this.buffer[this.start];
    this.buffer[this.start] = undefined;
    this.start++;
    if (this.start === this.buffer.length) this.start = 0;
    return result;
  }
}
```
- example usage
```shell
...
if (result instanceof Error) {
  return Promise.reject(result).nodeify(callback);
}
else {
  // This could be possible if we get back batch with just one document?
  if (self._data[0].length === self._index) {
    self._index = 0;
    self._data.shift();
    if ((self._data.length === 1)
      && (self._canFetch === true)
      && (self._closed === false)
      && (self._fetching === false)) {
        self._fetch();
    }
  }
...
```

#### <a name="apidoc.element.rethinkdbdash.dequeue.prototype.toArray"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>toArray (index)](#apidoc.element.rethinkdbdash.dequeue.prototype.toArray)
- description and source-code
```javascript
toArray = function (index) {
  var result = [];
  for(var i=0; i<this.getLength(); i++) {
    result.push(this.get(i));
  }
  return result;
}
```
- example usage
```shell
...
- Cursors are coerced to arrays by default

'''js
var r = require('rethinkdbdash')();
r.table('data').run().then(function(result) {
  assert(Array.isArray(result)) // true
  // With the official driver you need to call
  // result.toArray().then(function(result2) {
  //   assert(Array.isArray(result2))
  // })
});
'''

#### Drop in
...
```

#### <a name="apidoc.element.rethinkdbdash.dequeue.prototype.unshift"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.dequeue.prototype.</span>unshift (element)](#apidoc.element.rethinkdbdash.dequeue.prototype.unshift)
- description and source-code
```javascript
unshift = function (element) {
  // push on this.start-1 and then decrease this.start.
  // this.end should NEVER be equal to this.buffer.length

  var pos = this.start-1;
  if (pos < 0) pos = this.buffer.length-1;

  this.buffer[pos] = element;
  this.start = pos;

  if (this.start === this.end) {
    //Resize
    var previousBuffer = this.buffer;

    this.buffer = new Array(previousBuffer.length*2);

    var i, k = 0;
    for(i=this.start; i<previousBuffer.length; i++) {
      this.buffer[k++] = previousBuffer[i];
    }
    for(i=0; i<this.start; i++) {
      this.buffer[k++] = previousBuffer[i];
    }
    this.start = 0;
    this.end = previousBuffer.length;
  }
}
```
- example usage
```shell
...
  var result = {
str: '',
car: ''
  }
  var backtrace, currentFrame, underline;

  if (helper.isPlainObject(term[2])) {
//if ((currentFrame != null) && (frames != null)) frames.unshift(currentFrame);

//underline = Array.isArray(frames) && (frames.length === 0);
var underline = false;
//if (Array.isArray(frames)) currentFrame = frames.shift();

// This works before there is no prefix term than can be called with no normal argument but with an optarg
if (Array.isArray(term[1]) && (term[1].length > 1)) {
...
```



# <a name="apidoc.module.rethinkdbdash.error"></a>[module rethinkdbdash.error](#apidoc.module.rethinkdbdash.error)

#### <a name="apidoc.element.rethinkdbdash.error.ReqlClientError"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.error.</span>ReqlClientError (message)](#apidoc.element.rethinkdbdash.error.ReqlClientError)
- description and source-code
```javascript
function ReqlClientError(message) {
  Error.captureStackTrace(this, ReqlClientError);
  this.message = message;
}
```
- example usage
```shell
...
  else if (type === responseTypes.CLIENT_ERROR) {
self.emit('release');

if (typeof self.metadata[token].reject === 'function') {
  currentResolve = self.metadata[token].resolve;
  currentReject = self.metadata[token].reject;
  self.metadata[token].removeCallbacks();
  currentReject(new Err.ReqlClientError(helper.makeAtom(response), self.metadata[token].query, response));
  if (typeof self.metadata[token].endReject !== 'function') {
    // No pending STOP query, we can delete
    delete self.metadata[token]
  }
}
else if (typeof self.metadata[token].endResolve === 'function') {
  currentResolve = self.metadata[token].endResolve;
...
```

#### <a name="apidoc.element.rethinkdbdash.error.ReqlCompileError"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.error.</span>ReqlCompileError (message, query, frames)](#apidoc.element.rethinkdbdash.error.ReqlCompileError)
- description and source-code
```javascript
function ReqlCompileError(message, query, frames) {
  Error.captureStackTrace(this, ReqlCompileError);
  this.message = message;

  if ((query != null) && (frames)) {
    if ((this.message.length > 0) && (this.message[this.message.length-1] === '.')) {
      this.message = this.message.slice(0, this.message.length-1);
    }

    this.message += ' in:\n';

    frames = frames.b;
    if (frames) this.frames = frames.slice(0);
    //this.frames = JSON.stringify(frames, null, 2);

    var backtrace = generateBacktrace(query, 0, null, frames, {indent: 0, extra: 0});

    var queryLines = backtrace.str.split('\n');
    var carrotLines = backtrace.car.split('\n');

    for(var i=0; i<queryLines.length; i++) {
      this.message += queryLines[i]+'\n';
      if (carrotLines[i].match(/\^/)) {
        var pos = queryLines[i].match(/[^\s]/);
        if ((pos) && (pos.index)) {
          this.message += space(pos.index)+carrotLines[i].slice(pos.index)+'\n';
        }
        else {
          this.message += carrotLines[i]+'\n';
        }
      }
    }
  }
}
```
- example usage
```shell
...
var currentResolve, currentReject;
var datum;
var options;

if (type === responseTypes.COMPILE_ERROR) {
  self.emit('release');
  if (typeof self.metadata[token].reject === 'function') {
    self.metadata[token].reject(new Err.ReqlCompileError(helper.makeAtom(response), self.metadata[token].query, response));
  }

  delete self.metadata[token]
}
else if (type === responseTypes.CLIENT_ERROR) {
  self.emit('release');
...
```

#### <a name="apidoc.element.rethinkdbdash.error.ReqlDriverError"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.error.</span>ReqlDriverError (message, query, secondMessage)](#apidoc.element.rethinkdbdash.error.ReqlDriverError)
- description and source-code
```javascript
function ReqlDriverError(message, query, secondMessage) {
  Error.captureStackTrace(this, ReqlDriverError);
  this.message = this.msg = message;

  if ((Array.isArray(query) && (query.length > 0)) || (!Array.isArray(query) && query != null)) {
    if ((this.message.length > 0) && (this.message[this.message.length-1] === '.')) {
      this.message = this.message.slice(0, this.message.length-1);
    }

    this.message += ' after:\n';

    var backtrace = generateBacktrace(query, 0, null, [], {indent: 0, extra: 0});

    this.message += backtrace.str;
  }
  else {
    if (this.message[this.message.length-1] !== '?') this.message += '.';
  }
  if (secondMessage) this.message += '\n'+secondMessage;
}
```
- example usage
```shell
...

// Set default options - We have to save them in case the user tries to reconnect
if (!helper.isPlainObject(options)) options = {};
this.host = options.host || r._host;
this.port = options.port || r._port;
if (options.authKey != null) {
  if (options.user != null || options.password != null) {
    throw new Err.ReqlDriverError('Cannot use both authKey and password');
  }
  this.user = r._user;
  this.password = options.authKey;
} else {
  if (options.user === undefined) {
    this.user = r._user;
  } else {
...
```

#### <a name="apidoc.element.rethinkdbdash.error.ReqlRuntimeError"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.error.</span>ReqlRuntimeError (message, query, frames)](#apidoc.element.rethinkdbdash.error.ReqlRuntimeError)
- description and source-code
```javascript
function ReqlRuntimeError(message, query, frames) {
  Error.captureStackTrace(this, ReqlRuntimeError);
  this.message = this.msg = message;

  if ((query != null) && (frames)) {
    if ((this.message.length > 0) && (this.message[this.message.length-1] === '.')) {
      this.message = this.message.slice(0, this.message.length-1);
    }

    this.message += ' in:\n';

    frames = frames.b;
    if (frames) this.frames = frames.slice(0);
    //this.frames = JSON.stringify(frames, null, 2);

    var backtrace = generateBacktrace(query, 0, null, frames, {indent: 0, extra: 0});

    var queryLines = backtrace.str.split('\n');
    var carrotLines = backtrace.car.split('\n');

    for(var i=0; i<queryLines.length; i++) {
      this.message += queryLines[i]+'\n';
      if (carrotLines[i].match(/\^/)) {
        var pos = queryLines[i].match(/[^\s]/);
        if ((pos) && (pos.index)) {
          this.message += space(pos.index)+carrotLines[i].slice(pos.index)+'\n';
        }
        else {
          this.message += carrotLines[i]+'\n';
        }
      }
    }
  }
  //this.query = JSON.stringify(query, null, 2);
}
```
- example usage
```shell
...
  }
  else if (type === responseTypes.RUNTIME_ERROR) {
var errorValue = helper.makeAtom(response);
var error;
// We don't want to release a connection if we just pinged it.
if (self.pendingPing === false || (errorValue !== PING_VALUE)) {
  self.emit('release');
  error = new Err.ReqlRuntimeError(errorValue, self.metadata[token].query, response);
} else {
  error = new Err.ReqlRuntimeError(errorValue);
}

if (typeof self.metadata[token].reject === 'function') {
  currentResolve = self.metadata[token].resolve;
  currentReject = self.metadata[token].reject;
...
```

#### <a name="apidoc.element.rethinkdbdash.error.ReqlServerError"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.error.</span>ReqlServerError (message, query)](#apidoc.element.rethinkdbdash.error.ReqlServerError)
- description and source-code
```javascript
function ReqlServerError(message, query) {
  Error.captureStackTrace(this, ReqlServerError);
  this.message = this.msg = message;

  if ((Array.isArray(query) && (query.length > 0)) || (!Array.isArray(query) && query != null)) {
    if ((this.message.length > 0) && (this.message[this.message.length-1] === '.')) {
      this.message = this.message.slice(0, this.message.length-1);
    }

    this.message += ' for:\n';

    var backtrace = generateBacktrace(query, 0, null, [], {indent: 0, extra: 0});

    this.message += backtrace.str;
  }
  else {
    if (this.message[this.message.length-1] !== '?') this.message += '.';
  }
}
```
- example usage
```shell
...
Connection.prototype._isOpen = function() {
return this.open;
}

Connection.prototype._flush = function() {
helper.loopKeys(this.metadata, function(metadata, key) {
  if (typeof metadata[key].reject === 'function') {
    metadata[key].reject(new Err.ReqlServerError(
          'The connection was closed before the query could be completed.',
          metadata[key].query));
  }
  if (typeof metadata[key].endReject === 'function') {
    metadata[key].endReject(new Err.ReqlServerError(
          'The connection was closed before the query could be completed.',
          metadata[key].query));
...
```

#### <a name="apidoc.element.rethinkdbdash.error.generateBacktrace"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.error.</span>generateBacktrace (term, index, father, frames, options)](#apidoc.element.rethinkdbdash.error.generateBacktrace)
- description and source-code
```javascript
function generateBacktrace(term, index, father, frames, options) {
  var result = {
    str: '',
    car: ''
  }
  var backtrace, currentFrame, underline;

  // frames = null -> do not underline
  // frames = [] -> underline

  if (Array.isArray(term)) {
    if (term.length === 0) {
      var underline = Array.isArray(frames) && (frames.length === 0);
      carify(result, 'undefined', underline);
    }
    else if (specialType[term[0]]) {
      backtrace = specialType[term[0]](term, index, father, frames, options);
      result.str = backtrace.str;
      result.car = backtrace.car;
    }
    else if (nonPrefix[term[0]]) {
      backtrace = generateWithoutPrefixBacktrace(term, index, father, frames, options);
      result.str = backtrace.str;
      result.car = backtrace.car;
    }
    else { // normal type -- this.<method>( this.args... )
      backtrace = generateNormalBacktrace(term, index, father, frames, options);
      result.str = backtrace.str;
      result.car = backtrace.car;
    }
  }
  else if (term !== undefined) {
    backtrace = specialType[termTypes.DATUM](term, index, father, frames, options);

    result.str = backtrace.str;
    result.car = backtrace.car;
  }
  else {
    //throw new Error('The driver should never enter this condition. Please report the query to the developers -- End 2')
  }
  return result;
}
```
- example usage
```shell
...
return this.run().finally(handler);
}
Term.prototype.delay = function(msecs) {
return this.run().delay(msecs);
}

Term.prototype.toString = function() {
return Error.generateBacktrace(this._query, 0, null, [], {indent: 0, extra: 0}).str;
}

Term.prototype._wrap = function() {
var self = this;
if (helper.hasImplicit(this._query)) {
  if (this._query[0] === termTypes.ARGS) {
    throw new Error.ReqlDriverError('Implicit variable 'r.row' cannot be used inside 'r.args'')
...
```

#### <a name="apidoc.element.rethinkdbdash.error.setOperational"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.error.</span>setOperational (error)](#apidoc.element.rethinkdbdash.error.setOperational)
- description and source-code
```javascript
setOperational = function (error) {
  error[IS_OPERATIONAL] = true;
  return error;
}
```
- example usage
```shell
...
  }
}

self.connection.setKeepAlive(true);

self.timeoutOpen = setTimeout(function() {
  self.connection.end(); // Send a FIN packet
  reject(new Err.ReqlDriverError('Failed to connect to '+self.host+':'+self.port+' in less than '+self.timeoutConnect+'s').setOperational
());
}, self.timeoutConnect*1000);

self.connection.on('end', function() {
  self.open = false;
  self.emit('end');
  // We got a FIN packet, so we'll just flush
  self._flush();
...
```



# <a name="apidoc.module.rethinkdbdash.helper"></a>[module rethinkdbdash.helper](#apidoc.module.rethinkdbdash.helper)

#### <a name="apidoc.element.rethinkdbdash.helper.changeProto"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>changeProto (object, other)](#apidoc.element.rethinkdbdash.helper.changeProto)
- description and source-code
```javascript
function changeProto(object, other) {
  object.__proto__ = other.__proto__;
}
```
- example usage
```shell
...
var term = function(field) {
  if (Term.prototype._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    Term.prototype._arity(_args, 1, '(...)', self);
  }
  return term.bracket(field);
}
helper.changeProto(term, self);

if (value === undefined) {
  term._query = [];
}
else {
  term._query = value;
}
...
```

#### <a name="apidoc.element.rethinkdbdash.helper.compareDigest"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>compareDigest (a, b)](#apidoc.element.rethinkdbdash.helper.compareDigest)
- description and source-code
```javascript
function compareDigest(a, b) {
  var left = undefined
  var right = b
  var result = undefined
  if (a.length === b.length) {
    left = a
    result = 0
  } else {
    left = b
    result = 1
  }
  var len = Math.min(a.length, b.length);
  for(var i=0; i<len; i++) {
    result |= a[i] ^b[i]
  }
  return result === 0
}
```
- example usage
```shell
...
}

Connection.prototype._compareDigest = function(messageServer, resolve, reject) {
var self = this;
var firstEquals = messageServer.authentication.indexOf('=')
var serverSignatureValue = messageServer.authentication.slice(firstEquals+1)

if (!helper.compareDigest(serverSignatureValue, self.serverSignature.toString("base64"))) {
  reject(new Err.ReqlDriverError('Invalid server signature').setOperational());
}

self.state = 4
self.connection.removeAllListeners('error');
self.open = true;
self.connection.on('error', function(e) {
...
```

#### <a name="apidoc.element.rethinkdbdash.helper.createLogger"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>createLogger (poolMaster, silent)](#apidoc.element.rethinkdbdash.helper.createLogger)
- description and source-code
```javascript
function createLogger(poolMaster, silent) {
  return function(message) {
    if (silent !== true) {
      console.error(message);
    }
    poolMaster.emit('log', message);
  }
}
```
- example usage
```shell
...
self._index = 0; // next pool to used
self._indexUnknown =  0 // next unknown pool to used
self._discovery = (typeof options.discovery === 'boolean') ? options.discovery: false; // Whether the pool master is in discovery
 mode or not
//self._refresh = (typeof options.refresh === 'number') ? options.refresh: 1000*60*60; // Refresh rate for the list of servers
self._options = options;
self._options.buffer = options.buffer || 50;
self._options.max = options.max || 1000;
self._log = helper.createLogger(self, options.silent || false);
self._draining = false;
self._numConnections = 0;
self._numAvailableConnections = 0;
self._hasPrintWarningLocalhost = false;
self._feed = null;
self._consecutiveFails = -1;
self._timeoutError = options.timeoutError || 1000; // How long should we wait before recreating a connection that failed?
...
```

#### <a name="apidoc.element.rethinkdbdash.helper.getCanonicalAddress"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>getCanonicalAddress (addresses)](#apidoc.element.rethinkdbdash.helper.getCanonicalAddress)
- description and source-code
```javascript
function getCanonicalAddress(addresses) {
  // We suppose that the addresses are all valid, and therefore use loose regex
  for(var i=0; i<addresses.length; i++) {
    var addresse = addresses[i];
    if ((/^127(\.\d{1,3}){3}$/.test(addresse.host)) || (/0?:?0?:?0?:?0?:?0?:?0?:0?:1/.test(addresse.host))) {
      addresse.value = 0;
    }
    else if ((net.isIPv6(addresse.host)) && (/^[fF]|[eE]80:.*\:.*\:/.test(addresse.host))) {
      addresse.value = 1;
    }
    else if (/^169\.254\.\d{1,3}\.\d{1,3}$/.test(addresse.host)) {
      addresse.value = 2;
    }
    else if (/^192\.168\.\d{1,3}\.\d{1,3}$/.test(addresse.host)) {
      addresse.value = 3;
    }
    else if (/^172\.(1\d|2\d|30|31)\.\d{1,3}\.\d{1,3}$/.test(addresse.host)) {
      addresse.value = 4;
    }
    else if (/^10(\.\d{1,3}){3}$/.test(addresse.host)) {
      addresse.value = 5;
    }
    else if ((net.isIPv6(addresse.host)) && (/^[fF]|[cCdD].*\:.*\:/.test('addresse.host'))) {
      addresse.value = 6;
    }
    else {
      addresse.value = 7;
    }
  }
  var result = addresses[0];
  var max = addresses[0].value;
  for(var i=0; i<addresses.length; i++) {
    if (addresses[i].value > max) {
      result = addresses[i];
      max = addresses[i].value;
    }
  }
  return result;
}
```
- example usage
```shell
...
      (helper.localhostAliases.hasOwnProperty(server.network.canonical_addresses[k].host) &&
      helper.localhostAliases.hasOwnProperty(pool.options.connection.host))) &&
      (server.network.reql_port === pool.options.connection.port)) {

      self._pools[server.id] = self._pools[UNKNOWN_POOLS].splice(j, 1)[0];
      // We may assign the wrong pool to this server if it's maching on localhost
      if (helper.localhostAliases.hasOwnProperty(server.network.canonical_addresses[k].host)) {
        self._pools[server.id].options.connection.host = helper.getCanonicalAddress(server.network.canonical_addresses).host;
        self._pools[server.id].drainLocalhost();
      }
      found = true;
      break;
    }
  }
}
...
```

#### <a name="apidoc.element.rethinkdbdash.helper.hasImplicit"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>hasImplicit (arg)](#apidoc.element.rethinkdbdash.helper.hasImplicit)
- description and source-code
```javascript
function hasImplicit(arg) {
  if (Array.isArray(arg)) {
    if (arg[0] === termTypes.IMPLICIT_VAR) return true;

    if (Array.isArray(arg[1])) {
      for(var i=0; i<arg[1].length; i++) {
        if (hasImplicit(arg[1][i])) return true;
      }
    }
    if (isPlainObject(arg[2])) {
      for(var key in arg[2]) {
        if (hasImplicit(arg[2][key])) return true;
      }
    }
  }
  else if (isPlainObject(arg)) {
    for(var key in arg) {
      if (hasImplicit(arg[key])) return true;
    }
  }
  return false;
}
```
- example usage
```shell
...
  car: ''
};
var backtrace, underline, currentFrame;

var underline = Array.isArray(frames) && (frames.length === 0);
if (Array.isArray(frames)) currentFrame = frames.shift();

if ((term[1][0][1].length === 1) && (helper.hasImplicit(term[1][1]))) {
  if ((currentFrame != null) && (currentFrame === 1)) {
    backtrace = generateBacktrace(term[1][1], 1, term, frames, options);
  }
  else {
    backtrace = generateBacktrace(term[1][1], 1, term, null, options);
  }
  result.str = backtrace.str;
...
```

#### <a name="apidoc.element.rethinkdbdash.helper.isPlainObject"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>isPlainObject (obj)](#apidoc.element.rethinkdbdash.helper.isPlainObject)
- description and source-code
```javascript
function isPlainObject(obj) {
  return Object.prototype.toString.call(obj) === '[object Object]';
}
```
- example usage
```shell
...

function Connection(r, options, resolve, reject) {
var self = this;
this.r = r;
this.state = 0; // Track the progress of the handshake. -1 will be used for an error state.

// Set default options - We have to save them in case the user tries to reconnect
if (!helper.isPlainObject(options)) options = {};
this.host = options.host || r._host;
this.port = options.port || r._port;
if (options.authKey != null) {
  if (options.user != null || options.password != null) {
    throw new Err.ReqlDriverError('Cannot use both authKey and password');
  }
  this.user = r._user;
...
```

#### <a name="apidoc.element.rethinkdbdash.helper.loopKeys"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>loopKeys (obj, fn)](#apidoc.element.rethinkdbdash.helper.loopKeys)
- description and source-code
```javascript
function loopKeys(obj, fn) {
  var keys = Object.keys(obj);
  var result;
  var keysLength = keys.length;
  for(var i=0; i<keysLength; i++) {
    result = fn(obj, keys[i]);
    if (result === false) return;
  }
}
```
- example usage
```shell
...

  var tlsOptions = options.ssl || false;
  if (tlsOptions === false) {
    self.connection = net.connect(connectionArgs);
  } else {
    if (helper.isPlainObject(tlsOptions)) {
      // Copy the TLS options in connectionArgs
      helper.loopKeys(tlsOptions, function(tlsOptions, key) {
        connectionArgs[key] = tlsOptions[key];
      });
    }
    self.connection = tls.connect(connectionArgs);
  }
}
...
```

#### <a name="apidoc.element.rethinkdbdash.helper.makeAtom"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>makeAtom (response, options)](#apidoc.element.rethinkdbdash.helper.makeAtom)
- description and source-code
```javascript
function makeAtom(response, options) {
  options = options || {};
  return recursivelyConvertPseudotype(response.r[0], options);
}
```
- example usage
```shell
...
var currentResolve, currentReject;
var datum;
var options;

if (type === responseTypes.COMPILE_ERROR) {
  self.emit('release');
  if (typeof self.metadata[token].reject === 'function') {
    self.metadata[token].reject(new Err.ReqlCompileError(helper.makeAtom(response), self.metadata[token].query, response));
  }

  delete self.metadata[token]
}
else if (type === responseTypes.CLIENT_ERROR) {
  self.emit('release');
...
```

#### <a name="apidoc.element.rethinkdbdash.helper.makeSequence"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>makeSequence (response, options)](#apidoc.element.rethinkdbdash.helper.makeSequence)
- description and source-code
```javascript
function makeSequence(response, options) {
  options = options || {};
  return recursivelyConvertPseudotype(response.r, options);
}
```
- example usage
```shell
...
Cursor.prototype._push = function(data) {
  var couldfetch = this._canFetch;
  if (data.done) this._done();
  var response = data.response;
  this._fetching = false;
  // If the cursor was closed, we ignore all following response
  if ((response.r.length > 0) && (couldfetch === true)) {
    this._data.push(helper.makeSequence(response, this.options));
  }
  // this._fetching = false
  if ((this._closed === false) && (this._canFetch) && (this._data.length <= 1)) this._fetch();
  this._flush();
}
// Try to solve as many pending promises as possible
Cursor.prototype._flush = function() {
...
```

#### <a name="apidoc.element.rethinkdbdash.helper.splitCommaEqual"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>splitCommaEqual (message)](#apidoc.element.rethinkdbdash.helper.splitCommaEqual)
- description and source-code
```javascript
function splitCommaEqual(message) {
  var result = {};
  var messageParts = message.split(',');
  for(var i=0; i<messageParts.length; i++) {
    var equalPosition = messageParts[i].indexOf("=")
    result[messageParts[i].slice(0, equalPosition)] = messageParts[i].slice(equalPosition+1);
  }
  return result;
}
```
- example usage
```shell
...
  reject(new Err.ReqlDriverError('Unsupported protocol version: '+PROTOCOL_VERSION+', expected between '+minVersion+' and '+ maxVersion
).setOperational());
}
this.state = 1;
};

Connection.prototype._computeSaltedPassword = function(messageServer, reject) {
var self = this;
var authentication = helper.splitCommaEqual(messageServer.authentication);

var randomNonce = authentication.r
var salt = new Buffer(authentication.s, 'base64')
var iterations = parseInt(authentication.i)

if (randomNonce.substr(0, self.randomString.length) !== self.randomString) {
  self._abort();
...
```

#### <a name="apidoc.element.rethinkdbdash.helper.toArray"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>toArray (args)](#apidoc.element.rethinkdbdash.helper.toArray)
- description and source-code
```javascript
function toArray(args) {
  return Array.prototype.slice.call(args);
}
```
- example usage
```shell
...
- Cursors are coerced to arrays by default

'''js
var r = require('rethinkdbdash')();
r.table('data').run().then(function(result) {
  assert(Array.isArray(result)) // true
  // With the official driver you need to call
  // result.toArray().then(function(result2) {
  //   assert(Array.isArray(result2))
  // })
});
'''

#### Drop in
...
```

#### <a name="apidoc.element.rethinkdbdash.helper.tryCatch"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>tryCatch (toTry, handleError)](#apidoc.element.rethinkdbdash.helper.tryCatch)
- description and source-code
```javascript
function tryCatch(toTry, handleError) {
  try{
  toTry()
  }
  catch(err) {
  handleError(err)
  }
}
```
- example usage
```shell
...
self.randomString = new Buffer(crypto.randomBytes(18)).toString('base64')
var authBuffer = new Buffer(JSON.stringify({
  protocol_version: PROTOCOL_VERSION,
  authentication_method: AUTHENTIFICATION_METHOD,
  authentication: "n,,n=" + self.user + ",r=" + self.randomString
}));

helper.tryCatch(function() {
  self.connection.write(Buffer.concat([versionBuffer, authBuffer, NULL_BUFFER]));
}, function(err) {
  // The TCP connection is open, but the ReQL connection wasn't established.
  // We can just abort the whole thing
  self.open = false;
  reject(new Err.ReqlDriverError('Failed to perform handshake with '+self.host+':'+self.port).setOperational());
});
...
```

#### <a name="apidoc.element.rethinkdbdash.helper.xorBuffer"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.helper.</span>xorBuffer (a, b)](#apidoc.element.rethinkdbdash.helper.xorBuffer)
- description and source-code
```javascript
function xorBuffer(a, b) {
  var result = [];
  var len = Math.min(a.length, b.length)
  for(var i=0; i<len; i++) {
    result.push(a[i] ^ b[i]);
  }
  return new Buffer(result);
}
```
- example usage
```shell
...

var authMessage =
    "n=" + this.user + ",r=" + this.randomString + "," +
    authentication + "," +
    clientFinalMessageWithoutProof

var clientSignature = crypto.createHmac("sha256", storedKey).update(authMessage).digest()
var clientProof = helper.xorBuffer(clientKey, clientSignature)

var serverKey = crypto.createHmac("sha256", saltedPassword).update("Server Key").digest()
this.serverSignature = crypto.createHmac("sha256", serverKey).update(authMessage).digest()

this.state = 2
var message = JSON.stringify({
  authentication: clientFinalMessageWithoutProof + ",p=" + clientProof.toString("base64")
...
```



# <a name="apidoc.module.rethinkdbdash.metadata"></a>[module rethinkdbdash.metadata](#apidoc.module.rethinkdbdash.metadata)

#### <a name="apidoc.element.rethinkdbdash.metadata.metadata"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>metadata (resolve, reject, query, options)](#apidoc.element.rethinkdbdash.metadata.metadata)
- description and source-code
```javascript
function Metadata(resolve, reject, query, options) {
  this.resolve = resolve;
  this.reject = reject;
  this.query = query; // The query in case we have to build a backtrace
  this.options = options || {};
  this.cursor = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.metadata.prototype"></a>[module rethinkdbdash.metadata.prototype](#apidoc.module.rethinkdbdash.metadata.prototype)

#### <a name="apidoc.element.rethinkdbdash.metadata.prototype.removeCallbacks"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.metadata.prototype.</span>removeCallbacks ()](#apidoc.element.rethinkdbdash.metadata.prototype.removeCallbacks)
- description and source-code
```javascript
removeCallbacks = function () {
  this.resolve = null;
  this.reject = null;
}
```
- example usage
```shell
...
  }
  else if (type === responseTypes.CLIENT_ERROR) {
self.emit('release');

if (typeof self.metadata[token].reject === 'function') {
  currentResolve = self.metadata[token].resolve;
  currentReject = self.metadata[token].reject;
  self.metadata[token].removeCallbacks();
  currentReject(new Err.ReqlClientError(helper.makeAtom(response), self.metadata[token].query, response));
  if (typeof self.metadata[token].endReject !== 'function') {
    // No pending STOP query, we can delete
    delete self.metadata[token]
  }
}
else if (typeof self.metadata[token].endResolve === 'function') {
...
```

#### <a name="apidoc.element.rethinkdbdash.metadata.prototype.removeEndCallbacks"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.metadata.prototype.</span>removeEndCallbacks ()](#apidoc.element.rethinkdbdash.metadata.prototype.removeEndCallbacks)
- description and source-code
```javascript
removeEndCallbacks = function () {
  this.endResolve = null;
  this.endReject = null;
}
```
- example usage
```shell
...
    // No pending STOP query, we can delete
    delete self.metadata[token]
  }
}
else if (typeof self.metadata[token].endResolve === 'function') {
  currentResolve = self.metadata[token].endResolve;
  currentReject = self.metadata[token].endReject;
  self.metadata[token].removeEndCallbacks();
  currentReject(new Err.ReqlClientError(helper.makeAtom(response), self.metadata[token].query, response));
  delete self.metadata[token]
}
else if (token === -1) { // This should not happen now since 1.13 took the token out of the query
  var error = new Err.ReqlClientError(helper.makeAtom(response)+'\nClosing all outstanding queries...');
  self.emit('error', error);
  // We don't want a function to yield forever, so we just reject everything
...
```

#### <a name="apidoc.element.rethinkdbdash.metadata.prototype.setCallbacks"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.metadata.prototype.</span>setCallbacks (resolve, reject)](#apidoc.element.rethinkdbdash.metadata.prototype.setCallbacks)
- description and source-code
```javascript
setCallbacks = function (resolve, reject) {
  this.resolve = resolve;
  this.reject = reject;
}
```
- example usage
```shell
...
  if (!self.metadata[token]) {
    self.metadata[token] = new Metadata(resolve, reject, originalQuery, options);
  }
  else if (end === true) {
    self.metadata[token].setEnd(resolve, reject);
  }
  else {
    self.metadata[token].setCallbacks(resolve, reject);
  }
}
else {
  if (typeof resolve === 'function') resolve();
  this.emit('release');
}
...
```

#### <a name="apidoc.element.rethinkdbdash.metadata.prototype.setCursor"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.metadata.prototype.</span>setCursor ()](#apidoc.element.rethinkdbdash.metadata.prototype.setCursor)
- description and source-code
```javascript
setCursor = function () {
  this.cursor = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.metadata.prototype.setEnd"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.metadata.prototype.</span>setEnd (resolve, reject)](#apidoc.element.rethinkdbdash.metadata.prototype.setEnd)
- description and source-code
```javascript
setEnd = function (resolve, reject) {
  this.endResolve = resolve;
  this.endReject = reject;
}
```
- example usage
```shell
...

// noreply instead of noReply because the otpions are translated for the server
if ((!helper.isPlainObject(options)) || (options.noreply != true)) {
  if (!self.metadata[token]) {
    self.metadata[token] = new Metadata(resolve, reject, originalQuery, options);
  }
  else if (end === true) {
    self.metadata[token].setEnd(resolve, reject);
  }
  else {
    self.metadata[token].setCallbacks(resolve, reject);
  }
}
else {
  if (typeof resolve === 'function') resolve();
...
```



# <a name="apidoc.module.rethinkdbdash.pool"></a>[module rethinkdbdash.pool](#apidoc.module.rethinkdbdash.pool)

#### <a name="apidoc.element.rethinkdbdash.pool.pool"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>pool (r, options)](#apidoc.element.rethinkdbdash.pool.pool)
- description and source-code
```javascript
function Pool(r, options) {
  this._r = r;

  if (!helper.isPlainObject(options)) options = {};
  this.options = {};
  this.options.max = options.max || 1000; // 4000 is about the maximum the kernel can take
  var buffer = (typeof options.buffer === 'number') ? options.buffer : 50;
  this.options.buffer = (buffer < this.options.max) ? buffer : this.options.max;
  this.options.timeoutError = options.timeoutError || 1000; // How long should we wait before recreating a connection that failed
?
  this.options.timeoutGb = options.timeoutGb || 60*60*1000; // Default timeout for TCP connection is 2 hours on Linux, we time out
 after one hour.
  this.options.maxExponent = options.maxExponent || 6; // Maximum timeout is 2^maxExponent*timeoutError

  this.options.silent = options.silent || false;

  this.options.connection = {
    host: options.host || this._r._host,
    port: options.port || this._r._port,
    db: options.db || this._r._db,
    timeout: options.timeout || this._r._timeoutConnect,
    authKey: options.authKey,
    user: options.user,
    password: options.password,
    cursor: options.cursor || false,
    stream: options.stream || false,
    ssl: options.ssl || false,
    pingInterval: options.pingInterval || this._r._pingInterval
  }
  this._log = options._log;

  this._pool = new Dequeue(this.options.buffer+1);
  this._draining = false;
  this._drainingHandlers = null; // Store the resolve/reject methods once draining is called
  this._localhostToDrain = 0; // number of connections to "localhost" to remove
  this._connectionToReplace = 0; // number of connections to "localhost" to remove

  this._numConnections = 0;
  this._openingConnections = 0; // Number of connections being opened
  this._consecutiveFails = 0;   // In slow growth, the number of consecutive failures to open a connection
  this._slowGrowth = false;     // Opening one connection at a time
  this._slowlyGrowing = false;  // The next connection to be returned is one opened in slowGrowth mode
  this._extraConnections = 0; // Number of extra connections being opened that we should eventually close

  this._empty = true;

  var self = this;
  // So we can let the pool master bind listeners
  setTimeout(function() {
    if (self._draining === false) {
      for(var i=0; i<self.options.buffer; i++) {
        if (self.getLength() < self.options.max) {
          self.createConnection();
        }
      }
    }
  }, 0);
  this.id = Math.floor(Math.random()*100000);
  this._log('Creating a pool connected to '+this.getAddress());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.pool.super_"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool.</span>super_ ()](#apidoc.element.rethinkdbdash.pool.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.pool.prototype"></a>[module rethinkdbdash.pool.prototype](#apidoc.module.rethinkdbdash.pool.prototype)

#### <a name="apidoc.element.rethinkdbdash.pool.prototype._aggressivelyExpandBuffer"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>_aggressivelyExpandBuffer ()](#apidoc.element.rethinkdbdash.pool.prototype._aggressivelyExpandBuffer)
- description and source-code
```javascript
_aggressivelyExpandBuffer = function () {
  for(var i=0; i<this.options.buffer; i++) {
    this._expandBuffer();
  }
}
```
- example usage
```shell
...
}
// Need another flag
else if ((self._slowlyGrowing === true) && (self._slowGrowth === true) && (self._consecutiveFails > 0)) {
  self._log('Exiting slow growth mode');
  self._consecutiveFails = 0;
  self._slowGrowth = false;
  self._slowlyGrowing = false;
  self._aggressivelyExpandBuffer();
}



connection.on('error', function(error) {
  // We are going to close connection, but we don't want another process to use it before
  // So we remove it from the pool now (if it's inside)
...
```

#### <a name="apidoc.element.rethinkdbdash.pool.prototype._decreaseNumConnections"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>_decreaseNumConnections ()](#apidoc.element.rethinkdbdash.pool.prototype._decreaseNumConnections)
- description and source-code
```javascript
_decreaseNumConnections = function () {
  this._numConnections--;
  this.emit('size', this._numConnections)
  this.emit('size-diff', -1)
  if ((this._drainingHandlers !== null) && (this._numConnections === 0)) {
    this._drainingHandlers.resolve();
  }
  // We do not check for this._empty === false because we want to emit empty if the pool
  // tries to connect to an unavailable server (such that the master can remove it from the
  // healthy pool
  if (this._numConnections === 0) {
    this._empty = true;
    this.emit('empty');
  }
}
```
- example usage
```shell
...
      self.emit('available-size', self._pool.getLength());
      self.emit('available-size-diff', -1);
      break;
    }
  }

  clearTimeout(connection.timeout);
  self._decreaseNumConnections();
  self._expandBuffer();
});
connection.on('timeout', function() {
  for(var i=0; i<self.getAvailableLength(); i++) {
    if (self._pool.get(i) === this) {
      self._pool.delete(i);
      self.emit('available-size', self._pool.getLength());
...
```

#### <a name="apidoc.element.rethinkdbdash.pool.prototype._expandBuffer"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>_expandBuffer ()](#apidoc.element.rethinkdbdash.pool.prototype._expandBuffer)
- description and source-code
```javascript
_expandBuffer = function () {
  if ((this._draining === false) &&
      (this._pool.getLength() < this.options.buffer+this._localhostToDrain) &&
      (this._numConnections < this.options.max+this._localhostToDrain)) {
    this.createConnection();
  }
}
```
- example usage
```shell
...
      if ((self._numConnections === 0) && (self._slowGrowth === true)) {
        // If the server is down we do not want to buffer the queries
        return reject(new Err.ReqlDriverError('The pool does not have any opened connections and failed to open a new one').setOperational
());
      }
    }

    if (self._slowGrowth === false) {
      self._expandBuffer();
    }

  });
  return p;
};

Pool.prototype._decreaseNumConnections = function() {
...
```

#### <a name="apidoc.element.rethinkdbdash.pool.prototype._increaseNumConnections"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>_increaseNumConnections ()](#apidoc.element.rethinkdbdash.pool.prototype._increaseNumConnections)
- description and source-code
```javascript
_increaseNumConnections = function () {
  this._numConnections++;
  this.emit('size', this._numConnections)
  this.emit('size-diff', 1)
}
```
- example usage
```shell
...
  }
  connection.timeout = setTimeout(timeoutCb, self.options.timeoutGb);
}
};

Pool.prototype.createConnection = function() {
var self = this;
self._increaseNumConnections();
self._openingConnections++;

self.emit('creating-connection', self);
if (self._draining === true) {
  return; // Do not create a new connection if we are draining the pool.
}
...
```

#### <a name="apidoc.element.rethinkdbdash.pool.prototype.createConnection"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>createConnection ()](#apidoc.element.rethinkdbdash.pool.prototype.createConnection)
- description and source-code
```javascript
createConnection = function () {
  var self = this;
  self._increaseNumConnections();
  self._openingConnections++;

  self.emit('creating-connection', self);
  if (self._draining === true) {
    return; // Do not create a new connection if we are draining the pool.
  }

  return self._r.connect(self.options.connection).then(function(connection) {
    self.emit('created-connection', self);

    self._openingConnections--;

    if ((self._slowlyGrowing === false) && (self._slowGrowth === true) && (self._openingConnections === 0)) {
      self._consecutiveFails++;
      self._slowlyGrowing = true;
      self.timeoutReconnect = setTimeout(function() {
        self.createConnection();
        //self._expandBuffer();
      }, (1<<Math.min(self.options.maxExponent, self._consecutiveFails))*self.options.timeoutError);
    }
    // Need another flag
    else if ((self._slowlyGrowing === true) && (self._slowGrowth === true) && (self._consecutiveFails > 0)) {
      self._log('Exiting slow growth mode');
      self._consecutiveFails = 0;
      self._slowGrowth = false;
      self._slowlyGrowing = false;
      self._aggressivelyExpandBuffer();
    }



    connection.on('error', function(error) {
      // We are going to close connection, but we don't want another process to use it before
      // So we remove it from the pool now (if it's inside)
      self._log('Error emitted by a connection: '+JSON.stringify(error));
      for(var i=0; i<self.getAvailableLength(); i++) {
        if (self._pool.get(i) === this) {
          self._pool.delete(i);
          self.emit('available-size', self._pool.getLength());
          self.emit('available-size-diff', -1);
          break;
        }
      }
      // We want to make sure that it's not going to try to reconnect
      clearTimeout(connection.timeout);

      // Not sure what happened here, so let's be safe and close this connection.
      connection.close().then(function() {
        return self._expandBuffer();
      }).error(function(e) {
        // We failed to close this connection, but we removed it from the pool... so err, let's just ignore that.
        self._expandBuffer();
      });
    });
    connection.on('end', function(e) {
      // The connection was closed by the server, let's clean...
      for(var i=0; i<self.getAvailableLength(); i++) {
        if (self._pool.get(i) === this) {
          self._pool.delete(i);
          self.emit('available-size', self._pool.getLength());
          self.emit('available-size-diff', -1);
          break;
        }
      }

      clearTimeout(connection.timeout);
      self._decreaseNumConnections();
      self._expandBuffer();
    });
    connection.on('timeout', function() {
      for(var i=0; i<self.getAvailableLength(); i++) {
        if (self._pool.get(i) === this) {
          self._pool.delete(i);
          self.emit('available-size', self._pool.getLength());
          self.emit('available-size-diff', -1);
          break;
        }
      }

      clearTimeout(connection.timeout);
      self._decreaseNumConnections();
      self._expandBuffer();
    });
    connection.on('release', function() {
      if (this._isOpen()) self.putConnection(this);
    });
    self.putConnection(connection);
    return null;
  }).error(function(error) {
    // We failed to create a connection, we are now going to create connections one by one
    self._openingConnections--;
    self._decreaseNumConnections();

    self._slowGrowth = true;
    if (self._slowlyGrowing === false) {
      self._log('Entering slow growth mode');
    }
    self._slowlyGrowing = true;

    // Log an error
    self._log('Fail to create a new connection for the connection pool. Error:'+JSON.stringify(error));

    if (self._openingConnections === 0) {
      self._consecutiveFails++;
      self.timeoutReconnect = setTimeout(function() {
        //self._expandBuffer();
        self.createConnection();
      }, (1<<Math.min(self.options.maxExponent, self._consecutiveFails))*self.options.timeoutError);
    }
  })
}
```
- example usage
```shell
...

  var self = this;
  // So we can let the pool master bind listeners
  setTimeout(function() {
    if (self._draining === false) {
      for(var i=0; i<self.options.buffer; i++) {
        if (self.getLength() < self.options.max) {
          self.createConnection();
        }
      }
    }
  }, 0);
  this.id = Math.floor(Math.random()*100000);
  this._log('Creating a pool connected to '+this.getAddress());
}
...
```

#### <a name="apidoc.element.rethinkdbdash.pool.prototype.drain"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>drain ()](#apidoc.element.rethinkdbdash.pool.prototype.drain)
- description and source-code
```javascript
drain = function () {
  var self = this;
  self._draining = true;
  self._log('Draining the pool connected to '+this.getAddress());
  self.emit('draining');
  var p = new Promise(function(resolve, reject) {
    var connection = self._pool.pop();
    self.emit('available-size', self._pool.getLength());
    self.emit('available-size-diff', -1);
    while(connection) {
      connection.close();
      clearTimeout(connection.timeout);
      connection = self._pool.pop();
    }
    if (self.timeoutReconnect !== undefined) {
      clearTimeout(self.timeoutReconnect);
      self.timeoutReconnect = null;
    }
    if (self.getLength() === 0) {
      resolve();
    }
    else {
      self._drainingHandlers = {
        resolve: resolve,
        reject: reject
      }
    }
  });
  return p;
}
```
- example usage
```shell
...
is solved, this behavior may be changed in the future.

Because the connection pool will keep some connections available, a script will not
terminate. If you have finished executing your queries and want your Node.js script
to exit, you need to drain the pool with:

'''js
r.getPoolMaster().drain();
'''

The pool master by default will log all errors/new states on 'stderr'. If you do not
want to pollute 'stderr', pass 'silent: true' when you import the driver. You can retrieve the
logs by binding a listener for the 'log' event on the pool master.

'''js
...
```

#### <a name="apidoc.element.rethinkdbdash.pool.prototype.drainLocalhost"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>drainLocalhost ()](#apidoc.element.rethinkdbdash.pool.prototype.drainLocalhost)
- description and source-code
```javascript
drainLocalhost = function () {
  var self = this;
  // All the connections are to localhost, let's create new ones (not to localhost)
  self._connectionToReplace = self._numConnections;
  ;
  for(var i=0, numConnections=self._numConnections; i<numConnections; i++) {
    self.createConnection().finally(function() {
      self._localhostToDrain++;
      self._connectionToReplace--;
      if ((self._connectionToReplace === 0) && (self._localhostToDrain > 0)) {
        var len = self._pool.getLength();
        for(var j=0; j<len; j++) {
          if (self._localhostToDrain === 0) {
            break;
          }
          var _connection = self._pool.shift();
          if (helper.localhostAliases.hasOwnProperty(_connection.host)) {
            self._localhostToDrain--;
            _connection.close();
            clearTimeout(_connection.timeout);
          }
          else {
            self._pool.push(_connection);
          }
        }
      }

    });
  }
}
```
- example usage
```shell
...
      helper.localhostAliases.hasOwnProperty(pool.options.connection.host))) &&
      (server.network.reql_port === pool.options.connection.port)) {

      self._pools[server.id] = self._pools[UNKNOWN_POOLS].splice(j, 1)[0];
      // We may assign the wrong pool to this server if it's maching on localhost
      if (helper.localhostAliases.hasOwnProperty(server.network.canonical_addresses[k].host)) {
        self._pools[server.id].options.connection.host = helper.getCanonicalAddress(server.network.canonical_addresses).host;
        self._pools[server.id].drainLocalhost();
      }
      found = true;
      break;
    }
  }
}
if (found === false) {
...
```

#### <a name="apidoc.element.rethinkdbdash.pool.prototype.getAddress"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>getAddress ()](#apidoc.element.rethinkdbdash.pool.prototype.getAddress)
- description and source-code
```javascript
getAddress = function () {
  return this.options.connection.host+':'+this.options.connection.port;
}
```
- example usage
```shell
...
       if (self.getLength() < self.options.max) {
         self.createConnection();
       }
     }
   }
 }, 0);
 this.id = Math.floor(Math.random()*100000);
 this._log('Creating a pool connected to '+this.getAddress());
}

util.inherits(Pool, events.EventEmitter);
/*
* Events:
*  - draining // when 'drain' is called
*  - queueing(size of the queue) // the number of queries being beffered changed
...
```

#### <a name="apidoc.element.rethinkdbdash.pool.prototype.getAvailableLength"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>getAvailableLength ()](#apidoc.element.rethinkdbdash.pool.prototype.getAvailableLength)
- description and source-code
```javascript
getAvailableLength = function () {
  return this._pool.getLength();
}
```
- example usage
```shell
...
r.getPoolMaster().getLength();
'''

You can also get the number of available connections (idle connections, without
a query running on it).

'''js
r.getPoolMaster().getAvailableLength();
'''

You can also drain the pool as mentionned earlier with;

'''js
r.getPoolMaster().drain();
'''
...
```

#### <a name="apidoc.element.rethinkdbdash.pool.prototype.getConnection"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>getConnection ()](#apidoc.element.rethinkdbdash.pool.prototype.getConnection)
- description and source-code
```javascript
getConnection = function () {
  var self = this;
  var p = new Promise(function(resolve, reject) {
    if (self._draining === true) {
      return reject(new Err.ReqlDriverError('The pool is being drained').setOperational());
    }

    var connection = self._pool.pop();
    self.emit('available-size', self._pool.getLength());
    self.emit('available-size-diff', -1);

    if (connection) {
      clearTimeout(connection.timeout);
      resolve(connection);
    }
    else {
      if ((self._numConnections === 0) && (self._slowGrowth === true)) {
        // If the server is down we do not want to buffer the queries
        return reject(new Err.ReqlDriverError('The pool does not have any opened connections and failed to open a new one').setOperational
());
      }
    }

    if (self._slowGrowth === false) {
      self._expandBuffer();
    }

  });
  return p;
}
```
- example usage
```shell
...
// Find a pool with available connections
var result;
for(var i=0; i<self._healthyPools.length; i++) {
  if (self._index >= self._healthyPools.length) {
    self._index = 0;
  }
  if (self._healthyPools[self._index].getAvailableLength() > 0) {
    result = self._healthyPools[self._index].getConnection();
  }
  self._index++;
  if (self._index === self._healthyPools.length) {
    self._index = 0;
  }
  if (result) {
    return result;
...
```

#### <a name="apidoc.element.rethinkdbdash.pool.prototype.getLength"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>getLength ()](#apidoc.element.rethinkdbdash.pool.prototype.getLength)
- description and source-code
```javascript
getLength = function () {
  return this._numConnections;
}
```
- example usage
```shell
...
- 'draining': when 'drain' is called
- 'queueing': when a query is added/removed from the queue (queries waiting for a connection), the size of the queue is provided
- 'size': when the number of connections changes, the number of connections is provided
- 'available-size': when the number of available connections changes, the number of available connections is provided

You can get the number of connections (opened or being opened).
'''js
r.getPoolMaster().getLength();
'''

You can also get the number of available connections (idle connections, without
a query running on it).

'''js
r.getPoolMaster().getAvailableLength();
...
```

#### <a name="apidoc.element.rethinkdbdash.pool.prototype.putConnection"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>putConnection (connection)](#apidoc.element.rethinkdbdash.pool.prototype.putConnection)
- description and source-code
```javascript
putConnection = function (connection) {
  var self = this;
  if (connection.end === false) {
    // Temporary attempt to fix #192 - this should not happen.
    return;
  }
  if (self._empty === true) {
    self._empty = false;
    // We emit not-empty only we have at least one opened connection
    self.emit('not-empty');
  }
  if ((self._localhostToDrain > 0) && (helper.localhostAliases.hasOwnProperty(connection.host))) {
    self._localhostToDrain--;
    connection.close();
    clearTimeout(connection.timeout);
    self.createConnection();
  }
  else if (self._drainingHandlers !== null) {
    connection.close();
    clearTimeout(connection.timeout);
    if (self.getLength() === 0) {
      self._drainingHandlers.resolve();
    }
  }
  else if (self._extraConnections > 0) {
    self._extraConnections--;
    connection.close().error(function(error) {
      self._log('Fail to properly close a connection. Error:'+JSON.stringify(error));
    });
    clearTimeout(connection.timeout);
  }
<span class="apidocCodeCommentSpan">  /*
  // We let the pool garbage collect these connections
  else if (self.getAvailableLength()+1 > self.options.buffer) { // +1 for the connection we may put back
    // Note that because we have available connections here, the pool master has no pending
    // queries.
    connection.close().error(function(error) {
      self._log('Fail to properly close a connection. Error:'+JSON.stringify(error));
    });
    clearTimeout(connection.timeout);
  }
  */
</span>  else {
    self._pool.push(connection);
    self.emit('available-size', self._pool.getLength());
    self.emit('available-size-diff', 1);
    self.emit('new-connection', connection);

    clearTimeout(connection.timeout);
    var timeoutCb = function() {
      if (self._pool.get(0) === connection) {
        if (self._pool.getLength() > self.options.buffer) {
          self._pool.shift().close();
          self.emit('available-size', self._pool.getLength());
          self.emit('available-size-diff', -1);
        }
        else {
          connection.timeout = setTimeout(timeoutCb, self.options.timeoutGb);
        }
      }
      else {
        // This should technically never happens
        connection.timeout = setTimeout(timeoutCb, self.options.timeoutGb);
      }
    }
    connection.timeout = setTimeout(timeoutCb, self.options.timeoutGb);
  }
}
```
- example usage
```shell
...
    }

    clearTimeout(connection.timeout);
    self._decreaseNumConnections();
    self._expandBuffer();
  });
  connection.on('release', function() {
    if (this._isOpen()) self.putConnection(this);
  });
  self.putConnection(connection);
  return null;
}).error(function(error) {
  // We failed to create a connection, we are now going to create connections one by one
  self._openingConnections--;
  self._decreaseNumConnections();
...
```

#### <a name="apidoc.element.rethinkdbdash.pool.prototype.setOptions"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool.prototype.</span>setOptions (options)](#apidoc.element.rethinkdbdash.pool.prototype.setOptions)
- description and source-code
```javascript
setOptions = function (options) {
  if (helper.isPlainObject(options)) {
    for(var key in options) {
      this.options[key] = options[key];
    }
  }
  return this.options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.pool_master"></a>[module rethinkdbdash.pool_master](#apidoc.module.rethinkdbdash.pool_master)

#### <a name="apidoc.element.rethinkdbdash.pool_master.pool_master"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>pool_master (r, options)](#apidoc.element.rethinkdbdash.pool_master.pool_master)
- description and source-code
```javascript
function PoolMaster(r, options) {
  var self = this;
  var options = options || {};
  var lineLength = options.buffer || 50;

  self._r = r;
  self._line = new Dequeue(lineLength);
  self._pools = {};
  self._pools[UNKNOWN_POOLS] = []; // pools for which we do not know the server'id
  self._healthyPools = [];
  self._healthy = false;
  self._init = false;
  self._index = 0; // next pool to used
  self._indexUnknown =  0 // next unknown pool to used
  self._discovery = (typeof options.discovery === 'boolean') ? options.discovery: false; // Whether the pool master is in discovery
 mode or not
  //self._refresh = (typeof options.refresh === 'number') ? options.refresh: 1000*60*60; // Refresh rate for the list of servers
  self._options = options;
  self._options.buffer = options.buffer || 50;
  self._options.max = options.max || 1000;
  self._log = helper.createLogger(self, options.silent || false);
  self._draining = false;
  self._numConnections = 0;
  self._numAvailableConnections = 0;
  self._hasPrintWarningLocalhost = false;
  self._feed = null;
  self._consecutiveFails = -1;
  self._timeoutError = options.timeoutError || 1000; // How long should we wait before recreating a connection that failed?
  self._maxExponent = options.maxExponent || 6; // Maximum timeout is 2^maxExponent*timeoutError

  //TODO
  //self._usingPool = true; // If we have used the pool
  self._seed = 0;

  var pool;
  if (Array.isArray(options.servers)) {
    if (options.servers.length > 0) {
      self._servers = options.servers;
      for(var i=0; i<options.servers.length; i++) {
        var settings = self.createPoolSettings(options, options.servers[i], self._log);
        pool = new Pool(self._r, settings);
        self._pools[UNKNOWN_POOLS].push(pool);
        // A pool is considered healthy by default such that people can do
        // var = require(...)(); query.run();
        self._healthyPools.push(pool);
        self.emitStatus()
      }
    }
    else {
      throw new Err.ReqlDriverError("If 'servers' is an array, it must contain at least one server")
    }
  }
  else {
    self._servers = [{
      host: options.host || 'localhost',
      port: options.port || 28015
    }]
    var settings = self.createPoolSettings(options, {}, self._log);
    pool = new Pool(self._r, settings);
    self._pools[UNKNOWN_POOLS].push(pool);
    self._healthyPools.push(pool);
    self.emitStatus()
  }

  // Initialize all the pools - bind listeners
  for(var i=0; i<self._pools[UNKNOWN_POOLS].length; i++) {
    self.initPool(self._pools[UNKNOWN_POOLS][i]);
  }
  if ((self._discovery === true)) {
    self._timeout = setTimeout(function() { self.fetchServers() }, 0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.super_"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.</span>super_ ()](#apidoc.element.rethinkdbdash.pool_master.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.pool_master.prototype"></a>[module rethinkdbdash.pool_master.prototype](#apidoc.module.rethinkdbdash.pool_master.prototype)

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype._expandAll"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>_expandAll ()](#apidoc.element.rethinkdbdash.pool_master.prototype._expandAll)
- description and source-code
```javascript
_expandAll = function () {
  for(var i=0; i<this._healthyPools.length; i++) {
    this._healthyPools[i]._expandBuffer();
  }
}
```
- example usage
```shell
...
    self._line.push({
      resolve: resolve,
      reject: reject
    });

    self.emit('queueing', self._line.getLength())
    // We could add a condition to be less greedy (for early start)
    self._expandAll();
  });

}
}
PoolMaster.prototype._expandAll = function() {
for(var i=0; i<this._healthyPools.length; i++) {
  this._healthyPools[i]._expandBuffer();
...
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype._flushErrors"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>_flushErrors ()](#apidoc.element.rethinkdbdash.pool_master.prototype._flushErrors)
- description and source-code
```javascript
_flushErrors = function () {
  while(this._line.getLength() > 0) {
    this._line.shift().reject(new Err.ReqlDriverError('None of the pools have an opened connection and failed to open a new one').
setOperational());
    this.emit('queueing', this._line.getLength())
  }
}
```
- example usage
```shell
...
    if (self._healthyPools[i] === this) {
      self._healthyPools.splice(i, 1);
      self.emitStatus()
      break;
    }
  }
  if (self._healthyPools.length === 0) {
    self._flushErrors();
  }

  self.resetBufferParameters();
});
pool.on('draining', function() {
  for(var i=0; i<self._healthyPools.length; i++) {
    if (self._healthyPools[i] === this) {
...
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.createPool"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>createPool (server)](#apidoc.element.rethinkdbdash.pool_master.prototype.createPool)
- description and source-code
```javascript
createPool = function (server) {
  var self = this;
  var address = helper.getCanonicalAddress(server.network.canonical_addresses);
  var settings = self.createPoolSettings(self._options, {
    port: server.network.reql_port,
    host: address.host
  }, self._log);
  var pool = new Pool(self._r, settings);
  self._pools[server.id] = pool
  self.initPool(pool);
  self._healthyPools.push(pool);
  self.emitStatus()
  self.resetBufferParameters();
}
```
- example usage
```shell
...
          found = true;
          break;
        }
      }
    }
    if (found === false) {
      // We just found a new server, let's extract the canonical address and connect to it
      self.createPool(server);
    }
  }
} // Each server know has a pool

// Check if we need to remove pools
helper.loopKeys(self._pools, function(pools, key) { // among the pools with a server id
  if (key !== UNKNOWN_POOLS) {
...
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.createPoolSettings"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>createPoolSettings (globalOptions, serverOptions, log)](#apidoc.element.rethinkdbdash.pool_master.prototype.createPoolSettings)
- description and source-code
```javascript
createPoolSettings = function (globalOptions, serverOptions, log) {
  var settings = {};
  var numServers = Array.isArray(globalOptions.servers) ? globalOptions.servers.length: 1;
  helper.loopKeys(globalOptions, function(options, key) {
    if ((key === 'buffer') || (key === 'max')) {
      settings[key] = Math.ceil(options[key]/numServers);
      settings[key] = Math.ceil(options[key]/numServers);
    }
    else if (key !== 'servers') {
      settings[key] = options[key];
    }
  });
  if (serverOptions) {
    helper.loopKeys(serverOptions, function(options, key) {
      settings[key] = options[key];
    });
  }
  settings._log = log;
  return settings;
}
```
- example usage
```shell
...
self._seed = 0;

var pool;
if (Array.isArray(options.servers)) {
  if (options.servers.length > 0) {
    self._servers = options.servers;
    for(var i=0; i<options.servers.length; i++) {
      var settings = self.createPoolSettings(options, options.servers[i], self._log);
      pool = new Pool(self._r, settings);
      self._pools[UNKNOWN_POOLS].push(pool);
      // A pool is considered healthy by default such that people can do
      // var = require(...)(); query.run();
      self._healthyPools.push(pool);
      self.emitStatus()
    }
...
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.deletePool"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>deletePool (key)](#apidoc.element.rethinkdbdash.pool_master.prototype.deletePool)
- description and source-code
```javascript
deletePool = function (key) {
  var self = this;
  var pool = self._pools[key];
  self._log('Removing pool connected to: '+pool.getAddress())
  pool.drain().then(function() {
    pool.removeAllListeners();
  }).error(function(error) {
    self._log('Pool connected to: '+self._pools[key].getAddress()+' could not be properly drained.')
    self._log(error.message);
    self._log(error.stack);
  });
  delete self._pools[key];
  self.resetBufferParameters();
}
```
- example usage
```shell
...
  }
} // Each server know has a pool

// Check if we need to remove pools
helper.loopKeys(self._pools, function(pools, key) { // among the pools with a server id
  if (key !== UNKNOWN_POOLS) {
    if (knownServer.hasOwnProperty(key) === false) {
      self.deletePool(key); // We just found a pool that doesn't map to any known RethinkDB server
    }
    else {
      knownServer[key].count++;
    }
  }
});
for(var i=0;i<self._pools[UNKNOWN_POOLS].length; i++) {
...
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.drain"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>drain ()](#apidoc.element.rethinkdbdash.pool_master.prototype.drain)
- description and source-code
```javascript
drain = function () {
  this.emit('draining');
  if (this._discovery === true) {
    this._discovery = false;
    if (this._feed != null) {
      this._feed.close();
    }
  }
  this._draining = true;
  var promises = [];
  var pools = this.getPools();
  for(var i=0; i<pools.length; i++) {
    promises.push(pools[i].drain());
  }
  this._healthyPools = [];
  var self = this;
  return Promise.all(promises).then(function() {
    for(var i=0; i<pools.length; i++) {
      pools[i].removeAllListeners();
    }
  }).error(function(error) {
    if (self._options.silent !== true) {
      self._log('Failed to drain all the pools:');
      self._log(error.message);
      self._log(error.stack);
    }
  });
}
```
- example usage
```shell
...
is solved, this behavior may be changed in the future.

Because the connection pool will keep some connections available, a script will not
terminate. If you have finished executing your queries and want your Node.js script
to exit, you need to drain the pool with:

'''js
r.getPoolMaster().drain();
'''

The pool master by default will log all errors/new states on 'stderr'. If you do not
want to pollute 'stderr', pass 'silent: true' when you import the driver. You can retrieve the
logs by binding a listener for the 'log' event on the pool master.

'''js
...
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.emitStatus"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>emitStatus ()](#apidoc.element.rethinkdbdash.pool_master.prototype.emitStatus)
- description and source-code
```javascript
emitStatus = function () {
  var healthy = this._healthyPools.length !== 0;
  if (this._healthy !== healthy) {
    this._healthy = healthy;
    this.emit('healthy', healthy)
  }
}
```
- example usage
```shell
...
    for(var i=0; i<options.servers.length; i++) {
      var settings = self.createPoolSettings(options, options.servers[i], self._log);
      pool = new Pool(self._r, settings);
      self._pools[UNKNOWN_POOLS].push(pool);
      // A pool is considered healthy by default such that people can do
      // var = require(...)(); query.run();
      self._healthyPools.push(pool);
      self.emitStatus()
    }
  }
  else {
    throw new Err.ReqlDriverError("If 'servers' is an array, it must contain at least one server")
  }
}
else {
...
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.fetchServers"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>fetchServers (useSeeds)](#apidoc.element.rethinkdbdash.pool_master.prototype.fetchServers)
- description and source-code
```javascript
fetchServers = function (useSeeds) {
  var self = this;
  var query = self._r.db('rethinkdb').table('server_status')
      .union([SEPARATOR])
      .union(self._r.db('rethinkdb').table('server_status').changes())
  // In case useSeeds is true, we rotate through all the seeds + the pool master
  if (!useSeeds || self._seed === self._servers.length) {
    if (useSeeds && self._seed === self._servers.length) {
      // We increase the back off only when we went through all the seeds
      self._consecutiveFails++;
    }

    self._seed = 0;
    var promise = query.run({cursor: true})
  }
  else {
    var settings = self._servers[self._seed];
    self._seed++;
    var promise = self._r.connect(settings).then(function(connection) {
      return query.run(connection, {cursor: true})
    });
  }
  promise.then(function(feed) {
    if (self._draining === true) {
      // There is no need to close the feed here as we'll close the connections
      return feed.close();
    }
    self._feed = feed;
    var initializing = true;
    var servers = [];
    feed.each(function(err, change) {
      if (err) {
        self._log('The changefeed on server_status returned an error: '+err.toString());
        // We have to refetch everything as the server that was serving the feed may
        // have died.
        if (!self._draining) {
          setTimeout(function() {
            self.fetchServers();
          }, 0); // Give a timeout to let the driver clean the pools
        }
        return;
      }
      if (initializing === true) {
        if (change === SEPARATOR) {
          initializing = false;
          self.handleAllServersResponse(servers);
          // Rerun the whole query after to make sure that a change did not skip/sneak between the union. As long
          // as RethinkDB does not provide initial results
          setTimeout(function() {
            self._r.db('rethinkdb').table('server_status').run({cursor: false}).then(function(servers) {
              self.handleAllServersResponse(servers);
            }).error(function(error) {
              self._log('Fail to retrieve a second copy of server_status');
              //TODO Retry
            });
          }, 1000);
        }
        else {
          servers.push(change);
        }
        return;
      }

      if (change.new_val !== null && change.old_val === null) {
        // New server
        self.createPool(change.new_val);
      }
      else if (change.new_val === null && change.old_val !== null) {
        // A server was removed
        var server = change.old_val;
        if (self._pools[server.id] != null) {
          self.deletePool(server.id);
        }
        else {
          var found = false;
          for(var i=0; i<self._pools[UNKNOWN_POOLS].length; i++) {
            if (((server.network.canonical_addresses[k].host === self._pools[UNKNOWN_POOLS][i].options.connection.host) ||
              (helper.localhostAliases.hasOwnProperty(server.network.canonical_addresses[k].host) && (helper.localhostAliases.hasOwnProperty
(self._pools[UNKNOWN_POOLS][i].options.connection.host)))) &&
              (server.network.reql_port === self._pools[UNKNOWN_POOLS][i].options.connection.port)) {
              found = true;

              (function (pool) {
                self._log('Removing pool connected to: '+pool.getAddress())
                var pool = self._pools[UNKNOWN_POOLS].splice(i, 1)[0];
                pool.drain().then(function() {
                  pool.removeAllListeners();
                }).error(function(error) {
                  if (self._options.silent !== true) {
                    self._log('Pool connected to: '+pool.getAddress()+' could not be properly drained.')
                    self._log(error.message);
                    self._log(error.stack);
                  }
                });
              })(self._pools[UNKNOWN_POOLS][i]);
              break;
            }
          }
        }
        if (found === false) {
          self._log('A server was removed but no pool for this server exists...')
        }
      }
      // We ignore this change since t ...
```
- example usage
```shell
...
}

// Initialize all the pools - bind listeners
for(var i=0; i<self._pools[UNKNOWN_POOLS].length; i++) {
  self.initPool(self._pools[UNKNOWN_POOLS][i]);
}
if ((self._discovery === true)) {
  self._timeout = setTimeout(function() { self.fetchServers() }, 0);
}
}
util.inherits(PoolMaster, events.EventEmitter);

PoolMaster.prototype.getPools = function() {
var result = [];
helper.loopKeys(this._pools, function(pools, key) {
...
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.getAvailableLength"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>getAvailableLength ()](#apidoc.element.rethinkdbdash.pool_master.prototype.getAvailableLength)
- description and source-code
```javascript
getAvailableLength = function () {
  return this._numAvailableConnections;
}
```
- example usage
```shell
...
r.getPoolMaster().getLength();
'''

You can also get the number of available connections (idle connections, without
a query running on it).

'''js
r.getPoolMaster().getAvailableLength();
'''

You can also drain the pool as mentionned earlier with;

'''js
r.getPoolMaster().drain();
'''
...
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.getConnection"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>getConnection ()](#apidoc.element.rethinkdbdash.pool_master.prototype.getConnection)
- description and source-code
```javascript
getConnection = function () {
  var self = this;
  // Find a pool with available connections
  var result;
  for(var i=0; i<self._healthyPools.length; i++) {
    if (self._index >= self._healthyPools.length) {
      self._index = 0;
    }
    if (self._healthyPools[self._index].getAvailableLength() > 0) {
      result = self._healthyPools[self._index].getConnection();
    }
    self._index++;
    if (self._index === self._healthyPools.length) {
      self._index = 0;
    }
    if (result) {
      return result;
    }
  }
  if (self._healthyPools.length === 0) {
    return new Promise(function(resolve, reject) {
      reject(new Err.ReqlDriverError('None of the pools have an opened connection and failed to open a new one').setOperational());
    });
  }
  else {
    // All pool are busy, buffer the request
    return new Promise(function(resolve, reject) {
      self._line.push({
        resolve: resolve,
        reject: reject
      });

      self.emit('queueing', self._line.getLength())
      // We could add a condition to be less greedy (for early start)
      self._expandAll();
    });

  }
}
```
- example usage
```shell
...
// Find a pool with available connections
var result;
for(var i=0; i<self._healthyPools.length; i++) {
  if (self._index >= self._healthyPools.length) {
    self._index = 0;
  }
  if (self._healthyPools[self._index].getAvailableLength() > 0) {
    result = self._healthyPools[self._index].getConnection();
  }
  self._index++;
  if (self._index === self._healthyPools.length) {
    self._index = 0;
  }
  if (result) {
    return result;
...
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.getLength"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>getLength ()](#apidoc.element.rethinkdbdash.pool_master.prototype.getLength)
- description and source-code
```javascript
getLength = function () {
  return this._numConnections;
}
```
- example usage
```shell
...
- 'draining': when 'drain' is called
- 'queueing': when a query is added/removed from the queue (queries waiting for a connection), the size of the queue is provided
- 'size': when the number of connections changes, the number of connections is provided
- 'available-size': when the number of available connections changes, the number of available connections is provided

You can get the number of connections (opened or being opened).
'''js
r.getPoolMaster().getLength();
'''

You can also get the number of available connections (idle connections, without
a query running on it).

'''js
r.getPoolMaster().getAvailableLength();
...
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.getNumAvailableConnections"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>getNumAvailableConnections ()](#apidoc.element.rethinkdbdash.pool_master.prototype.getNumAvailableConnections)
- description and source-code
```javascript
getNumAvailableConnections = function () {
  var sum = 0;
  for(var i=0; i<this._healthyPools.length; i++) {
    sum += this._healthyPools[i].getAvailableLength();
  }
  return sum;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.getNumConnections"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>getNumConnections ()](#apidoc.element.rethinkdbdash.pool_master.prototype.getNumConnections)
- description and source-code
```javascript
getNumConnections = function () {
  var sum = 0;
  for(var i=0; i<this._healthyPools.length; i++) {
    sum += this._healthyPools[i].getLength();
  }
  return sum;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.getPools"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>getPools ()](#apidoc.element.rethinkdbdash.pool_master.prototype.getPools)
- description and source-code
```javascript
getPools = function () {
  var result = [];
  helper.loopKeys(this._pools, function(pools, key) {
    if (key === UNKNOWN_POOLS) {
      for(var i=0;i<pools[key].length; i++) {
        result.push(pools[key][i]);
      }
    }
    else {
      result.push(pools[key]);
    }
  });
  return result;
}
```
- example usage
```shell
...

'''js
r.getPoolMaster().drain();
'''

You can access all the pools with:
'''js
r.getPoolMaster().getPools();
'''

The pool master emits the 'healthy' when its state change. Its state is defined as:
- healthy when at least one pool is healthy: Queries can be immediately executed or will be queued.
- not healthy when no pool is healthy: Queries will immediately fail.

A pool being healthy is it has at least one available connection, or it was just
...
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.handleAllServersResponse"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>handleAllServersResponse (servers)](#apidoc.element.rethinkdbdash.pool_master.prototype.handleAllServersResponse)
- description and source-code
```javascript
handleAllServersResponse = function (servers) {
  var self = this;
  if (self._draining === true) {
    return;
  }
  // Fill all the known server from RethinkDB
  var knownServer = {};
  for(var i=0; i<servers.length; i++) {
    var server = servers[i];
    knownServer[server.id] = {count: 0, server: server};
    if (self._pools[server.id] === undefined) {
      // We potentially have a new server in the cluster, or we already have a pool for this server
      // in one of the UNKNOWN_POOLS
      var found = false;
      for(var j=0; j<self._pools[UNKNOWN_POOLS].length; j++) {
        if (found) break;
        var pool = self._pools[UNKNOWN_POOLS][j];
        // If a pool is created with localhost, it will probably match the first server even though it may not the the one
        // So it gets an id
        for(var k=0; k<server.network.canonical_addresses.length; k++) {
          // Check for the same host (or if they are both localhost) and port
          if (((server.network.canonical_addresses[k].host === pool.options.connection.host) ||
               (server.network.hostname === pool.options.connection.host) ||
            (helper.localhostAliases.hasOwnProperty(server.network.canonical_addresses[k].host) &&
            helper.localhostAliases.hasOwnProperty(pool.options.connection.host))) &&
            (server.network.reql_port === pool.options.connection.port)) {

            self._pools[server.id] = self._pools[UNKNOWN_POOLS].splice(j, 1)[0];
            // We may assign the wrong pool to this server if it's maching on localhost
            if (helper.localhostAliases.hasOwnProperty(server.network.canonical_addresses[k].host)) {
              self._pools[server.id].options.connection.host = helper.getCanonicalAddress(server.network.canonical_addresses).host
;
              self._pools[server.id].drainLocalhost();
            }
            found = true;
            break;
          }
        }
      }
      if (found === false) {
        // We just found a new server, let's extract the canonical address and connect to it
        self.createPool(server);
      }
    }
  } // Each server know has a pool

  // Check if we need to remove pools
  helper.loopKeys(self._pools, function(pools, key) { // among the pools with a server id
    if (key !== UNKNOWN_POOLS) {
      if (knownServer.hasOwnProperty(key) === false) {
        self.deletePool(key); // We just found a pool that doesn't map to any known RethinkDB server
      }
      else {
        knownServer[key].count++;
      }
    }
  });
  for(var i=0;i<self._pools[UNKNOWN_POOLS].length; i++) {
    // These pools does not match any server returned by RethinkDB.
    var pool = self._pools[UNKNOWN_POOLS].splice(i, 1)[0];
    self._log('Removing pool connected to: '+pool.getAddress())
    pool.drain().then(function() {
      pool.removeAllListeners();
    }).error(function(error) {
      self._log('Pool connected to: '+self._pools[UNKNOWN_POOLS][i].getAddress()+' could not be properly drained.')
      self._log(error.message);
      self._log(error.stack);
    });
  }
}
```
- example usage
```shell
...
    }, 0); // Give a timeout to let the driver clean the pools
  }
  return;
}
if (initializing === true) {
  if (change === SEPARATOR) {
    initializing = false;
    self.handleAllServersResponse(servers);
    // Rerun the whole query after to make sure that a change did not skip/sneak between the union. As long
    // as RethinkDB does not provide initial results
    setTimeout(function() {
      self._r.db('rethinkdb').table('server_status').run({cursor: false}).then(function(servers) {
        self.handleAllServersResponse(servers);
      }).error(function(error) {
        self._log('Fail to retrieve a second copy of server_status');
...
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.initPool"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>initPool (pool)](#apidoc.element.rethinkdbdash.pool_master.prototype.initPool)
- description and source-code
```javascript
initPool = function (pool) {
  var self = this;

  pool.on('size-diff', function(diff) {
    self._numConnections += diff;
    self.emit('size', self._numConnections)
  });
  pool.on('available-size-diff', function(diff) {
    self._numAvailableConnections += diff;
    self.emit('available-size', self._numAvailableConnections)
  });

  pool.on('new-connection', function() {
    if (self._line.getLength() > 0) {
      var p = self._line.shift();
      this.getConnection().then(p.resolve).error(p.reject);
      self.emit('queueing', self._line.getLength())
    }
  });
  pool.on('not-empty', function() {
    if (self._draining === false) {
      var found = false;
      for(var i=0; i<self._healthyPools.length; i++) {
        if (self._healthyPools[i] === this) {
          self._healthyPools.length;
          found = true;
          break;
        }
      }
      if (found === false) {
        self._healthyPools.push(this);
        self.emitStatus()
        self.resetBufferParameters();
      }
    }
  });
  pool.on('empty', function() {
    // A pool that become empty is considered unhealthy
    for(var i=0; i<self._healthyPools.length; i++) {
      if (self._healthyPools[i] === this) {
        self._healthyPools.splice(i, 1);
        self.emitStatus()
        break;
      }
    }
    if (self._healthyPools.length === 0) {
      self._flushErrors();
    }

    self.resetBufferParameters();
  });
  pool.on('draining', function() {
    for(var i=0; i<self._healthyPools.length; i++) {
      if (self._healthyPools[i] === this) {
        self._healthyPools.splice(i, 1);
        self.emitStatus()
        break;
      }
    }

    if (self._healthyPools === 0) {
      self._flushErrors();
    }
  });
}
```
- example usage
```shell
...
    self._pools[UNKNOWN_POOLS].push(pool);
    self._healthyPools.push(pool);
    self.emitStatus()
  }

  // Initialize all the pools - bind listeners
  for(var i=0; i<self._pools[UNKNOWN_POOLS].length; i++) {
    self.initPool(self._pools[UNKNOWN_POOLS][i]);
  }
  if ((self._discovery === true)) {
    self._timeout = setTimeout(function() { self.fetchServers() }, 0);
  }
}
util.inherits(PoolMaster, events.EventEmitter);
...
```

#### <a name="apidoc.element.rethinkdbdash.pool_master.prototype.resetBufferParameters"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.pool_master.prototype.</span>resetBufferParameters ()](#apidoc.element.rethinkdbdash.pool_master.prototype.resetBufferParameters)
- description and source-code
```javascript
resetBufferParameters = function () {
  var max = Math.floor(this._options.max/this._healthyPools.length)
  var buffer = Math.floor(this._options.buffer/this._healthyPools.length)
  for(var i=0; i<this._healthyPools.length; i++) {
    if (this._healthyPools[i].getLength() > max) {
      this._healthyPools[i]._extraConnections = this._healthyPools[i].getLength()-max;
    }
    else {
      this._healthyPools[i]._extraConnections = 0;
    }
    this._healthyPools[i].options.max = max
    this._healthyPools[i].options.buffer = buffer;
  }
}
```
- example usage
```shell
...
  host: address.host
}, self._log);
var pool = new Pool(self._r, settings);
self._pools[server.id] = pool
self.initPool(pool);
self._healthyPools.push(pool);
self.emitStatus()
self.resetBufferParameters();
}

// Delete a known pool
PoolMaster.prototype.deletePool = function(key) {
var self = this;
var pool = self._pools[key];
self._log('Removing pool connected to: '+pool.getAddress())
...
```



# <a name="apidoc.module.rethinkdbdash.stream"></a>[module rethinkdbdash.stream](#apidoc.module.rethinkdbdash.stream)

#### <a name="apidoc.element.rethinkdbdash.stream.stream"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>stream (options, cursor)](#apidoc.element.rethinkdbdash.stream.stream)
- description and source-code
```javascript
function ReadableStream(options, cursor) {
  if (cursor) this._cursor = cursor;
  this._pending = 0; // How many time we called _read while no cursor was available
  this._index = 0;
  this._maxRecursion = 1000; // Hardcoded
  this._highWaterMark = options.highWaterMark;
  this._closed = false;

  Readable.call(this, {
    objectMode: true,
    highWaterMark: this._highWaterMark
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.stream.super_"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.stream.</span>super_ (options)](#apidoc.element.rethinkdbdash.stream.super_)
- description and source-code
```javascript
function Readable(options) {
  if (!(this instanceof Readable))
    return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function')
    this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.stream.prototype"></a>[module rethinkdbdash.stream.prototype](#apidoc.module.rethinkdbdash.stream.prototype)

#### <a name="apidoc.element.rethinkdbdash.stream.prototype._fetch"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.stream.prototype.</span>_fetch ()](#apidoc.element.rethinkdbdash.stream.prototype._fetch)
- description and source-code
```javascript
_fetch = function () {
  var self = this;
  if (self._closed === true) {
    return;
  }
  if (self._cursor._closed === true) {
    self.push(null);
  }
  else {
    self._cursor._next().then(function(data) {
      if (self._closed === true) {
        return;
      }
      // Silently drop null values for now
      if (data === null) {
        if (self._recursion++ === self._maxRecursion) {
          process.nextTick(function() {
            self._fetch();
          });
        }
        else {
          self._fetch();
        }
      }
      else {
        if (self.push(data) !== false) {
          if (self._recursion++ === self._maxRecursion) {
            process.nextTick(function() {
              self._fetch();
            });
          }
          else {
            self._fetch();
          }
        }
      }
      return null;
    }).error(function(error) {
      if (error.message.match(/No more rows in the/)) {
        self.push(null);
      }
      else if (error.message === 'You cannot retrieve data from a cursor that is closed.') {
        // if the user call 'close', the cursor may reject pending requests. We just
        // ignore them here.
      }
      else {
        self.emit('error', error);
        self.push(null);
      }
    });
  }
}
```
- example usage
```shell
...
    if (self._data[0].length === self._index) {
      self._index = 0;
      self._data.shift();
      if ((self._data.length === 1)
        && (self._canFetch === true)
        && (self._closed === false)
        && (self._fetching === false)) {
          self._fetch();
      }
    }
    return Promise.resolve(result).nodeify(callback);
  }
}
else {
  return new Promise(function(resolve, reject) {
...
```

#### <a name="apidoc.element.rethinkdbdash.stream.prototype._fetchAndDecrement"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.stream.prototype.</span>_fetchAndDecrement ()](#apidoc.element.rethinkdbdash.stream.prototype._fetchAndDecrement)
- description and source-code
```javascript
_fetchAndDecrement = function () {
  var self = this;
  self._pending--;
  if (self._pending < 0 || self._closed === true) {
    return;
  }

  if (self._cursor._closed === true) {
    self.push(null);
  }
  else {
    self._cursor._next().then(function(data) {
      // Silently drop null values for now
      if (data === null) {
        if (self._recursion++ === self._maxRecursion) {
          //Avoid maximum call stack errors
          process.nextTick(function() {
            self._fetchAndDecrement();
          });
        }
        else {
          self._fetchAndDecrement();
        }
      }
      else {
        if (self.push(data) !== false) {
          if (self._recursion++ === self._maxRecursion) {
            process.nextTick(function() {
              self._fetchAndDecrement();
            });
          }
          else {
            self._fetchAndDecrement();
          }
        }
      }
      return null;
    }).error(function(error) {
      if (error.message.match(/No more rows in the/)) {
        self.push(null);
      }
      else if (error.message === 'You cannot retrieve data from a cursor that is closed.') {
        // if the user call 'close', the cursor may reject pending requests. We just
        // ignore them here.
      }
      else {
        self.emit('error', error);
        self.push(null);
      }
    });
  }
}
```
- example usage
```shell
...
ReadableStream.prototype._setCursor = function(cursor) {
if (cursor instanceof Cursor === false) {
  this.emit('error', new Error('Cannot create a stream on a single value.'));
  this.push(null);
  return this;
}
this._cursor = cursor;
this._fetchAndDecrement();
}
ReadableStream.prototype._read = function(size) {
this._count++;
if (this._cursor === undefined) {
  this._pending++;
  return;
}
...
```

#### <a name="apidoc.element.rethinkdbdash.stream.prototype._read"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.stream.prototype.</span>_read (size)](#apidoc.element.rethinkdbdash.stream.prototype._read)
- description and source-code
```javascript
_read = function (size) {
  this._count++;
  if (this._cursor === undefined) {
    this._pending++;
    return;
  }

  this._recursion = 0;
  this._fetch();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.stream.prototype._setCursor"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.stream.prototype.</span>_setCursor (cursor)](#apidoc.element.rethinkdbdash.stream.prototype._setCursor)
- description and source-code
```javascript
_setCursor = function (cursor) {
  if (cursor instanceof Cursor === false) {
    this.emit('error', new Error('Cannot create a stream on a single value.'));
    this.push(null);
    return this;
  }
  this._cursor = cursor;
  this._fetchAndDecrement();
}
```
- example usage
```shell
...
  //toStream make sure that options is an object
  helper.loopKeys(options, function(obj, key) {
    _options[key] = obj[key];
  });
  _options.cursor = true;
  stream = new ReadableStream(_options);
  this.run(connection, _options).then(function(cursor) {
    stream._setCursor(cursor);
    return null;
  }).error(function(error) {
    stream.emit('error', error);
  });
}
else {
  helper.loopKeys(connection, function(obj, key) {
...
```

#### <a name="apidoc.element.rethinkdbdash.stream.prototype.close"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.stream.prototype.</span>close ()](#apidoc.element.rethinkdbdash.stream.prototype.close)
- description and source-code
```javascript
close = function () {
  this._closed = true;
  this.push(null);
  return this._cursor.close();
}
```
- example usage
```shell
...
2. Remove everything related to a connection:

'''js
r.connect({host: ..., port: ...}).then(function(connection) {
  connection.on('error', handleError);
  query.run(connection).then(function(result) {
    // console.log(result);
    connection.close();
  });
});
'''

Becomes:

'''js
...
```



# <a name="apidoc.module.rethinkdbdash.term"></a>[module rethinkdbdash.term](#apidoc.module.rethinkdbdash.term)

#### <a name="apidoc.element.rethinkdbdash.term.term"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>term (r, value, error)](#apidoc.element.rethinkdbdash.term.term)
- description and source-code
```javascript
function Term(r, value, error) {
  var self = this;
  var term = function(field) {
    if (Term.prototype._fastArity(arguments.length, 1) === false) {
      var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
      Term.prototype._arity(_args, 1, '(...)', self);
    }
    return term.bracket(field);
  }
  helper.changeProto(term, self);

  if (value === undefined) {
    term._query = [];
  }
  else {
    term._query = value;
  }
  term._r = r; // Keep a reference to r for global settings

  if (error !== undefined) {
    term._error = error;
    term._frames = [];
  }

  return term;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.term.prototype"></a>[module rethinkdbdash.term.prototype](#apidoc.module.rethinkdbdash.term.prototype)

#### <a name="apidoc.element.rethinkdbdash.term.prototype.ISO8601"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>ISO8601 (isoTime, options)](#apidoc.element.rethinkdbdash.term.prototype.ISO8601)
- description and source-code
```javascript
ISO8601 = function (isoTime, options) {
  this._noPrefix(this, 'ISO8601');
  if (this._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 1, 2, 'ISO8601', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.ISO8601)
  var args = [new Term(this._r).expr(isoTime)._query];
  term._fillArgs(args);
  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if (key !== 'defaultTimezone') {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'ISO8601'. Available options are primaryKey <string>,
durability <string>, datancenter <string>');
      }
    });
    term._query.push(new Term(this._r).expr(translateOptions(options))._query);
  }

  return term;
}
```
- example usage
```shell
...
  if (expression instanceof Term) {
return expression;
  }
  else if (expression instanceof Function) {
return new Func(self._r, expression);
  }
  else if (expression instanceof Date) {
return new Term(self._r).ISO8601(expression.toISOString())
  }
  else if (Array.isArray(expression)) {
var term = new Term(self._r);
term._query.push(termTypes.MAKE_ARRAY);

var args = [];
for(var i=0; i<expression.length; i++) {
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype._arity"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_arity (args, num, method, term)](#apidoc.element.rethinkdbdash.term.prototype._arity)
- description and source-code
```javascript
_arity = function (args, num, method, term) {
  var foundArgs = false;
  for(var i=0; i<args.length; i++) {
    if ((args[i] instanceof Term) && (args[i]._query[0] === termTypes.ARGS)) {
      foundArgs = true;
      break;
    }
  }
  if (foundArgs === false) {
    throw new Error.ReqlDriverError('''+method+'' takes '+num+' argument'+((num>1)?'s':'')+', '+args.length+' provided', term._query
);
  }
}
```
- example usage
```shell
...
var TransformStream = require(__dirname+'/transform_stream.js');

function Term(r, value, error) {
var self = this;
var term = function(field) {
  if (Term.prototype._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    Term.prototype._arity(_args, 1, '(...)', self);
  }
  return term.bracket(field);
}
helper.changeProto(term, self);

if (value === undefined) {
  term._query = [];
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype._arityRange"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_arityRange (args, min, max, method, term)](#apidoc.element.rethinkdbdash.term.prototype._arityRange)
- description and source-code
```javascript
_arityRange = function (args, min, max, method, term) {
  var foundArgs = false;
  if (args.length < min) {
    for(var i=0; i<args.length; i++) {
      if ((args[i] instanceof Term) && (args[i]._query[0] === termTypes.ARGS)) {
        foundArgs = true;
        break;
      }
    }
    if (foundArgs === false) {
      throw new Error.ReqlDriverError('''+method+'' takes at least '+min+' argument'+((min>1)?'s':'')+', '+args.length+' provided
', term._query);
    }
  }
  else if (args.length > max) {
    for(var i=0; i<args.length; i++) {
      if ((args[i] instanceof Term) && (args[i]._query[0] === termTypes.ARGS)) {
        foundArgs = true;
        break;
      }
    }
    if (foundArgs === false) {
      throw new Error.ReqlDriverError('''+method+'' takes at most '+max+' argument'+((max>1)?'s':'')+', '+args.length+' provided
', term._query);
    }
  }
}
```
- example usage
```shell
...
}

// Manipulating Tables
Term.prototype.tableCreate = function(table, options) {
var self = this;
if (self._fastArityRange(arguments.length, 1, 2) === false) {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  self._arityRange(_args, 1, 2, 'tableCreate', self);
}


var term = new Term(self._r);
term._query.push(termTypes.TABLE_CREATE)

var args = [];
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype._fastArity"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_fastArity (len, num)](#apidoc.element.rethinkdbdash.term.prototype._fastArity)
- description and source-code
```javascript
_fastArity = function (len, num) {
  return (len === num);
}
```
- example usage
```shell
...
var ReadableStream = require(__dirname+'/stream.js');
var WritableStream = require(__dirname+'/writable_stream.js');
var TransformStream = require(__dirname+'/transform_stream.js');

function Term(r, value, error) {
var self = this;
var term = function(field) {
  if (Term.prototype._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    Term.prototype._arity(_args, 1, '(...)', self);
  }
  return term.bracket(field);
}
helper.changeProto(term, self);
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype._fastArityRange"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_fastArityRange (len, min, max)](#apidoc.element.rethinkdbdash.term.prototype._fastArityRange)
- description and source-code
```javascript
_fastArityRange = function (len, min, max) {
  return ((len >= min) && (len <= max));
}
```
- example usage
```shell
...
term._query.push(termTypes.DB_LIST)
return term;
}

// Manipulating Tables
Term.prototype.tableCreate = function(table, options) {
var self = this;
if (self._fastArityRange(arguments.length, 1, 2) === false) {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  self._arityRange(_args, 1, 2, 'tableCreate', self);
}


var term = new Term(self._r);
term._query.push(termTypes.TABLE_CREATE)
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype._fillArgs"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_fillArgs (args)](#apidoc.element.rethinkdbdash.term.prototype._fillArgs)
- description and source-code
```javascript
_fillArgs = function (args) {
  var foundError = false;
  var internalArgs = [];
  for(var i=0; i<args.length; i++) {
  if (args[i] instanceof Term) {
    internalArgs.push(args[i]._query);
    if (!foundError && (args[i]._error != null)) {
    this._error = args[i]._error;
    this._frames = args[i]._frames;
    this._frames.unshift(i);
    foundError = true;
    }
  }
  else {
    internalArgs.push(args[i]);
  }
  }
  this._query.push(internalArgs);
  return this;
}
```
- example usage
```shell
...
Term.prototype.dbCreate = function(db) {
// Check for arity is done in r.prototype.dbCreate
this._noPrefix(this, 'dbCreate');

var term = new Term(this._r);
term._query.push(termTypes.DB_CREATE);
var args = [new Term(this._r).expr(db)._query]
term._fillArgs(args);
return term;
}
Term.prototype.dbDrop = function(db) {
this._noPrefix(this, 'dbDrop');

var term = new Term(this._r);
term._query.push(termTypes.DB_DROP);
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype._noPrefix"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_noPrefix (term, method)](#apidoc.element.rethinkdbdash.term.prototype._noPrefix)
- description and source-code
```javascript
_noPrefix = function (term, method) {
  if ((!Array.isArray(term._query)) || (term._query.length > 0)) {
    throw new Error.ReqlDriverError('''+method+'' is not defined', term._query);
  }
}
```
- example usage
```shell
...
  }
}


// Manipulating databases
Term.prototype.dbCreate = function(db) {
  // Check for arity is done in r.prototype.dbCreate
  this._noPrefix(this, 'dbCreate');

  var term = new Term(this._r);
  term._query.push(termTypes.DB_CREATE);
  var args = [new Term(this._r).expr(db)._query]
  term._fillArgs(args);
  return term;
}
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype._setArrayLimit"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_setArrayLimit (arrayLimit)](#apidoc.element.rethinkdbdash.term.prototype._setArrayLimit)
- description and source-code
```javascript
_setArrayLimit = function (arrayLimit) {
  Term.prototype._arrayLimit = arrayLimit;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype._setNestingLevel"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_setNestingLevel (nestingLevel)](#apidoc.element.rethinkdbdash.term.prototype._setNestingLevel)
- description and source-code
```javascript
_setNestingLevel = function (nestingLevel) {
  Term.prototype._nestingLevel = nestingLevel;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype._toReadableStream"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_toReadableStream (connection, options)](#apidoc.element.rethinkdbdash.term.prototype._toReadableStream)
- description and source-code
```javascript
_toReadableStream = function (connection, options) {
  var stream;

  var _options = {};
  if (helper.isPlainObject(connection) && (typeof connection._isConnection === 'function') && (connection._isConnection() === true
)) {
    //toStream make sure that options is an object
    helper.loopKeys(options, function(obj, key) {
      _options[key] = obj[key];
    });
    _options.cursor = true;
    stream = new ReadableStream(_options);
    this.run(connection, _options).then(function(cursor) {
      stream._setCursor(cursor);
      return null;
    }).error(function(error) {
      stream.emit('error', error);
    });
  }
  else {
    helper.loopKeys(connection, function(obj, key) {
      _options[key] = obj[key];
    });
    _options.cursor = true;
    stream = new ReadableStream(_options);
    this.run(_options).then(function(cursor) {
      stream._setCursor(cursor);
      return null;
    }).error(function(error) {
      stream.emit('error', error);
    });
  }
  return stream;
}
```
- example usage
```shell
...

Term.prototype.toStream = function(connection, options) {
if (helper.isPlainObject(connection) && (typeof connection._isConnection === 'function') && (connection._isConnection() === true
)) {
  if (helper.isPlainObject(options) === false) {
    options = {};
  }
  if (options.readable === true) {
    return this._toReadableStream(connection, options);
  }
  else if (options.writable === true) {
    return this._toWritableStream(connection, options);
  }
  else if (options.transform === true) {
    return this._toTransformStream(connection, options);
  }
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype._toTransformStream"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_toTransformStream (connection, options)](#apidoc.element.rethinkdbdash.term.prototype._toTransformStream)
- description and source-code
```javascript
_toTransformStream = function (connection, options) {
  if (this._query[0] !== termTypes.TABLE) {
    throw new Error.ReqlDriverError('Cannot create a writable stream on something else than a table.');
  }

  if (helper.isPlainObject(connection) && (typeof connection._isConnection === 'function') && (connection._isConnection() === true
)) {
    return new TransformStream(this, options, connection);
  }
  else {
    return new TransformStream(this, connection);
  }
}
```
- example usage
```shell
...
  if (options.readable === true) {
    return this._toReadableStream(connection, options);
  }
  else if (options.writable === true) {
    return this._toWritableStream(connection, options);
  }
  else if (options.transform === true) {
    return this._toTransformStream(connection, options);
  }
  else {
    return this._toReadableStream(connection, options);
  }
}
else {
  options = connection;
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype._toWritableStream"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_toWritableStream (connection, options)](#apidoc.element.rethinkdbdash.term.prototype._toWritableStream)
- description and source-code
```javascript
_toWritableStream = function (connection, options) {
  if (this._query[0] !== termTypes.TABLE) {
    throw new Error.ReqlDriverError('Cannot create a writable stream on something else than a table.');
  }

  if (helper.isPlainObject(connection) && (typeof connection._isConnection === 'function') && (connection._isConnection() === true
)) {
    return new WritableStream(this, options, connection);
  }
  else {
    return new WritableStream(this, connection);
  }
}
```
- example usage
```shell
...
if (helper.isPlainObject(options) === false) {
  options = {};
}
if (options.readable === true) {
  return this._toReadableStream(connection, options);
}
else if (options.writable === true) {
  return this._toWritableStream(connection, options);
}
else if (options.transform === true) {
  return this._toTransformStream(connection, options);
}
else {
  return this._toReadableStream(connection, options);
}
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype._wrap"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>_wrap ()](#apidoc.element.rethinkdbdash.term.prototype._wrap)
- description and source-code
```javascript
_wrap = function () {
  var self = this;
  if (helper.hasImplicit(this._query)) {
    if (this._query[0] === termTypes.ARGS) {
      throw new Error.ReqlDriverError('Implicit variable 'r.row' cannot be used inside 'r.args'')
    }
    //Must pass at least one variable to the function or it won't accept r.row
    return new Term(this._r).expr(function(doc) { return self; })
  }
  else {
    return self;
  }
}
```
- example usage
```shell
...
  fn = undefined;
}

var term = new Term(this._r);
term._query.push(termTypes.INDEX_CREATE);
var args = [this];
args.push(new Term(this._r).expr(name));
if (typeof fn !== 'undefined') args.push(new Term(this._r).expr(fn)._wrap());
term._fillArgs(args);

if (helper.isPlainObject(options)) {
  // There is no need to translate here
  helper.loopKeys(options, function(obj, key) {
    if ((key !== 'multi') && (key !== 'geo')) {
      throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'indexCreate'', self._query, 'Available option is multi <
bool> and geo <bool>');
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.add"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>add ()](#apidoc.element.rethinkdbdash.term.prototype.add)
- description and source-code
```javascript
add = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'add', this);

  var term = new Term(this._r);
  term._query.push(termTypes.ADD)
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...
if (self._options.format === 'primaryKey') {
  query = query.do(function(result) {
    return self._r.branch(
      result('errors').eq(0),
      self._table.config()('primary_key').do(function(primaryKey) {
        return result('changes')('new_val')(primaryKey)
      }),
      result(self._r.error(result('errors').coerceTo('STRING').add(' errors returned. First error:\n').add(result('first_error'))))
    )
  })
}

query.run(self._connection).then(function(result) {
  self._inserting = false;
  if (self._options.format === 'primaryKey') {
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.and"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>and ()](#apidoc.element.rethinkdbdash.term.prototype.and)
- description and source-code
```javascript
and = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}

  var term = new Term(this._r);
  term._query.push(termTypes.AND)
  var args = [];
  if (!Array.isArray(this._query) || (this._query.length > 0)) {
    args.push(this);
  }
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.append"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>append (value)](#apidoc.element.rethinkdbdash.term.prototype.append)
- description and source-code
```javascript
append = function (value) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'append', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.APPEND)
  var args = [this, new Term(this._r).expr(value)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.april"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>april ()](#apidoc.element.rethinkdbdash.term.prototype.april)
- description and source-code
```javascript
april = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.APRIL);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.args"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>args ()](#apidoc.element.rethinkdbdash.term.prototype.args)
- description and source-code
```javascript
args = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._noPrefix(this, 'args');

  var term = new Term(this._r);
  term._query.push(termTypes.ARGS);
  var args = [];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.asc"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>asc (field)](#apidoc.element.rethinkdbdash.term.prototype.asc)
- description and source-code
```javascript
asc = function (field) {
  this._noPrefix(this, 'asc');
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'asc', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.ASC)
  var args = [new Term(this._r).expr(field)._wrap()];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.august"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>august ()](#apidoc.element.rethinkdbdash.term.prototype.august)
- description and source-code
```javascript
august = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.AUGUST);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.avg"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>avg (field)](#apidoc.element.rethinkdbdash.term.prototype.avg)
- description and source-code
```javascript
avg = function (field) {
  if (this._fastArityRange(arguments.length, 0, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 0, 1, 'avg', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.AVG)
  var args = [this];
  if (field !== undefined) {
    args.push(new Term(this._r).expr(field)._wrap())
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.between"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>between (start, end, options)](#apidoc.element.rethinkdbdash.term.prototype.between)
- description and source-code
```javascript
between = function (start, end, options) {
  var self = this;
  if (self._fastArityRange(arguments.length, 2, 3) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 2, 3, 'between', self);
  }

  var term = new Term(self._r);
  term._query.push(termTypes.BETWEEN);
  var args = [self, new Term(self._r).expr(start), new Term(self._r).expr(end)]
  term._fillArgs(args);

  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'index') && (key !== 'leftBound') && (key !== 'rightBound')){
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'between'', self._query, 'Available options are index <
string>, leftBound <string>, rightBound <string>');
      }
    });
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.binary"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>binary (bin)](#apidoc.element.rethinkdbdash.term.prototype.binary)
- description and source-code
```javascript
binary = function (bin) {
  this._noPrefix(this, 'binary');
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'binary', this);
  }

  var term;
  if (bin instanceof Buffer) {
    // We could use BINARY, and coerce 'bin' to an ASCII string, but that
    // will break if there is a null char
    term = new Term(this._r, {
      $reql_type$: 'BINARY',
      data: bin.toString('base64')
    });
  }
  else {
    term = new Term(this._r);
    term._query.push(termTypes.BINARY)
    var args = [new Term(this._r).expr(bin)];
    term._fillArgs(args);
  }
  return term;
}
```
- example usage
```shell
...

var result = {
  str: '',
  car: ''
}

if ((helper.isPlainObject(term)) && (term.$reql_type$ === 'BINARY')) {
  carify(result, 'r.binary(<Buffer>)', underline);
  return result;
}

if ((index === 0) && ((father == null) || (!nonPrefix[father[0]]))) carify(result, 'r.expr(', underline)

if (typeof term === 'string' ) {
  carify(result, '"'+term+'"', underline);
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.bracket"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>bracket (field)](#apidoc.element.rethinkdbdash.term.prototype.bracket)
- description and source-code
```javascript
bracket = function (field) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, '(...)', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.BRACKET)
  var args = [this, new Term(this._r).expr(field)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...
function Term(r, value, error) {
var self = this;
var term = function(field) {
  if (Term.prototype._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    Term.prototype._arity(_args, 1, '(...)', self);
  }
  return term.bracket(field);
}
helper.changeProto(term, self);

if (value === undefined) {
  term._query = [];
}
else {
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.branch"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>branch ()](#apidoc.element.rethinkdbdash.term.prototype.branch)
- description and source-code
```javascript
branch = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 2, Infinity, '', this);

  var term = new Term(this._r);
  term._query.push(termTypes.BRANCH)
  var args = [];
  args.push(this);
  for(var i=0; i<_len; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...
if (typeof pendingCallback === 'function') {
  pendingCallback();
}

var query = self._table.insert(cache, self._insertOptions);
if (self._options.format === 'primaryKey') {
  query = query.do(function(result) {
    return self._r.branch(
      result('errors').eq(0),
      self._table.config()('primary_key').do(function(primaryKey) {
        return result('changes')('new_val')(primaryKey)
      }),
      result(self._r.error(result('errors').coerceTo('STRING').add(' errors returned. First error:\n').add(result('first_error'))))
    )
  })
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.catch"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>catch (reject)](#apidoc.element.rethinkdbdash.term.prototype.catch)
- description and source-code
```javascript
catch = function (reject) {
  return this.run().catch(reject);
}
```
- example usage
```shell
...
'''


#### Optional 'run' with 'yield'

The 'then' and 'catch' methods are implemented on a 'Term' - returned by any methods
like 'filter', 'update' etc. They are shortcut for 'this.run().then(callback)' and
'this.run().catch(callback)'.

This means that you can 'yield' any query without calling 'run.'

'''js
var bluebird = require('bluebird');
var r = require('rethinkdbdash')();
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.ceil"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>ceil ()](#apidoc.element.rethinkdbdash.term.prototype.ceil)
- description and source-code
```javascript
ceil = function () {
  if (this._fastArityRange(arguments.length, 0, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 0, 1, 'ceil', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.CEIL)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...

// Create the settings for a given pool. Merge the global options + the servers's one.
PoolMaster.prototype.createPoolSettings = function(globalOptions, serverOptions, log) {
var settings = {};
var numServers = Array.isArray(globalOptions.servers) ? globalOptions.servers.length: 1;
helper.loopKeys(globalOptions, function(options, key) {
  if ((key === 'buffer') || (key === 'max')) {
    settings[key] = Math.ceil(options[key]/numServers);
    settings[key] = Math.ceil(options[key]/numServers);
  }
  else if (key !== 'servers') {
    settings[key] = options[key];
  }
});
if (serverOptions) {
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.changeAt"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>changeAt (index, value)](#apidoc.element.rethinkdbdash.term.prototype.changeAt)
- description and source-code
```javascript
changeAt = function (index, value) {
  if (this._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 1, 2, 'changeAt', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.CHANGE_AT);
  var args = [this];
  args.push(new Term(this._r).expr(index))
  args.push(new Term(this._r).expr(value))
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.changes"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>changes (options)](#apidoc.element.rethinkdbdash.term.prototype.changes)
- description and source-code
```javascript
changes = function (options) {
  var self = this;
  if (self._fastArityRange(arguments.length, 0, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 0, 1, 'changes', self);
  }

  var term = new Term(self._r);
  term._query.push(termTypes.CHANGES);
  var args = [self];
  term._fillArgs(args);
  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'squash') && (key !== 'includeStates') && (key !== 'includeTypes')
          && (key !== 'includeInitial') && (key !== 'includeOffsets')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'changes'', self._query,
            'Available options are squash <bool>, includeInitial <bool>, includeStates <bool>, includeOffsets <bool>, includeTypes
 <bool>');
      }
    });
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
...
}

//  Create the feed on server_status and bind the listener to the feed
PoolMaster.prototype.fetchServers = function(useSeeds) {
var self = this;
var query = self._r.db('rethinkdb').table('server_status')
    .union([SEPARATOR])
    .union(self._r.db('rethinkdb').table('server_status').changes())
// In case useSeeds is true, we rotate through all the seeds + the pool master
if (!useSeeds || self._seed === self._servers.length) {
  if (useSeeds && self._seed === self._servers.length) {
    // We increase the back off only when we went through all the seeds
    self._consecutiveFails++;
  }
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.circle"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>circle (center, radius, options)](#apidoc.element.rethinkdbdash.term.prototype.circle)
- description and source-code
```javascript
circle = function (center, radius, options) {
  var self = this;

  // Arity check is done by r.circle
  self._noPrefix(self, 'circle');
  var term = new Term(self._r);
  term._query.push(termTypes.CIRCLE);
  var args = [new Term(self._r).expr(center), new Term(self._r).expr(radius)];
  term._fillArgs(args);

  if (helper.isPlainObject(options)) {
    // There is no need to translate here
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'numVertices') && (key !== 'geoSystem') && (key !== 'unit') && (key !== 'fill')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'circle'', self._query, 'Available options are numVertices
 <number>, geoSsystem <string>, unit <string> and fill <bool>');
      }
    });
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }

  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.coerceTo"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>coerceTo (type)](#apidoc.element.rethinkdbdash.term.prototype.coerceTo)
- description and source-code
```javascript
coerceTo = function (type) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'coerceTo', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.COERCE_TO)
  var args = [this, new Term(this._r).expr(type)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...
if (self._options.format === 'primaryKey') {
  query = query.do(function(result) {
    return self._r.branch(
      result('errors').eq(0),
      self._table.config()('primary_key').do(function(primaryKey) {
        return result('changes')('new_val')(primaryKey)
      }),
      result(self._r.error(result('errors').coerceTo('STRING').add(' errors returned. First error:\n').add(result('first_error'))))
    )
  })
}

query.run(self._connection).then(function(result) {
  self._inserting = false;
  if (self._options.format === 'primaryKey') {
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.concatMap"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>concatMap (transformation)](#apidoc.element.rethinkdbdash.term.prototype.concatMap)
- description and source-code
```javascript
concatMap = function (transformation) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'concatMap', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.CONCAT_MAP);
  var args = [this];
  args.push(new Term(this._r).expr(transformation)._wrap())
  term._fillArgs(args);

  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.config"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>config ()](#apidoc.element.rethinkdbdash.term.prototype.config)
- description and source-code
```javascript
config = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'config', this);
  }
  var term = new Term(this._r);
  term._query.push(termTypes.CONFIG);
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...
}

var query = self._table.insert(cache, self._insertOptions);
if (self._options.format === 'primaryKey') {
  query = query.do(function(result) {
    return self._r.branch(
      result('errors').eq(0),
      self._table.config()('primary_key').do(function(primaryKey) {
        return result('changes')('new_val')(primaryKey)
      }),
      result(self._r.error(result('errors').coerceTo('STRING').add(' errors returned. First error:\n').add(result('first_error'))))
    )
  })
}
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.contains"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>contains ()](#apidoc.element.rethinkdbdash.term.prototype.contains)
- description and source-code
```javascript
contains = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'contains', this);

  var term = new Term(this._r);
  term._query.push(termTypes.CONTAINS)
  var args = [this._query];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i])._wrap())
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.count"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>count (filter)](#apidoc.element.rethinkdbdash.term.prototype.count)
- description and source-code
```javascript
count = function (filter) {
  if (this._fastArityRange(arguments.length, 0, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 0, 1, 'count', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.COUNT);
  var args = [];
  args.push(this);
  if (filter !== undefined) {
    args.push(new Term(this._r).expr(filter)._wrap())
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.date"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>date ()](#apidoc.element.rethinkdbdash.term.prototype.date)
- description and source-code
```javascript
date = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'date', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.DATE)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.day"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>day ()](#apidoc.element.rethinkdbdash.term.prototype.day)
- description and source-code
```javascript
day = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'day', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.DAY)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.dayOfWeek"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>dayOfWeek ()](#apidoc.element.rethinkdbdash.term.prototype.dayOfWeek)
- description and source-code
```javascript
dayOfWeek = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'dayOfWeek', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.DAY_OF_WEEK)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.dayOfYear"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>dayOfYear ()](#apidoc.element.rethinkdbdash.term.prototype.dayOfYear)
- description and source-code
```javascript
dayOfYear = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'dayOfYear', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.DAY_OF_YEAR)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.db"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>db (db)](#apidoc.element.rethinkdbdash.term.prototype.db)
- description and source-code
```javascript
db = function (db) {
  this._noPrefix(this, 'db');
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'db', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.DB)
  var args = [new Term(this._r).expr(db)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...
      carify(result, 'r.'+typeToString[term[0]]+'(', underline);
      if (Array.isArray(term[1])) {
        for(var i=0; i<term[1].length; i++) {
if (i !==0) result.str += ', ';


if ((currentFrame != null) && (currentFrame === 1)) {
  // +1 for index because it's like if there was a r.db(...) before .table(...)
  backtrace = generateBacktrace(term[1][i], i+1, term, frames, options)
}
else {
  backtrace = generateBacktrace(term[1][i], i+1, term, null, options)
}
result.str += backtrace.str;
result.car += backtrace.car
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.dbCreate"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>dbCreate (db)](#apidoc.element.rethinkdbdash.term.prototype.dbCreate)
- description and source-code
```javascript
dbCreate = function (db) {
  // Check for arity is done in r.prototype.dbCreate
  this._noPrefix(this, 'dbCreate');

  var term = new Term(this._r);
  term._query.push(termTypes.DB_CREATE);
  var args = [new Term(this._r).expr(db)._query]
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...
var tableName = util.uuid()

var query; // without '.run()'
//query = 'r.table("foo").add(1).add(1).add("hello-super-long-string").add("another-long-string").add("one-last-string").map( function
(doc) { return r.expr([1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16]).map(function(test) { return test("b").add("hello-super-long-string
").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string
").add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-
long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string").mul(test("
b")).merge({ firstName: "xxxxxx", lastName: "yyyy", email: "xxxxx@yyyy.com", phone: "xxx-xxx-xxxx" }); }).add(2).map(function(doc
) { return doc.add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add
("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string").
add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long
-string").add("one-last-string") }); })';
query = 'r.db(dbName).table(tableName).rebalance().do(function(x) { return x.add(4) })';
Promise.coroutine(function* () {
try {
  yield r.dbCreate(dbName).run();
  yield r.db(dbName).tableCreate(tableName).run();

  var result = yield eval(query).run();
  throw new Error("Should have thrown an error");
}
catch(e) {
  console.log(e.message);
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.dbDrop"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>dbDrop (db)](#apidoc.element.rethinkdbdash.term.prototype.dbDrop)
- description and source-code
```javascript
dbDrop = function (db) {
  this._noPrefix(this, 'dbDrop');

  var term = new Term(this._r);
  term._query.push(termTypes.DB_DROP);
  var args = [new Term(this._r).expr(db)._query]
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.dbList"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>dbList ()](#apidoc.element.rethinkdbdash.term.prototype.dbList)
- description and source-code
```javascript
dbList = function () {
  this._noPrefix(this, 'dbList');

  var term = new Term(this._r);
  term._query.push(termTypes.DB_LIST)
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.december"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>december ()](#apidoc.element.rethinkdbdash.term.prototype.december)
- description and source-code
```javascript
december = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.DECEMBER);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.default"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>default (expression)](#apidoc.element.rethinkdbdash.term.prototype.default)
- description and source-code
```javascript
default = function (expression) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'default', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.DEFAULT);
  var args = [this, new Term(this._r).expr(expression)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.delay"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>delay (msecs)](#apidoc.element.rethinkdbdash.term.prototype.delay)
- description and source-code
```javascript
delay = function (msecs) {
  return this.run().delay(msecs);
}
```
- example usage
```shell
...
Term.prototype.catch = function(reject) {
  return this.run().catch(reject);
}
Term.prototype.finally = function(handler) {
  return this.run().finally(handler);
}
Term.prototype.delay = function(msecs) {
  return this.run().delay(msecs);
}

Term.prototype.toString = function() {
  return Error.generateBacktrace(this._query, 0, null, [], {indent: 0, extra: 0}).str;
}

Term.prototype._wrap = function() {
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.delete"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>delete (options)](#apidoc.element.rethinkdbdash.term.prototype.delete)
- description and source-code
```javascript
delete = function (options) {
  var self = this;
  if (self._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 0, 1, 'delete', self);
  }

  var term = new Term(self._r);
  term._query.push(termTypes.DELETE);
  var args = [self];
  term._fillArgs(args);

  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'returnChanges') && (key !== 'durability')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'delete'', self._query, 'Available options are returnChanges
 <bool>, durability <string>');
      }
    });
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
...

    connection.on('error', function(error) {
// We are going to close connection, but we don't want another process to use it before
// So we remove it from the pool now (if it's inside)
self._log('Error emitted by a connection: '+JSON.stringify(error));
for(var i=0; i<self.getAvailableLength(); i++) {
  if (self._pool.get(i) === this) {
    self._pool.delete(i);
    self.emit('available-size', self._pool.getLength());
    self.emit('available-size-diff', -1);
    break;
  }
}
// We want to make sure that it's not going to try to reconnect
clearTimeout(connection.timeout);
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.deleteAt"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>deleteAt (start, end)](#apidoc.element.rethinkdbdash.term.prototype.deleteAt)
- description and source-code
```javascript
deleteAt = function (start, end) {
  if (this._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 1, 2, 'deleteAt', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.DELETE_AT);
  var args = [this, new Term(this._r).expr(start)];
  if (end !== undefined) {
    args.push(new Term(this._r).expr(end))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.desc"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>desc (field)](#apidoc.element.rethinkdbdash.term.prototype.desc)
- description and source-code
```javascript
desc = function (field) {
  this._noPrefix(this, 'desc');
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'desc', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.DESC)
  var args = [new Term(this._r).expr(field)._wrap()];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.difference"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>difference (other)](#apidoc.element.rethinkdbdash.term.prototype.difference)
- description and source-code
```javascript
difference = function (other) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'difference', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.DIFFERENCE)
  var args = [this, new Term(this._r).expr(other)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.distance"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>distance (geometry, options)](#apidoc.element.rethinkdbdash.term.prototype.distance)
- description and source-code
```javascript
distance = function (geometry, options) {
  var self = this;
  if (self._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 1, 2, 'distance', self);
  }
  var term = new Term(self._r);
  term._query.push(termTypes.DISTANCE);
  var args = [self, new Term(self._r).expr(geometry)];
  term._fillArgs(args);
  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'geoSystem') && (key !== 'unit')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'distance'', self._query, 'Available options are geoSystem
 <string>, unit <string>');
      }
    });
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.distinct"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>distinct (options)](#apidoc.element.rethinkdbdash.term.prototype.distinct)
- description and source-code
```javascript
distinct = function (options) {
  var self= this;
  if (self._fastArityRange(arguments.length, 0, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 0, 1, 'distinct', self);
  }

  var term = new Term(self._r);
  term._query.push(termTypes.DISTINCT)
  var args = [self];
  term._fillArgs(args);

  if (helper.isPlainObject(options)) {
    var keepGoing = true;
    helper.loopKeys(options, function(obj, key) {
      if ((keepGoing === true) && (key !== 'index')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'distinct'', self._query, 'Available option is index: <
string>');
        keepGoing = false;
      }
    });
    if (keepGoing === true) {
      term._query.push(new Term(self._r).expr(translateOptions(options))._query);
    }
  }

  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.div"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>div ()](#apidoc.element.rethinkdbdash.term.prototype.div)
- description and source-code
```javascript
div = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'div', this);

  var term = new Term(this._r);
  term._query.push(termTypes.DIV)
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.do"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>do ()](#apidoc.element.rethinkdbdash.term.prototype.do)
- description and source-code
```javascript
do = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'do', this);

  var term = new Term(this._r);
  term._query.push(termTypes.FUNCALL);
  var args = [new Term(this._r).expr(_args[_args.length-1])._wrap()._query];
  args.push(this);
  for(var i=0; i<_args.length-1; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...

carify(result, 'var_'+term[1][0], underline);

if (underline) result.car = result.str.replace(/./g, '^');
return result;
  },
  FUNCALL: function(term, index, father, frames, options) {
// The syntax is args[1].do(args[0])
var result = {
  str: '',
  car: ''
};
var backtrace, underline, currentFrame;

var underline = Array.isArray(frames) && (frames.length === 0);
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.downcase"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>downcase (regex)](#apidoc.element.rethinkdbdash.term.prototype.downcase)
- description and source-code
```javascript
downcase = function (regex) {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'upcase', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.DOWNCASE)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.during"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>during (left, right, options)](#apidoc.element.rethinkdbdash.term.prototype.during)
- description and source-code
```javascript
during = function (left, right, options) {
  if (this._fastArityRange(arguments.length, 2, 3) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 2, 3, 'during', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.DURING);
  var args = [];
  args.push(this);
  args.push(new Term(this._r).expr(left));
  args.push(new Term(this._r).expr(right));

  term._fillArgs(args);
  if (helper.isPlainObject(options)) {
    term._query.push(new Term(this._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.epochTime"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>epochTime (epochTime)](#apidoc.element.rethinkdbdash.term.prototype.epochTime)
- description and source-code
```javascript
epochTime = function (epochTime) {
  this._noPrefix(this, 'epochTime');

  var term = new Term(this._r);
  term._query.push(termTypes.EPOCH_TIME)
  var args = [new Term(this._r).expr(epochTime)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.eq"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>eq ()](#apidoc.element.rethinkdbdash.term.prototype.eq)
- description and source-code
```javascript
eq = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'eq', this);

  var term = new Term(this._r);
  term._query.push(termTypes.EQ)
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...
  pendingCallback();
}

var query = self._table.insert(cache, self._insertOptions);
if (self._options.format === 'primaryKey') {
  query = query.do(function(result) {
    return self._r.branch(
      result('errors').eq(0),
      self._table.config()('primary_key').do(function(primaryKey) {
        return result('changes')('new_val')(primaryKey)
      }),
      result(self._r.error(result('errors').coerceTo('STRING').add(' errors returned. First error:\n').add(result('first_error'))))
    )
  })
}
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.eqJoin"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>eqJoin (rightKey, sequence, options)](#apidoc.element.rethinkdbdash.term.prototype.eqJoin)
- description and source-code
```javascript
eqJoin = function (rightKey, sequence, options) {
  var self = this;
  if (self._fastArityRange(arguments.length, 2, 3) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 2, 3, 'eqJoin', self);
  }

  var term = new Term(self._r);
  term._query.push(termTypes.EQ_JOIN);
  var args = [self];
  args.push(new Term(self._r).expr(rightKey)._wrap());
  args.push(new Term(self._r).expr(sequence));
  term._fillArgs(args);

  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'index') && (key !== 'ordered')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'eqJoin'', self._query, 'Available options are index <
string>, ordered <boolean>');
      }
    })
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.error"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>error (reject)](#apidoc.element.rethinkdbdash.term.prototype.error)
- description and source-code
```javascript
error = function (reject) {
  return this.run().error(reject);
}
```
- example usage
```shell
...
Once you have imported the driver, you can immediately run queries,
you don't need to call 'r.connect', or pass a connection to 'run'.

'''js
var r = require('rethinkdbdash')();
r.table('users').get('orphee@gmail.com').run().then(function(user) {
  // ...
}).error(handleError)
'''

- Cursors are coerced to arrays by default

'''js
var r = require('rethinkdbdash')();
r.table('data').run().then(function(result) {
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.expr"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>expr (expression, nestingLevel)](#apidoc.element.rethinkdbdash.term.prototype.expr)
- description and source-code
```javascript
expr = function (expression, nestingLevel) {
  var self = this;
  self._noPrefix(self, 'expr');
  if (self._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 1, 2, 'expr', self);
  }

  // undefined will be caught in the last else
  var ar, obj;

  if (expression === undefined) {
    var error = 'Cannot convert 'undefined' with r.expr()';
    return new Term(self._r, expression, error);
  }

  var _nestingLevel = nestingLevel;
  if (_nestingLevel == null) {
    _nestingLevel = self._r.nestingLevel;
  }
  //if (nestingLevel == null) nestingLevel = self._r.nestingLevel;
  if (_nestingLevel < 0) throw new Error.ReqlDriverError('Nesting depth limit exceeded.\nYou probably have a circular reference
somewhere')

  if (expression instanceof Term) {
    return expression;
  }
  else if (expression instanceof Function) {
    return new Func(self._r, expression);
  }
  else if (expression instanceof Date) {
    return new Term(self._r).ISO8601(expression.toISOString())
  }
  else if (Array.isArray(expression)) {
    var term = new Term(self._r);
    term._query.push(termTypes.MAKE_ARRAY);

    var args = [];
    for(var i=0; i<expression.length; i++) {
      args.push(new Term(self._r).expr(expression[i], _nestingLevel-1))
    }
    term._fillArgs(args);
    return term;
  }
  else if (expression instanceof Buffer) {
    return self._r.binary(expression);
  }
  else if (helper.isPlainObject(expression)) {
    var term = new Term(self._r);
    var optArgs = {};
    var foundError = false;
    helper.loopKeys(expression, function(expression, key) {
      if (expression[key] !== undefined) {
        var optArg = new Term(self._r).expr(expression[key], _nestingLevel-1);
        if (optArg instanceof Term && !foundError && optArg._error != null) {
          foundError = true;
          term._error = optArg._error;
          term._frames = [key].concat(optArg._frames);
        }
        optArgs[key] = optArg._query;
      }
    });
    term._query = optArgs;
    return term;
  }
  else { // Primitive
    if (expression === null) {
      return new Term(self._r, null, expression);
    }
    else if (typeof expression === 'string') {
      return new Term(self._r, expression);
    }
    else if (typeof expression === 'number') {
      if (expression !== expression) {
        var error = 'Cannot convert 'NaN' to JSON';
        return new Term(self._r, expression, error);
      }
      else if (!isFinite(expression)) {
        var error = 'Cannot convert 'Infinity' to JSON';
        return new Term(self._r, expression, error);
      }
      return new Term(self._r, expression);
    }
    else if (typeof expression === 'boolean') {
      return new Term(self._r, expression);
    }
    else {
      self._error = new Error.ReqlDriverError('Cannot convert ''+expression+'' to datum.');
      self._frames = [];
    }
  }
  return self;
}
```
- example usage
```shell
...
#### Arrays by default, not cursors

Rethinkdbdash automatically coerce cursors to arrays. If you need a raw cursor,
you can call the 'run' command with the option '{cursor: true}' or import the
driver with '{cursor: true}'.

'''js
r.expr([1, 2, 3]).run().then(function(result) {
console.log(JSON.stringify(result)) // print [1, 2, 3]
})
'''

'''js
r.expr([1, 2, 3]).run({cursor: true}).then(function(cursor) {
cursor.toArray().then(function(result) {
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.february"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>february ()](#apidoc.element.rethinkdbdash.term.prototype.february)
- description and source-code
```javascript
february = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.FEBRUARY);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.fill"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>fill ()](#apidoc.element.rethinkdbdash.term.prototype.fill)
- description and source-code
```javascript
fill = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'fill', this);
  }
  var term = new Term(this._r);
  term._query.push(termTypes.FILL);
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.filter"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>filter (filter, options)](#apidoc.element.rethinkdbdash.term.prototype.filter)
- description and source-code
```javascript
filter = function (filter, options) {
  var self = this;
  if (self._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 1, 2, 'filter', self);
  }

  var term = new Term(self._r);
  term._query.push(termTypes.FILTER);
  var args = [self, new Term(self._r).expr(filter)._wrap()]
  term._fillArgs(args);

  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if (key !== 'default') {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'filter'', self._query, 'Available option is filter');
      }
    })
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.finally"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>finally (handler)](#apidoc.element.rethinkdbdash.term.prototype.finally)
- description and source-code
```javascript
finally = function (handler) {
  return this.run().finally(handler);
}
```
- example usage
```shell
...
}
Pool.prototype.drainLocalhost = function() {
var self = this;
// All the connections are to localhost, let's create new ones (not to localhost)
self._connectionToReplace = self._numConnections;
;
for(var i=0, numConnections=self._numConnections; i<numConnections; i++) {
  self.createConnection().finally(function() {
    self._localhostToDrain++;
    self._connectionToReplace--;
    if ((self._connectionToReplace === 0) && (self._localhostToDrain > 0)) {
      var len = self._pool.getLength();
      for(var j=0; j<len; j++) {
        if (self._localhostToDrain === 0) {
          break;
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.floor"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>floor ()](#apidoc.element.rethinkdbdash.term.prototype.floor)
- description and source-code
```javascript
floor = function () {
  if (this._fastArityRange(arguments.length, 0, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 0, 1, 'floor', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.FLOOR)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...
}

var queryStr = JSON.stringify(query);
var querySize = Buffer.byteLength(queryStr);

var buffer = new Buffer(8+4+querySize);
buffer.writeUInt32LE(token & 0xFFFFFFFF, 0)
buffer.writeUInt32LE(Math.floor(token / 0xFFFFFFFF), 4)

buffer.writeUInt32LE(querySize, 8);

buffer.write(queryStr, 12);

// noreply instead of noReply because the otpions are translated for the server
if ((!helper.isPlainObject(options)) || (options.noreply != true)) {
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.fold"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>fold (base, func, options)](#apidoc.element.rethinkdbdash.term.prototype.fold)
- description and source-code
```javascript
fold = function (base, func, options) {
  if (this._fastArityRange(arguments.length, 2, 3) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 2, 3, 'range', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.FOLD)
  var args = [this, new Term(this._r).expr(base), new Term(this._r).expr(func)._wrap()];
  term._fillArgs(args);
  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'emit') && (key !== 'finalEmit')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'fold'. Available options are emit <function>, finalEmit
 <function>');
      }
    });
    term._query.push(new Term(this._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.forEach"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>forEach (func)](#apidoc.element.rethinkdbdash.term.prototype.forEach)
- description and source-code
```javascript
forEach = function (func) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'forEach', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.FOR_EACH);
  var args = [this, new Term(this._r).expr(func)._wrap()];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.friday"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>friday ()](#apidoc.element.rethinkdbdash.term.prototype.friday)
- description and source-code
```javascript
friday = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.FRIDAY);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.ge"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>ge (other)](#apidoc.element.rethinkdbdash.term.prototype.ge)
- description and source-code
```javascript
ge = function (other) {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'ge', this);

  var term = new Term(this._r);
  term._query.push(termTypes.GE)
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.geojson"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>geojson (geometry)](#apidoc.element.rethinkdbdash.term.prototype.geojson)
- description and source-code
```javascript
geojson = function (geometry) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'geojson', this);
  }
  this._noPrefix(this, 'geojson');
  var term = new Term(this._r);
  term._query.push(termTypes.GEOJSON);
  var args = [new Term(this._r).expr(geometry)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.get"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>get (primaryKey)](#apidoc.element.rethinkdbdash.term.prototype.get)
- description and source-code
```javascript
get = function (primaryKey) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'get', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.GET);
  var args = [this, new Term(this._r).expr(primaryKey)]
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...

- Connections are managed by the driver with an efficient connection pool.
Once you have imported the driver, you can immediately run queries,
you don't need to call 'r.connect', or pass a connection to 'run'.

'''js
var r = require('rethinkdbdash')();
r.table('users').get('orphee@gmail.com').run().then(function(user) {
  // ...
}).error(handleError)
'''

- Cursors are coerced to arrays by default

'''js
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.getAll"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>getAll ()](#apidoc.element.rethinkdbdash.term.prototype.getAll)
- description and source-code
```javascript
getAll = function () {
  // We explicitly _args here, so fastArityRange is not useful
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}

  var term = new Term(this._r);
  term._query.push(termTypes.GET_ALL);

  var args = [];
  args.push(this);
  for(var i=0; i<_args.length-1; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  if ((_args.length > 0) && (helper.isPlainObject(_args[_args.length-1])) && (_args[_args.length-1].index !== undefined)) {
    term._fillArgs(args);
    term._query.push(new Term(this._r).expr(translateOptions(_args[_args.length-1]))._query);
  }
  else if (_args.length > 0) {
    args.push(new Term(this._r).expr(_args[_args.length-1]))
    term._fillArgs(args);
  } else {
    term._fillArgs(args);
  }
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.getField"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>getField (field)](#apidoc.element.rethinkdbdash.term.prototype.getField)
- description and source-code
```javascript
getField = function (field) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, '(...)', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.GET_FIELD)
  var args = [this, new Term(this._r).expr(field)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.getIntersecting"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>getIntersecting (geometry, options)](#apidoc.element.rethinkdbdash.term.prototype.getIntersecting)
- description and source-code
```javascript
getIntersecting = function (geometry, options) {
  if (this._fastArity(arguments.length, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 2, 'getIntersecting', this);
  }
  var term = new Term(this._r);
  term._query.push(termTypes.GET_INTERSECTING);
  var args = [this, new Term(this._r).expr(geometry)];
  term._fillArgs(args);
  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if (key !== 'index') {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'distance'', self._query, 'Available options are index
 <string>');
      }
    });
    term._query.push(new Term(this._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.getNearest"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>getNearest (geometry, options)](#apidoc.element.rethinkdbdash.term.prototype.getNearest)
- description and source-code
```javascript
getNearest = function (geometry, options) {
  var self = this;
  if (self._fastArity(arguments.length, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arity(_args, 2, 'getNearest', self);
  }
  var term = new Term(self._r);
  term._query.push(termTypes.GET_NEAREST);
  var args = [self, new Term(self._r).expr(geometry)];
  term._fillArgs(args);
  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'index') && (key !== 'maxResults') && (key !== 'maxDist') && (key !== 'unit') && (key !== 'geoSystem')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'getNearest'', self._query, 'Available options are index
 <string>, maxResults <number>, maxDist <number>, unit <string>, geoSystem <string>');
      }
    });
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }
  return term;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.grant"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>grant (name, access)](#apidoc.element.rethinkdbdash.term.prototype.grant)
- description and source-code
```javascript
grant = function (name, access) {
  if (this._fastArity(arguments.length, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 2, 'grant', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.GRANT)
  var args = [this, new Term(this._r).expr(name), new Term(this._r).expr(access)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.group"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>group ()](#apidoc.element.rethinkdbdash.term.prototype.group)
- description and source-code
```javascript
group = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  var self = this;
  self._arityRange(_args, 1, Infinity, 'group', self);

  var term = new Term(self._r);
  term._query.push(termTypes.GROUP);
  var args = [self];
  for(var i=0; i<_args.length-1; i++) {
    args.push(new Term(self._r).expr(_args[i])._wrap())
  }
  if (_args.length > 0) {
    if (helper.isPlainObject(_args[_args.length-1])) {
      helper.loopKeys(_args[_args.length-1], function(obj, key) {
         if ((key !== 'index')
        && (key !==  'multi')) {
          throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'group'', self._query, 'Available options are index: <
string>, multi <boolean>');
        }
      });
      term._fillArgs(args);
      term._query.push(new Term(self._r).expr(translateOptions(_args[_args.length-1]))._query);
    }
    else {
      args.push(new Term(self._r).expr(_args[_args.length-1])._wrap())
      term._fillArgs(args);
    }
  }
  else {
    term._fillArgs(args);
  }

  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.gt"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>gt (other)](#apidoc.element.rethinkdbdash.term.prototype.gt)
- description and source-code
```javascript
gt = function (other) {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'gt', this);

  var term = new Term(this._r);
  term._query.push(termTypes.GT)
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.hasFields"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>hasFields ()](#apidoc.element.rethinkdbdash.term.prototype.hasFields)
- description and source-code
```javascript
hasFields = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'hasFields', this);

  var term = new Term(this._r);
  term._query.push(termTypes.HAS_FIELDS)
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.hours"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>hours ()](#apidoc.element.rethinkdbdash.term.prototype.hours)
- description and source-code
```javascript
hours = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'hours', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.HOURS)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.http"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>http (url, options)](#apidoc.element.rethinkdbdash.term.prototype.http)
- description and source-code
```javascript
http = function (url, options) {
  this._noPrefix(this, 'http');
  if (this._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 1, 2, 'http', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.HTTP);
  var args = [new Term(this._r).expr(url)];
  term._fillArgs(args);
  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'timeout')
        && (key !==  'attempts')
        && (key !==  'redirects')
        && (key !==  'verify')
        && (key !==  'resultFormat')
        && (key !==  'method')
        && (key !==  'auth')
        && (key !==  'params')
        && (key !==  'header')
        && (key !==  'data')
        && (key !==  'page')
        && (key !==  'pageLimit')
        && (key !==  '')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'http'. Available options are attempts <number>, redirects
 <number>, verify <boolean>, resultFormat: <string>, method: <string>, auth: <object>, params: <object>, header: <string>, data: <
string>, page: <string/function>, pageLimit: <number>');
      }
    });

    term._query.push(new Term(this._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.inTimezone"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>inTimezone (timezone)](#apidoc.element.rethinkdbdash.term.prototype.inTimezone)
- description and source-code
```javascript
inTimezone = function (timezone) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'inTimezone', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.IN_TIMEZONE)
  var args = [this, new Term(this._r).expr(timezone)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.includes"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>includes (geometry)](#apidoc.element.rethinkdbdash.term.prototype.includes)
- description and source-code
```javascript
includes = function (geometry) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'includes', this);
  }
  var term = new Term(this._r);
  term._query.push(termTypes.INCLUDES);
  var args = [this, new Term(this._r).expr(geometry)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.indexCreate"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>indexCreate (name, fn, options)](#apidoc.element.rethinkdbdash.term.prototype.indexCreate)
- description and source-code
```javascript
indexCreate = function (name, fn, options) {
  if (this._fastArityRange(arguments.length, 1, 3) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 1, 3, 'indexCreate', this);
  }

  if ((options == null) && (helper.isPlainObject(fn))) {
    options = fn;
    fn = undefined;
  }

  var term = new Term(this._r);
  term._query.push(termTypes.INDEX_CREATE);
  var args = [this];
  args.push(new Term(this._r).expr(name));
  if (typeof fn !== 'undefined') args.push(new Term(this._r).expr(fn)._wrap());
  term._fillArgs(args);

  if (helper.isPlainObject(options)) {
    // There is no need to translate here
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'multi') && (key !== 'geo')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'indexCreate'', self._query, 'Available option is multi
 <bool> and geo <bool>');
      }
    });
    term._query.push(new Term(this._r).expr(options)._query);
  }
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.indexDrop"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>indexDrop (name)](#apidoc.element.rethinkdbdash.term.prototype.indexDrop)
- description and source-code
```javascript
indexDrop = function (name) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'indexDrop', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.INDEX_DROP);
  var args = [this, new Term(this._r).expr(name)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.indexList"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>indexList ()](#apidoc.element.rethinkdbdash.term.prototype.indexList)
- description and source-code
```javascript
indexList = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'indexList', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.INDEX_LIST);
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.indexRename"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>indexRename (oldName, newName, options)](#apidoc.element.rethinkdbdash.term.prototype.indexRename)
- description and source-code
```javascript
indexRename = function (oldName, newName, options) {
  var self = this;
  if (self._fastArityRange(arguments.length, 2, 3) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 2, 3, 'indexRename', self);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.INDEX_RENAME);
  var args = [this, new Term(this._r).expr(oldName), new Term(this._r).expr(newName)];
  term._fillArgs(args);

  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if (key !== 'overwrite') {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'indexRename'', self._query, 'Available options are overwrite
 <bool>');
      }
    });
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }


  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.indexStatus"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>indexStatus ()](#apidoc.element.rethinkdbdash.term.prototype.indexStatus)
- description and source-code
```javascript
indexStatus = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  var term = new Term(this._r);
  term._query.push(termTypes.INDEX_STATUS);
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.indexWait"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>indexWait ()](#apidoc.element.rethinkdbdash.term.prototype.indexWait)
- description and source-code
```javascript
indexWait = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  var term = new Term(this._r);
  term._query.push(termTypes.INDEX_WAIT);
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.indexesOf"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>indexesOf (predicate)](#apidoc.element.rethinkdbdash.term.prototype.indexesOf)
- description and source-code
```javascript
indexesOf = function (predicate) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'indexesOf', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.OFFSETS_OF)
  var args = [this, new Term(this._r).expr(predicate)._wrap()];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.info"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>info ()](#apidoc.element.rethinkdbdash.term.prototype.info)
- description and source-code
```javascript
info = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'info', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.INFO);
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.innerJoin"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>innerJoin (sequence, predicate)](#apidoc.element.rethinkdbdash.term.prototype.innerJoin)
- description and source-code
```javascript
innerJoin = function (sequence, predicate) {
  if (this._fastArity(arguments.length, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 2, 'innerJoin', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.INNER_JOIN);
  var args = [this._query];
  args.push(new Term(this._r).expr(sequence)._query);
  args.push(new Term(this._r).expr(predicate)._wrap()._query);
  term._fillArgs(args);

  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.insert"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>insert (documents, options)](#apidoc.element.rethinkdbdash.term.prototype.insert)
- description and source-code
```javascript
insert = function (documents, options) {
  var self = this;
  if (self._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 1, 2, 'insert', self);
  }

  var term = new Term(self._r);
  term._query.push(termTypes.INSERT);
  var args = [self, new Term(self._r).expr(documents)];
  term._fillArgs(args);

  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'returnChanges') && (key !== 'durability') && (key !== 'conflict')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'insert'', self._query, 'Available options are returnChanges
 <bool>, durability <string>, conflict <string>');
      }
    });
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
...

var pendingCallback = self._pendingCallback;
self._pendingCallback = null;
if (typeof pendingCallback === 'function') {
  pendingCallback();
}

var query = self._table.insert(cache, self._insertOptions);
if (self._options.format === 'primaryKey') {
  query = query.do(function(result) {
    return self._r.branch(
      result('errors').eq(0),
      self._table.config()('primary_key').do(function(primaryKey) {
        return result('changes')('new_val')(primaryKey)
      }),
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.insertAt"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>insertAt (index, value)](#apidoc.element.rethinkdbdash.term.prototype.insertAt)
- description and source-code
```javascript
insertAt = function (index, value) {
  if (this._fastArity(arguments.length, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 2, 'insertAt', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.INSERT_AT)
  var args = [this, new Term(this._r).expr(index), new Term(this._r).expr(value)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.intersects"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>intersects (geometry)](#apidoc.element.rethinkdbdash.term.prototype.intersects)
- description and source-code
```javascript
intersects = function (geometry) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'intersects', this);
  }
  var term = new Term(this._r);
  term._query.push(termTypes.INTERSECTS);
  var args = [this, new Term(this._r).expr(geometry)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>isEmpty ()](#apidoc.element.rethinkdbdash.term.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'isEmpty', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.IS_EMPTY)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.january"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>january ()](#apidoc.element.rethinkdbdash.term.prototype.january)
- description and source-code
```javascript
january = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.JANUARY);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.js"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>js (arg, options)](#apidoc.element.rethinkdbdash.term.prototype.js)
- description and source-code
```javascript
js = function (arg, options) {
  this._noPrefix(this, 'js');
  if (this._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 1, 2, 'js', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.JAVASCRIPT)
  var args = [new Term(this._r).expr(arg)];
  term._fillArgs(args);

  if (helper.isPlainObject(options)) {
    term._query.push(new Term(this._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.json"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>json (json)](#apidoc.element.rethinkdbdash.term.prototype.json)
- description and source-code
```javascript
json = function (json) {
  this._noPrefix(this, 'json');
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'info', this);
  }
<span class="apidocCodeCommentSpan">  /*
  if ((/\\u0000/.test(json)) || (/\0/.test(json))) {
    this._error = new Error.ReqlDriverError('The null character is currently not supported by RethinkDB');
  }
  */
</span>  var term = new Term(this._r);
  term._query.push(termTypes.JSON);

  var args = [new Term(this._r).expr(json)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.july"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>july ()](#apidoc.element.rethinkdbdash.term.prototype.july)
- description and source-code
```javascript
july = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.JULY);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.june"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>june ()](#apidoc.element.rethinkdbdash.term.prototype.june)
- description and source-code
```javascript
june = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.JUNE);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.keys"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>keys ()](#apidoc.element.rethinkdbdash.term.prototype.keys)
- description and source-code
```javascript
keys = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'keys', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.KEYS)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...

if ((index === 0) && ((father == null) || (!nonPrefix[father[0]]))) carify(result, 'r.expr(', underline)

if (typeof term === 'string' ) {
  carify(result, '"'+term+'"', underline);
}
else if (helper.isPlainObject(term)) {
  var totalKeys = Object.keys(term).length;
  if (totalKeys === 0) {
    carify(result, '{}', underline);
  }
  else {
    carify(result, '{\n', underline);
    var countKeys = 0;
    var extraToRemove = options.extra;
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.le"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>le (other)](#apidoc.element.rethinkdbdash.term.prototype.le)
- description and source-code
```javascript
le = function (other) {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'le', this);

  var term = new Term(this._r);
  term._query.push(termTypes.LE)
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.limit"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>limit (value)](#apidoc.element.rethinkdbdash.term.prototype.limit)
- description and source-code
```javascript
limit = function (value) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'limit', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.LIMIT)
  var args = [this, new Term(this._r).expr(value)]
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.line"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>line ()](#apidoc.element.rethinkdbdash.term.prototype.line)
- description and source-code
```javascript
line = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  // Arity check is done by r.line
  this._noPrefix(this, 'line');

  var term = new Term(this._r);
  term._query.push(termTypes.LINE);

  var args = [];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.literal"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>literal (obj)](#apidoc.element.rethinkdbdash.term.prototype.literal)
- description and source-code
```javascript
literal = function (obj) {
  this._noPrefix(this, 'literal');
  // The test for arity is performed in r.literal

  var term = new Term(this._r);
  term._query.push(termTypes.LITERAL);
  if (arguments.length > 0) {
    var args = [new Term(this._r).expr(obj)];
    term._fillArgs(args);
  }
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.lt"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>lt (other)](#apidoc.element.rethinkdbdash.term.prototype.lt)
- description and source-code
```javascript
lt = function (other) {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'lt', this);

  var term = new Term(this._r);
  term._query.push(termTypes.LT)
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.map"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>map ()](#apidoc.element.rethinkdbdash.term.prototype.map)
- description and source-code
```javascript
map = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'map', this);

  var term = new Term(this._r);
  term._query.push(termTypes.MAP);
  var args = [];
  if (!Array.isArray(this._query) || (this._query.length > 0)) {
    args.push(this);
  }
  for(var i=0; i<_args.length-1; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  // Make sure that we don't push undefined if no argument is passed to map,
  // in which case the server will handle the case and return an error.
  if (_args.length> 0) {
    args.push(new Term(this._r).expr(_args[_args.length-1])._wrap())
  }
  term._fillArgs(args);

  return term;
}
```
- example usage
```shell
...



var dbName = util.uuid()
var tableName = util.uuid()

var query; // without '.run()'
//query = 'r.table("foo").add(1).add(1).add("hello-super-long-string").add("another-long-string").add("one-last-string").map( function
(doc) { return r.expr([1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16]).map(function(test) { return test("b").add("hello-super-long-string
").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string
").add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-
long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string").mul(test("
b")).merge({ firstName: "xxxxxx", lastName: "yyyy", email: "xxxxx@yyyy.com", phone: "xxx-xxx-xxxx" }); }).add(2).map(function(doc
) { return doc.add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add
("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string").
add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long
-string").add("one-last-string") }); })';
query = 'r.db(dbName).table(tableName).rebalance().do(function(x) { return x.add(4) })';
Promise.coroutine(function* () {
  try {
yield r.dbCreate(dbName).run();
yield r.db(dbName).tableCreate(tableName).run();

var result = yield eval(query).run();
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.march"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>march ()](#apidoc.element.rethinkdbdash.term.prototype.march)
- description and source-code
```javascript
march = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.MARCH);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.match"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>match (regex)](#apidoc.element.rethinkdbdash.term.prototype.match)
- description and source-code
```javascript
match = function (regex) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'match', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.MATCH)
  var args = [this, new Term(this._r).expr(regex)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...
  }
}
else {
  if (self._closed === false) {
    if (self._stackSize <= MAX_CALL_STACK) {
      self._next().then(resolve).error(function(error) {
        if ((error.message !== 'You cannot retrieve data from a cursor that is closed.') &&
            (error.message.match(/You cannot call 'next' on a closed/) === null)) {
          reject(error);
        }
      });
    }
    else {
      setTimeout(function() {
        self._stackSize = 0;
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.max"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>max (field)](#apidoc.element.rethinkdbdash.term.prototype.max)
- description and source-code
```javascript
max = function (field) {
  if (this._fastArityRange(arguments.length, 0, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 0, 1, 'max', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.MAX)
  var args = [this];
  if (field !== undefined) {
    if (helper.isPlainObject(field)) {
      term._fillArgs(args);
      term._query.push(new Term(this._r).expr(translateOptions(field))._query);
    }
    else {
      args.push(new Term(this._r).expr(field)._wrap())
      term._fillArgs(args);
    }
  }
  else {
    term._fillArgs(args);
  }
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.maxval"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>maxval ()](#apidoc.element.rethinkdbdash.term.prototype.maxval)
- description and source-code
```javascript
maxval = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.MAXVAL);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.may"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>may ()](#apidoc.element.rethinkdbdash.term.prototype.may)
- description and source-code
```javascript
may = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.MAY);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.merge"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>merge (arg)](#apidoc.element.rethinkdbdash.term.prototype.merge)
- description and source-code
```javascript
merge = function (arg) {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'merge', this);

  var term = new Term(this._r);
  term._query.push(termTypes.MERGE)
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i])._wrap())
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...



var dbName = util.uuid()
var tableName = util.uuid()

var query; // without '.run()'
//query = 'r.table("foo").add(1).add(1).add("hello-super-long-string").add("another-long-string").add("one-last-string").map( function
(doc) { return r.expr([1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16]).map(function(test) { return test("b").add("hello-super-long-string
").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string
").add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-
long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string").mul(test("
b")).merge({ firstName: "xxxxxx", lastName: "yyyy", email: "xxxxx@yyyy.com", phone: "xxx-xxx-xxxx" }); }).add(2).map(function(doc
) { return doc.add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add
("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string").
add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long
-string").add("one-last-string") }); })';
query = 'r.db(dbName).table(tableName).rebalance().do(function(x) { return x.add(4) })';
Promise.coroutine(function* () {
  try {
yield r.dbCreate(dbName).run();
yield r.db(dbName).tableCreate(tableName).run();

var result = yield eval(query).run();
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.min"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>min (field)](#apidoc.element.rethinkdbdash.term.prototype.min)
- description and source-code
```javascript
min = function (field) {
  if (this._fastArityRange(arguments.length, 0, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 0, 1, 'min', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.MIN)
  var args = [this];
  if (field !== undefined) {
    if (helper.isPlainObject(field)) {
      term._fillArgs(args);
      term._query.push(new Term(this._r).expr(translateOptions(field))._query);
    }
    else {
      args.push(new Term(this._r).expr(field)._wrap());
      term._fillArgs(args);
    }
  }
  else {
    term._fillArgs(args);
  }
  return term;
}
```
- example usage
```shell
...
  }
  return result;
}
module.exports.splitCommaEqual = splitCommaEqual;

function xorBuffer(a, b) {
  var result = [];
  var len = Math.min(a.length, b.length)
  for(var i=0; i<len; i++) {
    result.push(a[i] ^ b[i]);
  }
  return new Buffer(result);
}
module.exports.xorBuffer = xorBuffer;
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.minutes"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>minutes ()](#apidoc.element.rethinkdbdash.term.prototype.minutes)
- description and source-code
```javascript
minutes = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'minutes', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.MINUTES)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.minval"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>minval ()](#apidoc.element.rethinkdbdash.term.prototype.minval)
- description and source-code
```javascript
minval = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.MINVAL);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.mod"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>mod (b)](#apidoc.element.rethinkdbdash.term.prototype.mod)
- description and source-code
```javascript
mod = function (b) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'mod', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.MOD)
  var args = [this, new Term(this._r).expr(b)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.monday"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>monday ()](#apidoc.element.rethinkdbdash.term.prototype.monday)
- description and source-code
```javascript
monday = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.MONDAY);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.month"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>month ()](#apidoc.element.rethinkdbdash.term.prototype.month)
- description and source-code
```javascript
month = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'month', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.MONTH)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.mul"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>mul ()](#apidoc.element.rethinkdbdash.term.prototype.mul)
- description and source-code
```javascript
mul = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'mul', this);

  var term = new Term(this._r);
  term._query.push(termTypes.MUL)
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...



var dbName = util.uuid()
var tableName = util.uuid()

var query; // without '.run()'
//query = 'r.table("foo").add(1).add(1).add("hello-super-long-string").add("another-long-string").add("one-last-string").map( function
(doc) { return r.expr([1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16]).map(function(test) { return test("b").add("hello-super-long-string
").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string
").add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-
long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string").mul(test("
b")).merge({ firstName: "xxxxxx", lastName: "yyyy", email: "xxxxx@yyyy.com", phone: "xxx-xxx-xxxx" }); }).add(2).map(function(doc
) { return doc.add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add
("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string").
add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long
-string").add("one-last-string") }); })';
query = 'r.db(dbName).table(tableName).rebalance().do(function(x) { return x.add(4) })';
Promise.coroutine(function* () {
  try {
yield r.dbCreate(dbName).run();
yield r.db(dbName).tableCreate(tableName).run();

var result = yield eval(query).run();
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.ne"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>ne ()](#apidoc.element.rethinkdbdash.term.prototype.ne)
- description and source-code
```javascript
ne = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'ne', this);

  var term = new Term(this._r);
  term._query.push(termTypes.NE)
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.not"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>not ()](#apidoc.element.rethinkdbdash.term.prototype.not)
- description and source-code
```javascript
not = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'not', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.NOT)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.november"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>november ()](#apidoc.element.rethinkdbdash.term.prototype.november)
- description and source-code
```javascript
november = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.NOVEMBER);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.now"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>now ()](#apidoc.element.rethinkdbdash.term.prototype.now)
- description and source-code
```javascript
now = function () {
  this._noPrefix(this, 'now');

  var term = new Term(this._r);
  term._query.push(termTypes.NOW)
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.nth"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>nth (value)](#apidoc.element.rethinkdbdash.term.prototype.nth)
- description and source-code
```javascript
nth = function (value) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'nth', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.NTH)
  var args = [this._query, new Term(this._r).expr(value)]
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.object"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>object ()](#apidoc.element.rethinkdbdash.term.prototype.object)
- description and source-code
```javascript
object = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._noPrefix(this, 'object');
  this._arityRange(_args, 0, Infinity, 'object', this);

  var term = new Term(this._r);
  term._query.push(termTypes.OBJECT)
  var args = [];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.october"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>october ()](#apidoc.element.rethinkdbdash.term.prototype.october)
- description and source-code
```javascript
october = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.OCTOBER);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.offsetsOf"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>offsetsOf (predicate)](#apidoc.element.rethinkdbdash.term.prototype.offsetsOf)
- description and source-code
```javascript
offsetsOf = function (predicate) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'indexesOf', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.OFFSETS_OF)
  var args = [this, new Term(this._r).expr(predicate)._wrap()];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.or"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>or ()](#apidoc.element.rethinkdbdash.term.prototype.or)
- description and source-code
```javascript
or = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}

  var term = new Term(this._r);
  term._query.push(termTypes.OR)
  var args = [];
  if (!Array.isArray(this._query) || (this._query.length > 0)) {
    args.push(this);
  }
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.orderBy"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>orderBy ()](#apidoc.element.rethinkdbdash.term.prototype.orderBy)
- description and source-code
```javascript
orderBy = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'orderBy', this);

  var term = new Term(this._r);
  term._query.push(termTypes.ORDER_BY);

  var args = [this];
  for(var i=0; i<_args.length-1; i++) {
    if ((_args[i] instanceof Term) &&
        ((_args[i]._query[0] === termTypes.DESC) || (_args[i]._query[0] === termTypes.ASC))) {
      args.push(new Term(this._r).expr(_args[i]))
    }
    else {
      args.push(new Term(this._r).expr(_args[i])._wrap())
    }
  }
  // We actually don't need to make the difference here, but...
  if ((_args.length > 0) && (helper.isPlainObject(_args[_args.length-1])) && (_args[_args.length-1].index !== undefined)) {
    term._fillArgs(args);
    term._query.push(new Term(this._r).expr(translateOptions(_args[_args.length-1]))._query);
  }
  else {
    if ((_args[_args.length-1] instanceof Term) &&
      ((_args[_args.length-1]._query[0] === termTypes.DESC) || (_args[_args.length-1]._query[0] === termTypes.ASC))) {
      args.push(new Term(this._r).expr(_args[_args.length-1]))
    }
    else {
      args.push(new Term(this._r).expr(_args[_args.length-1])._wrap())
    }
    term._fillArgs(args);
  }
  return term;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.outerJoin"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>outerJoin (sequence, predicate)](#apidoc.element.rethinkdbdash.term.prototype.outerJoin)
- description and source-code
```javascript
outerJoin = function (sequence, predicate) {
  if (this._fastArity(arguments.length, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 2, 'outerJoin', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.OUTER_JOIN);
  var args = [this];
  args.push(new Term(this._r).expr(sequence));
  args.push(new Term(this._r).expr(predicate)._wrap());
  term._fillArgs(args);

  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.pluck"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>pluck ()](#apidoc.element.rethinkdbdash.term.prototype.pluck)
- description and source-code
```javascript
pluck = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'pluck', this);

  var term = new Term(this._r);
  term._query.push(termTypes.PLUCK)
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.point"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>point (longitude, latitude)](#apidoc.element.rethinkdbdash.term.prototype.point)
- description and source-code
```javascript
point = function (longitude, latitude) {
  // Arity check is done by r.point
  this._noPrefix(this, 'point');

  var term = new Term(this._r);
  term._query.push(termTypes.POINT);
  var args = [new Term(this._r).expr(longitude), new Term(this._r).expr(latitude)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.polygon"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>polygon ()](#apidoc.element.rethinkdbdash.term.prototype.polygon)
- description and source-code
```javascript
polygon = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  // Arity check is done by r.polygon
  this._noPrefix(this, 'polygon');

  var term = new Term(this._r);
  term._query.push(termTypes.POLYGON);

  var args = [];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);

  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.polygonSub"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>polygonSub (geometry)](#apidoc.element.rethinkdbdash.term.prototype.polygonSub)
- description and source-code
```javascript
polygonSub = function (geometry) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'polygonSub', this);
  }
  var term = new Term(this._r);
  term._query.push(termTypes.POLYGON_SUB);
  var args = [this, new Term(this._r).expr(geometry)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.prepend"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>prepend (value)](#apidoc.element.rethinkdbdash.term.prototype.prepend)
- description and source-code
```javascript
prepend = function (value) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'prepend', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.PREPEND)
  var args = [this, new Term(this._r).expr(value)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.random"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>random ()](#apidoc.element.rethinkdbdash.term.prototype.random)
- description and source-code
```javascript
random = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  var self = this;
  self._noPrefix(this, 'random');
  self._arityRange(_args, 0, 3, 'random', self);

  var term = new Term(self._r);
  term._query.push(termTypes.RANDOM);

  var args = [];
  for(var i=0; i<_args.length-1; i++) {
    args.push(new Term(self._r).expr(_args[i]))
  }
  if (_args.length > 0) {
    if (helper.isPlainObject(_args[_args.length-1])) {
      helper.loopKeys(_args[_args.length-1], function(obj, key) {
        if (key !== 'float') {
          throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'random'', self._query, 'Available option is float: <
boolean>');
        }
      });
      term._fillArgs(args);
      term._query.push(new Term(self._r).expr(translateOptions(_args[_args.length-1]))._query);
    }
    else {
      args.push(new Term(self._r).expr(_args[_args.length-1]))
      term._fillArgs(args);
    }
  }
  else {
    term._fillArgs(args);
  }
  return term;
}
```
- example usage
```shell
...
     for(var i=0; i<self.options.buffer; i++) {
       if (self.getLength() < self.options.max) {
         self.createConnection();
       }
     }
   }
 }, 0);
 this.id = Math.floor(Math.random()*100000);
 this._log('Creating a pool connected to '+this.getAddress());
}

util.inherits(Pool, events.EventEmitter);
/*
* Events:
*  - draining // when 'drain' is called
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.range"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>range (start, end)](#apidoc.element.rethinkdbdash.term.prototype.range)
- description and source-code
```javascript
range = function (start, end) {
  this._noPrefix(this, 'range');
  if (this._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 1, 2, 'r.range', this);
  }
  var term = new Term(this._r);
  term._query.push(termTypes.RANGE);
  var args = [];
  args.push(new Term(this._r).expr(start));
  if (end !== undefined) {
    args.push(new Term(this._r).expr(end));
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.rebalance"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>rebalance ()](#apidoc.element.rethinkdbdash.term.prototype.rebalance)
- description and source-code
```javascript
rebalance = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'rebalance', this);
  }
  var term = new Term(this._r);
  term._query.push(termTypes.REBALANCE);
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
...


var dbName = util.uuid()
var tableName = util.uuid()

var query; // without '.run()'
//query = 'r.table("foo").add(1).add(1).add("hello-super-long-string").add("another-long-string").add("one-last-string").map( function
(doc) { return r.expr([1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16]).map(function(test) { return test("b").add("hello-super-long-string
").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string
").add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-
long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string").mul(test("
b")).merge({ firstName: "xxxxxx", lastName: "yyyy", email: "xxxxx@yyyy.com", phone: "xxx-xxx-xxxx" }); }).add(2).map(function(doc
) { return doc.add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add
("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string").
add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long
-string").add("one-last-string") }); })';
query = 'r.db(dbName).table(tableName).rebalance().do(function(x) { return x.add(4) })';
Promise.coroutine(function* () {
  try {
yield r.dbCreate(dbName).run();
yield r.db(dbName).tableCreate(tableName).run();

var result = yield eval(query).run();
throw new Error("Should have thrown an error");
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.reconfigure"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>reconfigure (config)](#apidoc.element.rethinkdbdash.term.prototype.reconfigure)
- description and source-code
```javascript
reconfigure = function (config) {
  var self = this;
  if (self._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arity(_args, 1, 'reconfigure', self);
  }
  var term = new Term(self._r);
  term._query.push(termTypes.RECONFIGURE);

  var args = [this];
  term._fillArgs(args);
  if (helper.isPlainObject(config)) {
    helper.loopKeys(config, function(obj, key) {
      if ((key !== 'shards') && (key !== 'replicas') &&
        (key !== 'dryRun') && (key !== 'primaryReplicaTag') &&
        (key !== 'nonvotingReplicaTags') && (key !== 'emergencyRepair')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'reconfigure'', self._query, 'Available options are shards
: <number>, replicas: <number>, primaryReplicaTag: <object>, dryRun <boolean>, emergencyRepair: <string>, nonvotingReplicaTags: <
array<string>>');
      }
    });
    term._query.push(new Term(self._r).expr(translateOptions(config))._query);
  }
  else {
    throw new Error.ReqlDriverError('First argument of 'reconfigure' must be an object');
  }
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.reduce"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>reduce (func)](#apidoc.element.rethinkdbdash.term.prototype.reduce)
- description and source-code
```javascript
reduce = function (func) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'reduce', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.REDUCE)
  var args = [this, new Term(this._r).expr(func)._wrap()];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.replace"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>replace (newValue, options)](#apidoc.element.rethinkdbdash.term.prototype.replace)
- description and source-code
```javascript
replace = function (newValue, options) {
  var self = this;
  if (self._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 1, 2, 'replace', self);
  }

  var term = new Term(self._r);
  term._query.push(termTypes.REPLACE);
  var args = [self, new Term(self._r).expr(newValue)._wrap()];
  term._fillArgs(args);

  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'returnChanges') && (key !== 'durability') && (key !== 'nonAtomic')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'replace'', self._query, 'Available options are returnChanges
 <bool>, durability <string>, nonAtomic <bool>');
      }
    });
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
...
  }
  else {
    carify(result, ''+term, underline);
  }

  if ((index === 0) && ((father == null) || (!nonPrefix[father[0]]))) carify(result, ')', underline);

  if (underline) result.car = result.str.replace(/./g, '^');

  return result;
},
TABLE: function(term, index, father, frames, options) {
  var result = {
    str: '',
    car: ''
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.round"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>round ()](#apidoc.element.rethinkdbdash.term.prototype.round)
- description and source-code
```javascript
round = function () {
  if (this._fastArityRange(arguments.length, 0, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 0, 1, 'round', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.ROUND)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.row"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>row ()](#apidoc.element.rethinkdbdash.term.prototype.row)
- description and source-code
```javascript
row = function () {
  this._noPrefix(this, 'row');
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'r.row', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.IMPLICIT_VAR)
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.run"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>run (connection, options, callback)](#apidoc.element.rethinkdbdash.term.prototype.run)
- description and source-code
```javascript
run = function (connection, options, callback) {
  var self = this;

  if (self._error != null) {
    var error = new Error.ReqlRuntimeError(self._error, self._query, {b: self._frames});
    return Promise.reject(error);
  }

  if (helper.isPlainObject(connection) && (typeof connection._isConnection === 'function') && (connection._isConnection() === true
)) {
    if (typeof options === 'function') {
      callback = options;
      options = {};
    }
    else {
      if (!helper.isPlainObject(options)) options = {};
    }

    if (connection._isOpen() !== true) {
      return new Promise(function(resolve, reject) {
        reject(new Error.ReqlDriverError(''run' was called with a closed connection', self._query).setOperational());
      });
    }
    var p = new Promise(function(resolve, reject) {
      var token = connection._getToken();

      var query = [protodef.Query.QueryType.START];
      query.push(self._query);

      var _options = {};
      var sendOptions = false;
      if (connection.db != null) {
        sendOptions = true;
        _options.db = self._r.db(connection.db)._query;
      }

      if (self._r.arrayLimit != null) {
        sendOptions = true;
        _options[self._translateArgs['arrayLimit']] = self._r.arrayLimit;
      };


      var keepGoing = true; // we need it just to avoir calling resolve/reject multiple times
      helper.loopKeys(options, function(options, key) {
        if (keepGoing === true) {
          if ((key === 'readMode') || (key === 'durability') || (key === 'db') ||
            (key === 'noreply') || (key === 'arrayLimit') || (key === 'profile') ||
            (key === 'minBatchRows') || (key === 'maxBatchRows') || (key === 'maxBatchBytes') ||
            (key === 'maxBatchSeconds') || (key === 'firstBatchScaledownFactor')) {

            sendOptions = true;
            if (key === 'db') {
              _options[key] = self._r.db(options[key])._query;
            }
            else if (self._translateArgs.hasOwnProperty(key)) {
              _options[self._translateArgs[key]] = new Term(self._r).expr(options[key])._query;
            }
            else {
              _options[key] = new Term(self._r).expr(options[key])._query;
            }
          }
          else if ((key !== 'timeFormat') && (key !== 'groupFormat') &&
              (key !== 'binaryFormat') && (key !== 'cursor') &&
              (key !== 'readable') && (key !== 'writable') &&
              (key !== 'transform') && (key !== 'stream') &&
              (key !== 'highWaterMark')) {
            reject(new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'run'. Available options are readMode <string>, durability
 <string>, noreply <bool>, timeFormat <string>, groupFormat: <string>, profile <bool>, binaryFormat <bool>, cursor <bool>, stream
 <bool>'));
            keepGoing = false;
          }
        }
      });

      if (keepGoing === false) {
        connection.emit('release');
        return // The promise was rejected in the loopKeys
      }

      if (sendOptions === true) {
        query.push(_options);
      }
      connection._send(query, token, resolve, reject, self._query, options);
    }).nodeify(callback);
  }
  else {
    var poolMaster = self._r.getPoolMaster(); // if self._r is defined, so is self._r.getPool()
    if (!poolMaster) {
      throw new Error.ReqlDriverError(''run' was called without a connection and no pool has been created', self._query);
    }
    else {
      if (typeof connection === 'function') {
        // run(callback);
        callback = connection;
        options = {};
      }
      else if (helper.isPlainObject(connection)) {
        // run(options[, callback])
        callback = options;
        options = connection;
      }
      else {
        options = {};
      }


      var p = new Promise(function(resolve, reject) {
        poolMaster.getConnection().then(function(connection) {
          var token = connection._getToken();
          var query = [protodef.Query.QueryType.START];
          query.push(self._query);

          var _options = {};
          var send ...
```
- example usage
```shell
...

- Connections are managed by the driver with an efficient connection pool.
Once you have imported the driver, you can immediately run queries,
you don't need to call 'r.connect', or pass a connection to 'run'.

'''js
var r = require('rethinkdbdash')();
r.table('users').get('orphee@gmail.com').run().then(function(user) {
  // ...
}).error(handleError)
'''

- Cursors are coerced to arrays by default

'''js
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.sample"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>sample (size)](#apidoc.element.rethinkdbdash.term.prototype.sample)
- description and source-code
```javascript
sample = function (size) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'sample', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.SAMPLE)
  var args = [this, new Term(this._r).expr(size)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.saturday"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>saturday ()](#apidoc.element.rethinkdbdash.term.prototype.saturday)
- description and source-code
```javascript
saturday = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.SATURDAY);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.seconds"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>seconds ()](#apidoc.element.rethinkdbdash.term.prototype.seconds)
- description and source-code
```javascript
seconds = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'seconds', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.SECONDS)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.september"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>september ()](#apidoc.element.rethinkdbdash.term.prototype.september)
- description and source-code
```javascript
september = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.SEPTEMBER);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.setDifference"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>setDifference (other)](#apidoc.element.rethinkdbdash.term.prototype.setDifference)
- description and source-code
```javascript
setDifference = function (other) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'setDifference', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.SET_DIFFERENCE)
  var args = [this, new Term(this._r).expr(other)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.setInsert"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>setInsert (other)](#apidoc.element.rethinkdbdash.term.prototype.setInsert)
- description and source-code
```javascript
setInsert = function (other) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'setInsert', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.SET_INSERT)
  var args = [this, new Term(this._r).expr(other)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.setIntersection"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>setIntersection (other)](#apidoc.element.rethinkdbdash.term.prototype.setIntersection)
- description and source-code
```javascript
setIntersection = function (other) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'setIntersection', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.SET_INTERSECTION)
  var args = [this, new Term(this._r).expr(other)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.setUnion"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>setUnion (other)](#apidoc.element.rethinkdbdash.term.prototype.setUnion)
- description and source-code
```javascript
setUnion = function (other) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'setUnion', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.SET_UNION)
  var args = [this, new Term(this._r).expr(other)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.skip"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>skip (value)](#apidoc.element.rethinkdbdash.term.prototype.skip)
- description and source-code
```javascript
skip = function (value) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'skip', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.SKIP)
  var args = [this, new Term(this._r).expr(value)]
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.slice"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>slice (start, end, options)](#apidoc.element.rethinkdbdash.term.prototype.slice)
- description and source-code
```javascript
slice = function (start, end, options) {
  if (this._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 1, 3, 'slice', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.SLICE);

  var args = [];
  args.push(this);
  args.push(new Term(this._r).expr(start));

  if ((end !== undefined) && (options !== undefined)) {
    args.push(new Term(this._r).expr(end));
    term._fillArgs(args);
    term._query.push(new Term(this._r).expr(translateOptions(options))._query);
  }
  else if ((end !== undefined) && (options === undefined)) {
    if (helper.isPlainObject(end) === false) {
      args.push(new Term(this._r).expr(end));
      term._fillArgs(args);
    }
    else {
      term._fillArgs(args);
      term._query.push(new Term(this._r).expr(translateOptions(end))._query);
    }
  }
  else { // end and options are both undefined
    term._fillArgs(args);
  }
  return term;
}
```
- example usage
```shell
...
  return;
}
self.buffer = Buffer.concat([self.buffer, buffer]);

if (self.open == false) {
  for(var i=0; i<self.buffer.length; i++) {
    if (self.buffer[i] === 0) {
      var messageServerStr = self.buffer.slice(0, i).toString();
      self.buffer = self.buffer.slice(i+1); // +1 to remove the null byte
      try {
        var messageServer = JSON.parse(messageServerStr);
      } catch(error) {
        self._abort();
        reject(new Err.ReqlDriverError('Could not parse the message sent by the server : \''+messageServerStr+'\'').setOperational
());
        return;
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.spliceAt"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>spliceAt (index, array)](#apidoc.element.rethinkdbdash.term.prototype.spliceAt)
- description and source-code
```javascript
spliceAt = function (index, array) {
  if (this._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 1, 2, 'spliceAt', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.SPLICE_AT)
  var args = [this, new Term(this._r).expr(index), new Term(this._r).expr(array)];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.split"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>split (separator, max)](#apidoc.element.rethinkdbdash.term.prototype.split)
- description and source-code
```javascript
split = function (separator, max) {
  if (this._fastArityRange(arguments.length, 0, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 0, 2, 'split', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.SPLIT)
  var args = [this];
  if (separator !== undefined) {
    args.push(new Term(this._r).expr(separator))
    if (max !== undefined) {
      args.push(new Term(this._r).expr(max))
    }
  }
  term._fillArgs(args);

  return term;
}
```
- example usage
```shell
...

frames = frames.b;
if (frames) this.frames = frames.slice(0);
//this.frames = JSON.stringify(frames, null, 2);

var backtrace = generateBacktrace(query, 0, null, frames, {indent: 0, extra: 0});

var queryLines = backtrace.str.split('\n');
var carrotLines = backtrace.car.split('\n');

for(var i=0; i<queryLines.length; i++) {
  this.message += queryLines[i]+'\n';
  if (carrotLines[i].match(/\^/)) {
    var pos = queryLines[i].match(/[^\s]/);
    if ((pos) && (pos.index)) {
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.status"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>status ()](#apidoc.element.rethinkdbdash.term.prototype.status)
- description and source-code
```javascript
status = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'status', this);
  }
  var term = new Term(this._r);
  term._query.push(termTypes.STATUS);
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.sub"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>sub ()](#apidoc.element.rethinkdbdash.term.prototype.sub)
- description and source-code
```javascript
sub = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'sub', this);

  var term = new Term(this._r);
  term._query.push(termTypes.SUB)
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.sum"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>sum (field)](#apidoc.element.rethinkdbdash.term.prototype.sum)
- description and source-code
```javascript
sum = function (field) {
  if (this._fastArityRange(arguments.length, 0, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arityRange(_args, 0, 1, 'sum', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.SUM);
  var args = [this];
  if (field !== undefined) {
    args.push(new Term(this._r).expr(field)._wrap())
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.sunday"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>sunday ()](#apidoc.element.rethinkdbdash.term.prototype.sunday)
- description and source-code
```javascript
sunday = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.SUNDAY);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.sync"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>sync ()](#apidoc.element.rethinkdbdash.term.prototype.sync)
- description and source-code
```javascript
sync = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'sync', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.SYNC)
  var args = [this._query];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.table"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>table (table, options)](#apidoc.element.rethinkdbdash.term.prototype.table)
- description and source-code
```javascript
table = function (table, options) {
  var self = this;
  if (self._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 1, 2, 'table', self);
  }

  var term = new Term(self._r);
  term._query.push(termTypes.TABLE)

  var args = [];
  if (Array.isArray(self._query) && (self._query.length > 0)) {
    args.push(self);
  }
  args.push(new Term(self._r).expr(table))
  term._fillArgs(args);

  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if (key !== 'readMode') {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'table'', self._query, 'Available option is readMode <
string>');
      }
    });
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
...

- Connections are managed by the driver with an efficient connection pool.
Once you have imported the driver, you can immediately run queries,
you don't need to call 'r.connect', or pass a connection to 'run'.

'''js
var r = require('rethinkdbdash')();
r.table('users').get('orphee@gmail.com').run().then(function(user) {
  // ...
}).error(handleError)
'''

- Cursors are coerced to arrays by default

'''js
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.tableCreate"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>tableCreate (table, options)](#apidoc.element.rethinkdbdash.term.prototype.tableCreate)
- description and source-code
```javascript
tableCreate = function (table, options) {
  var self = this;
  if (self._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 1, 2, 'tableCreate', self);
  }


  var term = new Term(self._r);
  term._query.push(termTypes.TABLE_CREATE)

  var args = [];
  if (Array.isArray(self._query) && (self._query.length > 0)) {
    args.push(self); // Push db
  }
  args.push(new Term(self._r).expr(table))
  term._fillArgs(args);

  if (helper.isPlainObject(options)) {
    // Check for non valid key
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'primaryKey')
          && (key !== 'durability')
          && (key !== 'shards')
          && (key !== 'replicas')
          && (key !== 'primaryReplicaTag')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'tableCreate'', self._query, 'Available options are primaryKey
 <string>, durability <string>, shards <number>, replicas <number/object>, primaryReplicaTag <object>');
      }
    });
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
...

var query; // without '.run()'
//query = 'r.table("foo").add(1).add(1).add("hello-super-long-string").add("another-long-string").add("one-last-string").map( function
(doc) { return r.expr([1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16]).map(function(test) { return test("b").add("hello-super-long-string
").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string
").add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-
long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string").mul(test("
b")).merge({ firstName: "xxxxxx", lastName: "yyyy", email: "xxxxx@yyyy.com", phone: "xxx-xxx-xxxx" }); }).add(2).map(function(doc
) { return doc.add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add
("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string").
add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long
-string").add("one-last-string") }); })';
query = 'r.db(dbName).table(tableName).rebalance().do(function(x) { return x.add(4) })';
Promise.coroutine(function* () {
try {
  yield r.dbCreate(dbName).run();
  yield r.db(dbName).tableCreate(tableName).run();

  var result = yield eval(query).run();
  throw new Error("Should have thrown an error");
}
catch(e) {
  console.log(e.message);
  console.log('')
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.tableDrop"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>tableDrop (table)](#apidoc.element.rethinkdbdash.term.prototype.tableDrop)
- description and source-code
```javascript
tableDrop = function (table) {
  if (this._fastArity(arguments.length, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 1, 'tableDrop', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.TABLE_DROP)

  var args = [];
  if (!Array.isArray(this._query) || (this._query.length > 0)) {
    args.push(this); // push db
  }
  args.push(new Term(this._r).expr(table))
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.tableList"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>tableList ()](#apidoc.element.rethinkdbdash.term.prototype.tableList)
- description and source-code
```javascript
tableList = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'tableList', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.TABLE_LIST);

  var args = [];
  if (!Array.isArray(this._query) || (this._query.length > 0)) {
    args.push(this);
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.then"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>then (resolve, reject)](#apidoc.element.rethinkdbdash.term.prototype.then)
- description and source-code
```javascript
then = function (resolve, reject) {
  return this.run().then(resolve, reject);
}
```
- example usage
```shell
...

- Connections are managed by the driver with an efficient connection pool.
Once you have imported the driver, you can immediately run queries,
you don't need to call 'r.connect', or pass a connection to 'run'.

'''js
var r = require('rethinkdbdash')();
r.table('users').get('orphee@gmail.com').run().then(function(user) {
  // ...
}).error(handleError)
'''

- Cursors are coerced to arrays by default

'''js
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.thursday"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>thursday ()](#apidoc.element.rethinkdbdash.term.prototype.thursday)
- description and source-code
```javascript
thursday = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.THURSDAY);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.time"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>time ()](#apidoc.element.rethinkdbdash.term.prototype.time)
- description and source-code
```javascript
time = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._noPrefix(this, 'time');
  // Special check for arity
  var foundArgs = false;
  for(var i=0; i<_args.length; i++) {
    if ((_args[i] instanceof Term) && (_args[i]._query[0] === termTypes.ARGS)) {
      foundArgs = true;
      break;
    }
  }
  if (foundArgs === false) {
    if ((_args.length !== 4) && (_args.length !== 7)) {
      throw new Error.ReqlDriverError(''r.time' called with '+_args.length+' argument'+((_args.length>1)?'s':''), null, ''r.time
' takes 4 or 7 arguments');
    }
  }

  var term = new Term(this._r);
  term._query.push(termTypes.TIME)
  var args = [];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.timeOfDay"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>timeOfDay ()](#apidoc.element.rethinkdbdash.term.prototype.timeOfDay)
- description and source-code
```javascript
timeOfDay = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'timeOfDay', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.TIME_OF_DAY)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.timezone"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>timezone ()](#apidoc.element.rethinkdbdash.term.prototype.timezone)
- description and source-code
```javascript
timezone = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'timezone', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.TIMEZONE)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.toEpochTime"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>toEpochTime ()](#apidoc.element.rethinkdbdash.term.prototype.toEpochTime)
- description and source-code
```javascript
toEpochTime = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'toEpochTime', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.TO_EPOCH_TIME)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.toGeojson"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>toGeojson ()](#apidoc.element.rethinkdbdash.term.prototype.toGeojson)
- description and source-code
```javascript
toGeojson = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'toGeojson', this);
  }
  var term = new Term(this._r);
  term._query.push(termTypes.TO_GEOJSON);
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.toISO8601"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>toISO8601 ()](#apidoc.element.rethinkdbdash.term.prototype.toISO8601)
- description and source-code
```javascript
toISO8601 = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'toISO8601', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.TO_ISO8601)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>toJSON ()](#apidoc.element.rethinkdbdash.term.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'toJSON', this);
  }
  var term = new Term(this._r);
  term._query.push(termTypes.TO_JSON_STRING);
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.toJsonString"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>toJsonString ()](#apidoc.element.rethinkdbdash.term.prototype.toJsonString)
- description and source-code
```javascript
toJsonString = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'toJSON', this);
  }
  var term = new Term(this._r);
  term._query.push(termTypes.TO_JSON_STRING);
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.toStream"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>toStream (connection, options)](#apidoc.element.rethinkdbdash.term.prototype.toStream)
- description and source-code
```javascript
toStream = function (connection, options) {
  if (helper.isPlainObject(connection) && (typeof connection._isConnection === 'function') && (connection._isConnection() === true
)) {
    if (helper.isPlainObject(options) === false) {
      options = {};
    }
    if (options.readable === true) {
      return this._toReadableStream(connection, options);
    }
    else if (options.writable === true) {
      return this._toWritableStream(connection, options);
    }
    else if (options.transform === true) {
      return this._toTransformStream(connection, options);
    }
    else {
      return this._toReadableStream(connection, options);
    }
  }
  else {
    options = connection;
    if (helper.isPlainObject(options) === false) {
      options = {};
    }
    if (options.readable === true) {
      return this._toReadableStream(options);
    }
    else if (options.writable === true) {
      return this._toWritableStream(options);
    }
    else if (options.transform === true) {
      return this._toTransformStream(options);
    }
    else {
      return this._toReadableStream(options);
    }
  }
}
```
- example usage
```shell
...
synchronously returned with the 'toStream([connection])' method.

'''js
var fs = require('fs');
var file = fs.createWriteStream('file.txt');

var r = require('rethinkdbdash')();
r.table('users').toStream()
  .on('error', console.log)
  .pipe(file)
  .on('error', console.log)
  .on('end', function() {
    r.getPool().drain();
  });
'''
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.toString"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>toString ()](#apidoc.element.rethinkdbdash.term.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return Error.generateBacktrace(this._query, 0, null, [], {indent: 0, extra: 0}).str;
}
```
- example usage
```shell
...
self.connection.on('error', function(error) {
  self.emit('error', error);
});

var versionBuffer = new Buffer(4)
versionBuffer.writeUInt32LE(protodef.VersionDummy.Version.V1_0, 0)

self.randomString = new Buffer(crypto.randomBytes(18)).toString('base64')
var authBuffer = new Buffer(JSON.stringify({
  protocol_version: PROTOCOL_VERSION,
  authentication_method: AUTHENTIFICATION_METHOD,
  authentication: "n,,n=" + self.user + ",r=" + self.randomString
}));

helper.tryCatch(function() {
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.tuesday"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>tuesday ()](#apidoc.element.rethinkdbdash.term.prototype.tuesday)
- description and source-code
```javascript
tuesday = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.TUESDAY);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.typeOf"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>typeOf ()](#apidoc.element.rethinkdbdash.term.prototype.typeOf)
- description and source-code
```javascript
typeOf = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'typeOf', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.TYPE_OF);
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.ungroup"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>ungroup ()](#apidoc.element.rethinkdbdash.term.prototype.ungroup)
- description and source-code
```javascript
ungroup = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'ungroup', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.UNGROUP)
  var args = [this._query];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.union"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>union ()](#apidoc.element.rethinkdbdash.term.prototype.union)
- description and source-code
```javascript
union = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}

  var term = new Term(this._r);
  term._query.push(termTypes.UNION)
  var args = [];
  if (!Array.isArray(this._query) || (this._query.length > 0)) {
    args.push(this);
  }
  for(var i=0; i<_args.length-1; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  if ((_args.length > 1) && (helper.isPlainObject(_args[_args.length-1])) && (_args[_args.length-1].interleave !== undefined)) {
    term._fillArgs(args);
    term._query.push(new Term(this._r).expr(translateOptions(_args[_args.length-1]))._query);
  }
  else if (_args.length > 0) {
    args.push(new Term(this._r).expr(_args[_args.length-1]))
    term._fillArgs(args);
  }
  return term;
}
```
- example usage
```shell
...
self.resetBufferParameters();
}

//  Create the feed on server_status and bind the listener to the feed
PoolMaster.prototype.fetchServers = function(useSeeds) {
var self = this;
var query = self._r.db('rethinkdb').table('server_status')
    .union([SEPARATOR])
    .union(self._r.db('rethinkdb').table('server_status').changes())
// In case useSeeds is true, we rotate through all the seeds + the pool master
if (!useSeeds || self._seed === self._servers.length) {
  if (useSeeds && self._seed === self._servers.length) {
    // We increase the back off only when we went through all the seeds
    self._consecutiveFails++;
  }
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.upcase"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>upcase (regex)](#apidoc.element.rethinkdbdash.term.prototype.upcase)
- description and source-code
```javascript
upcase = function (regex) {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'upcase', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.UPCASE)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.update"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>update (newValue, options)](#apidoc.element.rethinkdbdash.term.prototype.update)
- description and source-code
```javascript
update = function (newValue, options) {
  var self = this;
  if (self._fastArityRange(arguments.length, 1, 2) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 1, 2, 'update', self);
  }

  var term = new Term(self._r);
  term._query.push(termTypes.UPDATE);
  var args = [self, new Term(self._r).expr(newValue)._wrap()];
  term._fillArgs(args);

  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'returnChanges') && (key !== 'durability') && (key !== 'nonAtomic')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'update'', self._query, 'Available options are returnChanges
 <bool>, durability <string>, nonAtomic <bool>');
      }
    });
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }
  return term;
}
```
- example usage
```shell
...

'''js
var bluebird = require('bluebird');
var r = require('rethinkdbdash')();

bluebird.coroutine(function*() {
  try {
    var result = yield r.table('users').get('orphee@gmail.com').update({name: 'Michel'});
    assert.equal(result.errors, 0);
  } catch(err) {
    console.log(err);
  }
});
'''
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.uuid"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>uuid (str)](#apidoc.element.rethinkdbdash.term.prototype.uuid)
- description and source-code
```javascript
uuid = function (str) {
  this._noPrefix(this, 'uuid');

  var term = new Term(this._r);
  term._query.push(termTypes.UUID)

  if (str !== undefined) {
    var args = [new Term(this._r).expr(str)];
    term._fillArgs(args);
  }
  return term;
}
```
- example usage
```shell
...
var r = require(__dirname+'/../lib')(config);
var util = require(__dirname+'/../test/util/common.js');
var assert = require('assert');




var dbName = util.uuid()
var tableName = util.uuid()

var query; // without '.run()'
//query = 'r.table("foo").add(1).add(1).add("hello-super-long-string").add("another-long-string").add("one-last-string").map( function
(doc) { return r.expr([1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16]).map(function(test) { return test("b").add("hello-super-long-string
").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string
").add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-
long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string").mul(test("
b")).merge({ firstName: "xxxxxx", lastName: "yyyy", email: "xxxxx@yyyy.com", phone: "xxx-xxx-xxxx" }); }).add(2).map(function(doc
) { return doc.add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add
("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long-string").add("one-last-string").
add("hello-super-long-string").add("another-long-string").add("one-last-string").add("hello-super-long-string").add("another-long
-string").add("one-last-string") }); })';
query = 'r.db(dbName).table(tableName).rebalance().do(function(x) { return x.add(4) })';
Promise.coroutine(function* () {
try {
...
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.values"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>values ()](#apidoc.element.rethinkdbdash.term.prototype.values)
- description and source-code
```javascript
values = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'keys', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.VALUES)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.wait"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>wait (options)](#apidoc.element.rethinkdbdash.term.prototype.wait)
- description and source-code
```javascript
wait = function (options) {
  var self = this;
  if (self._fastArityRange(arguments.length, 0, 1) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    self._arityRange(_args, 0, 1, 'wait', self);
  }
  var term = new Term(self._r);
  term._query.push(termTypes.WAIT);
  var args = [self];
  term._fillArgs(args);
  if (helper.isPlainObject(options)) {
    helper.loopKeys(options, function(obj, key) {
      if ((key !== 'waitFor') && (key !== 'timeout')) {
        throw new Error.ReqlDriverError('Unrecognized option ''+key+'' in 'wait'', self._query, 'Available options are waitFor: <
string>, timeout: <number>');
      }
    });
    term._query.push(new Term(self._r).expr(translateOptions(options))._query);
  }

  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.wednesday"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>wednesday ()](#apidoc.element.rethinkdbdash.term.prototype.wednesday)
- description and source-code
```javascript
wednesday = function () {
  var term = new Term(this._r);
  term._query.push(termTypes.WEDNESDAY);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.withFields"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>withFields ()](#apidoc.element.rethinkdbdash.term.prototype.withFields)
- description and source-code
```javascript
withFields = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'withFields', this);

  var term = new Term(this._r);
  term._query.push(termTypes.WITH_FIELDS);
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);

  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.without"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>without ()](#apidoc.element.rethinkdbdash.term.prototype.without)
- description and source-code
```javascript
without = function () {
  var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
  this._arityRange(_args, 1, Infinity, 'without', this);

  var term = new Term(this._r);
  term._query.push(termTypes.WITHOUT)
  var args = [this];
  for(var i=0; i<_args.length; i++) {
    args.push(new Term(this._r).expr(_args[i]))
  }
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.year"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>year ()](#apidoc.element.rethinkdbdash.term.prototype.year)
- description and source-code
```javascript
year = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'year', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.YEAR)
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.term.prototype.zip"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.term.prototype.</span>zip ()](#apidoc.element.rethinkdbdash.term.prototype.zip)
- description and source-code
```javascript
zip = function () {
  if (this._fastArity(arguments.length, 0) === false) {
    var _len = arguments.length;var _args = new Array(_len); for(var _i = 0; _i < _len; _i++) {_args[_i] = arguments[_i];}
    this._arity(_args, 0, 'zip', this);
  }

  var term = new Term(this._r);
  term._query.push(termTypes.ZIP);
  var args = [this];
  term._fillArgs(args);
  return term;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.transform_stream"></a>[module rethinkdbdash.transform_stream](#apidoc.module.rethinkdbdash.transform_stream)

#### <a name="apidoc.element.rethinkdbdash.transform_stream.transform_stream"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>transform_stream (table, options, connection)](#apidoc.element.rethinkdbdash.transform_stream.transform_stream)
- description and source-code
```javascript
function TransformStream(table, options, connection) {
  this._table = table;
  this._r = table._r;
  this._options = options;
  this._cache = [];
  this._pendingCallback = null;
  this._ended = false;
  this._inserting = false;
  this._delayed = false;
  this._connection = connection;
  this._highWaterMark = options.highWaterMark || 100;
  this._insertOptions = {};
  this._insertOptions.durability = options.durability || 'hard';
  this._insertOptions.conflict = options.conflict || 'error';
  this._insertOptions.returnChanges = options.returnChanges || true;

  // Internal option to run some tests
  if (options.debug === true) {
    this._sequence = [];
  }

  Transform.call(this, {
    objectMode: true,
    highWaterMark: this._highWaterMark
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.transform_stream.super_"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.transform_stream.</span>super_ (options)](#apidoc.element.rethinkdbdash.transform_stream.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform))
    return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function')
      this._transform = options.transform;

    if (typeof options.flush === 'function')
      this._flush = options.flush;
  }

  // When the writable side finishes, then flush out anything remaining.
  this.once('prefinish', function() {
    if (typeof this._flush === 'function')
      this._flush(function(er) {
        done(stream, er);
      });
    else
      done(stream);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.transform_stream.prototype"></a>[module rethinkdbdash.transform_stream.prototype](#apidoc.module.rethinkdbdash.transform_stream.prototype)

#### <a name="apidoc.element.rethinkdbdash.transform_stream.prototype._flush"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.transform_stream.prototype.</span>_flush (done)](#apidoc.element.rethinkdbdash.transform_stream.prototype._flush)
- description and source-code
```javascript
_flush = function (done) {
  this._ended = true;
  if ((this._cache.length === 0) && (this._inserting === false)) {
    done();
  }
  else { // this._inserting === true
    if (this._inserting === false) {
      this._flushCallback = done;
      this._insert();
    }
    else {
      this._flushCallback = done;
    }
  }
}
```
- example usage
```shell
...
  reject(new Err.ReqlDriverError('Failed to connect to '+self.host+':'+self.port+' in less than '+self.timeoutConnect+'s').setOperational
());
}, self.timeoutConnect*1000);

self.connection.on('end', function() {
  self.open = false;
  self.emit('end');
  // We got a FIN packet, so we'll just flush
  self._flush();
});
self.connection.on('close', function() {
  // We emit end or close just once
  clearTimeout(self.timeoutOpen)
  clearInterval(self.pingIntervalId);
  self.connection.removeAllListeners();
  self.open = false;
...
```

#### <a name="apidoc.element.rethinkdbdash.transform_stream.prototype._insert"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.transform_stream.prototype.</span>_insert ()](#apidoc.element.rethinkdbdash.transform_stream.prototype._insert)
- description and source-code
```javascript
_insert = function () {
  var self = this;
  self._inserting = true;

  var cache = self._cache;
  self._cache = [];

  if (Array.isArray(self._sequence)) {
    self._sequence.push(cache.length);
  }

  var pendingCallback = self._pendingCallback;
  self._pendingCallback = null;
  if (typeof pendingCallback === 'function') {
    pendingCallback();
  }

  var query = self._table.insert(cache, self._insertOptions);
  if (self._options.format === 'primaryKey') {
    query = query.do(function(result) {
      return self._r.branch(
        result('errors').eq(0),
        self._table.config()('primary_key').do(function(primaryKey) {
          return result('changes')('new_val')(primaryKey)
        }),
        result(self._r.error(result('errors').coerceTo('STRING').add(' errors returned. First error:\n').add(result('first_error
'))))
      )
    })
  }

  query.run(self._connection).then(function(result) {
    self._inserting = false;
    if (self._options.format === 'primaryKey') {
      for(var i=0; i<result.length; i++) {
        self.push(result[i]);
      }
    }
    else {
      if (result.errors > 0) {
        self._inserting = false;
        self.emit('error', new Error('Failed to insert some documents:'+JSON.stringify(result, null, 2)));
      }
      else {
        if (self._insertOptions.returnChanges === true) {
          for(var i=0; i<result.changes.length; i++) {
            self.push(result.changes[i].new_val);
          }
        }
      }
    }

    pendingCallback = self._pendingCallback
    self._pendingCallback = null;
    if (typeof pendingCallback === 'function') {
      // Mean that we can buffer more
      pendingCallback();
    }
    else if (self._ended !== true) {
      if (((((self._writableState.lastBufferedRequest === null) ||
          self._writableState.lastBufferedRequest.chunk === self._cache[self._cache.length-1])))
        && (self._cache.length > 0)) {
          self._insert();
      }
    }
    else if (self._ended === true) {
      if (self._cache.length > 0) {
        self._insert();
      }
      else {
        if (typeof self._flushCallback === 'function') {
          self._flushCallback();
        }
        self.push(null);
      }
    }
  }).error(function(error) {
    self._inserting = false;
    self.emit('error', error);
  });
}
```
- example usage
```shell
...
  done();
}
else {
  if (this._inserting === false) {
    if (this._delayed === true) {
      // We have to flush
      this._delayed = false;
      this._insert();
      // Fill the buffer while we are inserting data
      done();
    }
    else {
      var self = this;
      this._delayed = true;
      setImmediate(function() {
...
```

#### <a name="apidoc.element.rethinkdbdash.transform_stream.prototype._next"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.transform_stream.prototype.</span>_next (value, encoding, done)](#apidoc.element.rethinkdbdash.transform_stream.prototype._next)
- description and source-code
```javascript
_next = function (value, encoding, done) {
  if ((this._writableState.lastBufferedRequest != null) && (this._writableState.lastBufferedRequest.chunk !== value)) {
    // There's more data to buffer
    if (this._cache.length < this._highWaterMark) {
      this._delayed = false;
      // Call done now, and more data will be put in the cache
      done();
    }
    else {
      if (this._inserting === false) {
        if (this._delayed === true) {
          // We have to flush
          this._delayed = false;
          this._insert();
          // Fill the buffer while we are inserting data
          done();
        }
        else {
          var self = this;
          this._delayed = true;
          setImmediate(function() {
            self._next(value, encoding, done);
          })
        }

      }
      else {
        // to call when we are dong inserting to keep buffering
        this._pendingCallback = done;
      }
    }
  }
  else { // We just pushed the last element in the internal buffer
    if (this._inserting === false) {
      if (this._delayed === true) {
        this._delayed = false;
        // to call when we are dong inserting to maybe flag the end
        this._insert();
        // We can call done now, because we have _flush to close the stream
        done();
      }
      else {
        var self = this;
        this._delayed = true;
        setImmediate(function() {
          self._next(value, encoding, done);
        })
      }
    }
    else {
      this._delayed = false;
      // There is nothing left in the internal buffer
      // But something is already inserting stuff.
      if (this._cache.length < this._highWaterMark-1) {
        // Call done, to attempt to buffer more
        // This may trigger _flush
        //this._pendingCallback = done;
        done();
      }
      else {
        this._pendingCallback = done;
      }
    }
  }
}
```
- example usage
```shell
...
  if (typeof onFinish === 'function') {
    onFinish();
  }
}
else {
  if (self._closed === false) {
    if (self._stackSize <= MAX_CALL_STACK) {
      self._next().then(resolve).error(function(error) {
        if ((error.message !== 'You cannot retrieve data from a cursor that is closed.') &&
            (error.message.match(/You cannot call 'next' on a closed/) === null)) {
          reject(error);
        }
      });
    }
    else {
...
```

#### <a name="apidoc.element.rethinkdbdash.transform_stream.prototype._transform"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.transform_stream.prototype.</span>_transform (value, encoding, done)](#apidoc.element.rethinkdbdash.transform_stream.prototype._transform)
- description and source-code
```javascript
_transform = function (value, encoding, done) {
  this._cache.push(value);
  this._next(value, encoding, done);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.writable_stream"></a>[module rethinkdbdash.writable_stream](#apidoc.module.rethinkdbdash.writable_stream)

#### <a name="apidoc.element.rethinkdbdash.writable_stream.writable_stream"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.</span>writable_stream (table, options, connection)](#apidoc.element.rethinkdbdash.writable_stream.writable_stream)
- description and source-code
```javascript
function WritableStream(table, options, connection) {
  this._table = table;
  this._options = options;
  this._cache = [];
  this._pendingCallback = null;
  this._inserting = false;
  this._delayed = false;
  this._connection = connection;
  this._highWaterMark = options.highWaterMark || 100;

  this._insertOptions = {};
  this._insertOptions.durability = options.durability || 'hard';
  this._insertOptions.conflict = options.conflict || 'error';

  // Internal option to run some tests
  if (options.debug === true) {
    this._sequence = [];
  }

  Writable.call(this, {
    objectMode: true,
    highWaterMark: this._highWaterMark
  });
  this._i = 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.rethinkdbdash.writable_stream.super_"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.writable_stream.</span>super_ (options)](#apidoc.element.rethinkdbdash.writable_stream.super_)
- description and source-code
```javascript
function Writable(options) {
  // Writable ctor is applied to Duplexes, too.
  // 'realHasInstance' is necessary because using plain 'instanceof'
  // would return false, as no '_writableState' property is attached.

  // Trying to use the custom 'instanceof' for Writable here will also break the
  // Node.js LazyTransform implementation, which has a non-trivial getter for
  // '_writableState' that would lead to infinite recursion.
  if (!(realHasInstance.call(Writable, this)) &&
      !(this instanceof Stream.Duplex)) {
    return new Writable(options);
  }

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  if (options) {
    if (typeof options.write === 'function')
      this._write = options.write;

    if (typeof options.writev === 'function')
      this._writev = options.writev;
  }

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.rethinkdbdash.writable_stream.prototype"></a>[module rethinkdbdash.writable_stream.prototype](#apidoc.module.rethinkdbdash.writable_stream.prototype)

#### <a name="apidoc.element.rethinkdbdash.writable_stream.prototype._insert"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.writable_stream.prototype.</span>_insert ()](#apidoc.element.rethinkdbdash.writable_stream.prototype._insert)
- description and source-code
```javascript
_insert = function () {
  var self = this;
  self._inserting = true;

  var cache = self._cache;
  self._cache = [];

  if (Array.isArray(self._sequence)) {
    self._sequence.push(cache.length);
  }

  self._table.insert(cache, self._insertOptions).run(self._connection).then(function(result) {
    self._inserting = false;
    if (result.errors > 0) {
      self._inserting = false;
      self.emit('error', new Error('Failed to insert some documents:'+JSON.stringify(result, null, 2)));
    }
    if (typeof self._pendingCallback === 'function') {
      var pendingCallback = self._pendingCallback;
      self._pendingCallback = null;
      pendingCallback();
    }
    return null;
  }).error(function(error) {
    self._inserting = false;
    self.emit('error', error);
  });
}
```
- example usage
```shell
...
  done();
}
else {
  if (this._inserting === false) {
    if (this._delayed === true) {
      // We have to flush
      this._delayed = false;
      this._insert();
      // Fill the buffer while we are inserting data
      done();
    }
    else {
      var self = this;
      this._delayed = true;
      setImmediate(function() {
...
```

#### <a name="apidoc.element.rethinkdbdash.writable_stream.prototype._next"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.writable_stream.prototype.</span>_next (value, encoding, done)](#apidoc.element.rethinkdbdash.writable_stream.prototype._next)
- description and source-code
```javascript
_next = function (value, encoding, done) {
  var self = this;
  if ((this._writableState.lastBufferedRequest != null) && (this._writableState.lastBufferedRequest.chunk !== value)) {
    // There's more data to buffer
    if (this._cache.length < this._highWaterMark) {
      this._delayed = false;
      // Call done now, and more data will be put in the cache
      done();
    }
    else {
      if (this._inserting === false) {
        if (this._delayed === true) {
          this._delayed = false;
          // We have to flush
          this._insert();
          // Fill the buffer while we are inserting data
          done();
        }
        else {
          var self = this;
          this._delayed = true;
          setImmediate(function() {
            self._next(value, encoding, done);
          })
        }

      }
      else {
        this._delayed = false;
        // to call when we are dong inserting to keep buffering
        this._pendingCallback = done;
      }
    }
  }
  else { // We just pushed the last element in the internal buffer
    if (this._inserting === false) {
      if (this._delayed === true) {
        this._delayed = false;
        // to call when we are dong inserting to maybe flag the end
        // We cannot call done here as we may be inserting the last batch
        this._pendingCallback = done;
        this._insert();
      }
      else {
        var self = this;
        this._delayed = true;
        setImmediate(function() {
          self._next(value, encoding, done);
        })
      }
    }
    else {
      this._delayed = false;
      // We cannot call done here as we may be inserting the last batch
      //this._pendingCallback = done;
      this._pendingCallback = function() {
        self._next(value, encoding, done);
      };
    }
  }
}
```
- example usage
```shell
...
  if (typeof onFinish === 'function') {
    onFinish();
  }
}
else {
  if (self._closed === false) {
    if (self._stackSize <= MAX_CALL_STACK) {
      self._next().then(resolve).error(function(error) {
        if ((error.message !== 'You cannot retrieve data from a cursor that is closed.') &&
            (error.message.match(/You cannot call 'next' on a closed/) === null)) {
          reject(error);
        }
      });
    }
    else {
...
```

#### <a name="apidoc.element.rethinkdbdash.writable_stream.prototype._write"></a>[function <span class="apidocSignatureSpan">rethinkdbdash.writable_stream.prototype.</span>_write (value, encoding, done)](#apidoc.element.rethinkdbdash.writable_stream.prototype._write)
- description and source-code
```javascript
_write = function (value, encoding, done) {
  this._i++;
  this._cache.push(value);
  this._next(value, encoding, done);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
