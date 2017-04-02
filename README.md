# api documentation for  [tap (v10.3.1)](http://node-tap.org/)  [![npm package](https://img.shields.io/npm/v/npmdoc-tap.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-tap) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-tap.svg)](https://travis-ci.org/npmdoc/node-npmdoc-tap)
#### A Test-Anything-Protocol library

[![NPM](https://nodei.co/npm/tap.png?downloads=true)](https://www.npmjs.com/package/tap)

[![apidoc](https://npmdoc.github.io/node-npmdoc-tap/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-tap_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-tap/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-tap/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Isaac Z. Schlueter",
        "email": "i@izs.me",
        "url": "http://blog.izs.me"
    },
    "bin": {
        "tap": "bin/run.js"
    },
    "bugs": {
        "url": "https://github.com/tapjs/node-tap/issues"
    },
    "config": {
        "nyc": {
            "exclude": [
                "node_modules/**",
                "test/**"
            ]
        }
    },
    "dependencies": {
        "bind-obj-methods": "^1.0.0",
        "bluebird": "^3.3.1",
        "clean-yaml-object": "^0.1.0",
        "color-support": "^1.1.0",
        "coveralls": "^2.11.2",
        "deeper": "^2.1.0",
        "foreground-child": "^1.3.3",
        "fs-exists-cached": "^1.0.0",
        "function-loop": "^1.0.1",
        "glob": "^7.0.0",
        "isexe": "^1.0.0",
        "js-yaml": "^3.3.1",
        "nyc": "^10.0.0",
        "only-shallow": "^1.0.2",
        "opener": "^1.4.1",
        "os-homedir": "1.0.1",
        "own-or": "^1.0.0",
        "own-or-env": "^1.0.0",
        "readable-stream": "^2.0.2",
        "signal-exit": "^3.0.0",
        "source-map-support": "^0.4.3",
        "stack-utils": "^1.0.0",
        "tap-mocha-reporter": "^3.0.1",
        "tap-parser": "^5.3.1",
        "tmatch": "^3.0.0",
        "trivial-deferred": "^1.0.1",
        "yapool": "^1.0.0"
    },
    "description": "A Test-Anything-Protocol library",
    "devDependencies": {
        "mkdirp": "^0.5.1",
        "rimraf": "^2.5.4",
        "standard": "^7.1.0",
        "which": "^1.1.1"
    },
    "directories": {},
    "dist": {
        "shasum": "3262fe43b6123cce7eab362420a2f3e70cee8b1c",
        "tarball": "https://registry.npmjs.org/tap/-/tap-10.3.1.tgz"
    },
    "engines": {
        "node": ">=0.8"
    },
    "files": [
        "bin/*",
        "lib/*"
    ],
    "gitHead": "98106c5533b94c48a949eddc427ea2080bc55dbe",
    "homepage": "http://node-tap.org/",
    "keywords": [
        "assert",
        "test",
        "tap"
    ],
    "license": "ISC",
    "main": "lib/tap.js",
    "maintainers": [
        {
            "name": "isaacs",
            "email": "i@izs.me"
        }
    ],
    "name": "tap",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tapjs/node-tap.git"
    },
    "scripts": {
        "postpublish": "git push origin --all; git push origin --tags",
        "posttest": "standard lib test",
        "postversion": "npm publish",
        "preversion": "npm test",
        "regen-fixtures": "node scripts/generate-test-test.js test/test/*.js",
        "smoke": "node bin/run.js --node-arg=test/test.js test/test/*.js -j2",
        "t": "node bin/run.js test/*.* -sfails.txt",
        "test": "node bin/run.js test/*.* --coverage -t3600 -sfails"
    },
    "version": "10.3.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module tap](#apidoc.module.tap)
1.  boolean <span class="apidocSignatureSpan">tap.</span>bail
1.  boolean <span class="apidocSignatureSpan">tap.</span>bailedOut
1.  boolean <span class="apidocSignatureSpan">tap.</span>buffered
1.  boolean <span class="apidocSignatureSpan">tap.</span>ended
1.  boolean <span class="apidocSignatureSpan">tap.</span>explicitEnded
1.  boolean <span class="apidocSignatureSpan">tap.</span>finished
1.  boolean <span class="apidocSignatureSpan">tap.</span>multiEndThrew
1.  boolean <span class="apidocSignatureSpan">tap.</span>noparallel
1.  boolean <span class="apidocSignatureSpan">tap.</span>occupied
1.  boolean <span class="apidocSignatureSpan">tap.</span>omitVersion
1.  boolean <span class="apidocSignatureSpan">tap.</span>preserveWhitespace
1.  boolean <span class="apidocSignatureSpan">tap.</span>pushedEnd
1.  boolean <span class="apidocSignatureSpan">tap.</span>ranAfterEach
1.  boolean <span class="apidocSignatureSpan">tap.</span>readable
1.  boolean <span class="apidocSignatureSpan">tap.</span>readyToProcess
1.  boolean <span class="apidocSignatureSpan">tap.</span>silent
1.  boolean <span class="apidocSignatureSpan">tap.</span>skip
1.  boolean <span class="apidocSignatureSpan">tap.</span>strict
1.  boolean <span class="apidocSignatureSpan">tap.</span>todo
1.  [function <span class="apidocSignatureSpan">tap.</span>Spawn (options)](#apidoc.element.tap.Spawn)
1.  [function <span class="apidocSignatureSpan">tap.</span>Spawn.super_ (options)](#apidoc.element.tap.Spawn.super_)
1.  [function <span class="apidocSignatureSpan">tap.</span>Stdin (options)](#apidoc.element.tap.Stdin)
1.  [function <span class="apidocSignatureSpan">tap.</span>Test (options)](#apidoc.element.tap.Test)
1.  [function <span class="apidocSignatureSpan">tap.</span>addAssert ()](#apidoc.element.tap.addAssert)
1.  [function <span class="apidocSignatureSpan">tap.</span>afterEach ()](#apidoc.element.tap.afterEach)
1.  [function <span class="apidocSignatureSpan">tap.</span>autoend ()](#apidoc.element.tap.autoend)
1.  [function <span class="apidocSignatureSpan">tap.</span>bailout ()](#apidoc.element.tap.bailout)
1.  [function <span class="apidocSignatureSpan">tap.</span>beforeEach ()](#apidoc.element.tap.beforeEach)
1.  [function <span class="apidocSignatureSpan">tap.</span>cb ()](#apidoc.element.tap.cb)
1.  [function <span class="apidocSignatureSpan">tap.</span>comment ()](#apidoc.element.tap.comment)
1.  [function <span class="apidocSignatureSpan">tap.</span>current ()](#apidoc.element.tap.current)
1.  [function <span class="apidocSignatureSpan">tap.</span>done ()](#apidoc.element.tap.done)
1.  [function <span class="apidocSignatureSpan">tap.</span>emitSubTeardown ()](#apidoc.element.tap.emitSubTeardown)
1.  [function <span class="apidocSignatureSpan">tap.</span>end ()](#apidoc.element.tap.end)
1.  [function <span class="apidocSignatureSpan">tap.</span>endAll ()](#apidoc.element.tap.endAll)
1.  [function <span class="apidocSignatureSpan">tap.</span>fail ()](#apidoc.element.tap.fail)
1.  [function <span class="apidocSignatureSpan">tap.</span>main ()](#apidoc.element.tap.main)
1.  [function <span class="apidocSignatureSpan">tap.</span>maybeAutoend ()](#apidoc.element.tap.maybeAutoend)
1.  [function <span class="apidocSignatureSpan">tap.</span>mochaGlobals ()](#apidoc.element.tap.mochaGlobals)
1.  [function <span class="apidocSignatureSpan">tap.</span>onbail ()](#apidoc.element.tap.onbail)
1.  [function <span class="apidocSignatureSpan">tap.</span>onbeforeend ()](#apidoc.element.tap.onbeforeend)
1.  [function <span class="apidocSignatureSpan">tap.</span>onbufferedend ()](#apidoc.element.tap.onbufferedend)
1.  [function <span class="apidocSignatureSpan">tap.</span>ondone ()](#apidoc.element.tap.ondone)
1.  [function <span class="apidocSignatureSpan">tap.</span>onindentedend ()](#apidoc.element.tap.onindentedend)
1.  [function <span class="apidocSignatureSpan">tap.</span>pass ()](#apidoc.element.tap.pass)
1.  [function <span class="apidocSignatureSpan">tap.</span>patchProcess ()](#apidoc.element.tap.patchProcess)
1.  [function <span class="apidocSignatureSpan">tap.</span>pipe ()](#apidoc.element.tap.pipe)
1.  [function <span class="apidocSignatureSpan">tap.</span>plan ()](#apidoc.element.tap.plan)
1.  [function <span class="apidocSignatureSpan">tap.</span>pragma ()](#apidoc.element.tap.pragma)
1.  [function <span class="apidocSignatureSpan">tap.</span>printResult ()](#apidoc.element.tap.printResult)
1.  [function <span class="apidocSignatureSpan">tap.</span>process ()](#apidoc.element.tap.process)
1.  [function <span class="apidocSignatureSpan">tap.</span>processSubtest ()](#apidoc.element.tap.processSubtest)
1.  [function <span class="apidocSignatureSpan">tap.</span>push ()](#apidoc.element.tap.push)
1.  [function <span class="apidocSignatureSpan">tap.</span>runAfterEach ()](#apidoc.element.tap.runAfterEach)
1.  [function <span class="apidocSignatureSpan">tap.</span>runBeforeEach ()](#apidoc.element.tap.runBeforeEach)
1.  [function <span class="apidocSignatureSpan">tap.</span>shouldAutoend ()](#apidoc.element.tap.shouldAutoend)
1.  [function <span class="apidocSignatureSpan">tap.</span>spawn ()](#apidoc.element.tap.spawn)
1.  [function <span class="apidocSignatureSpan">tap.</span>stdin ()](#apidoc.element.tap.stdin)
1.  [function <span class="apidocSignatureSpan">tap.</span>sub ()](#apidoc.element.tap.sub)
1.  [function <span class="apidocSignatureSpan">tap.</span>tearDown ()](#apidoc.element.tap.tearDown)
1.  [function <span class="apidocSignatureSpan">tap.</span>teardown ()](#apidoc.element.tap.teardown)
1.  [function <span class="apidocSignatureSpan">tap.</span>test ()](#apidoc.element.tap.test)
1.  [function <span class="apidocSignatureSpan">tap.</span>threw ()](#apidoc.element.tap.threw)
1.  [function <span class="apidocSignatureSpan">tap.</span>timeout ()](#apidoc.element.tap.timeout)
1.  [function <span class="apidocSignatureSpan">tap.</span>writeSubComment ()](#apidoc.element.tap.writeSubComment)
1.  number <span class="apidocSignatureSpan">tap.</span>_eventsCount
1.  number <span class="apidocSignatureSpan">tap.</span>count
1.  number <span class="apidocSignatureSpan">tap.</span>jobs
1.  number <span class="apidocSignatureSpan">tap.</span>n
1.  number <span class="apidocSignatureSpan">tap.</span>planEnd
1.  number <span class="apidocSignatureSpan">tap.</span>start
1.  object <span class="apidocSignatureSpan">tap.</span>Spawn.prototype
1.  object <span class="apidocSignatureSpan">tap.</span>Spawn.super_.prototype
1.  object <span class="apidocSignatureSpan">tap.</span>Stdin.prototype
1.  object <span class="apidocSignatureSpan">tap.</span>Test.prototype
1.  object <span class="apidocSignatureSpan">tap.</span>_events
1.  object <span class="apidocSignatureSpan">tap.</span>_readableState
1.  object <span class="apidocSignatureSpan">tap.</span>assertAt
1.  object <span class="apidocSignatureSpan">tap.</span>assertStack
1.  object <span class="apidocSignatureSpan">tap.</span>asserts
1.  object <span class="apidocSignatureSpan">tap.</span>currentAssert
1.  object <span class="apidocSignatureSpan">tap.</span>domain
1.  object <span class="apidocSignatureSpan">tap.</span>hrtime
1.  object <span class="apidocSignatureSpan">tap.</span>mocha
1.  object <span class="apidocSignatureSpan">tap.</span>onAfterEach
1.  object <span class="apidocSignatureSpan">tap.</span>onBeforeEach
1.  object <span class="apidocSignatureSpan">tap.</span>options
1.  object <span class="apidocSignatureSpan">tap.</span>parent
1.  object <span class="apidocSignatureSpan">tap.</span>parser
1.  object <span class="apidocSignatureSpan">tap.</span>pool
1.  object <span class="apidocSignatureSpan">tap.</span>queue
1.  object <span class="apidocSignatureSpan">tap.</span>results
1.  object <span class="apidocSignatureSpan">tap.</span>stack
1.  object <span class="apidocSignatureSpan">tap.</span>subtests
1.  object <span class="apidocSignatureSpan">tap.</span>synonyms
1.  object <span class="apidocSignatureSpan">tap.</span>time
1.  string <span class="apidocSignatureSpan">tap.</span>indent
1.  string <span class="apidocSignatureSpan">tap.</span>name
1.  string <span class="apidocSignatureSpan">tap.</span>output

#### [module tap.Spawn](#apidoc.module.tap.Spawn)
1.  [function <span class="apidocSignatureSpan">tap.</span>Spawn (options)](#apidoc.element.tap.Spawn.Spawn)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.</span>super_ (options)](#apidoc.element.tap.Spawn.super_)

#### [module tap.Spawn.prototype](#apidoc.module.tap.Spawn.prototype)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.prototype.</span>endAll ()](#apidoc.element.tap.Spawn.prototype.endAll)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.prototype.</span>main (cb)](#apidoc.element.tap.Spawn.prototype.main)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.prototype.</span>onprocclose (code, signal)](#apidoc.element.tap.Spawn.prototype.onprocclose)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.prototype.</span>threw (er, extra, proxy)](#apidoc.element.tap.Spawn.prototype.threw)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.prototype.</span>timeout (extra)](#apidoc.element.tap.Spawn.prototype.timeout)

#### [module tap.Spawn.super_](#apidoc.module.tap.Spawn.super_)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.</span>super_ (options)](#apidoc.element.tap.Spawn.super_.super_)

#### [module tap.Spawn.super_.prototype](#apidoc.module.tap.Spawn.super_.prototype)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>_read (n)](#apidoc.element.tap.Spawn.super_.prototype._read)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>debug ()](#apidoc.element.tap.Spawn.super_.prototype.debug)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>inspect ()](#apidoc.element.tap.Spawn.super_.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>main (cb)](#apidoc.element.tap.Spawn.super_.prototype.main)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>onbail (reason)](#apidoc.element.tap.Spawn.super_.prototype.onbail)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>onbeforeend ()](#apidoc.element.tap.Spawn.super_.prototype.onbeforeend)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>oncomplete (results)](#apidoc.element.tap.Spawn.super_.prototype.oncomplete)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>ondone ()](#apidoc.element.tap.Spawn.super_.prototype.ondone)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>online (line)](#apidoc.element.tap.Spawn.super_.prototype.online)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>passing ()](#apidoc.element.tap.Spawn.super_.prototype.passing)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>push (c, e)](#apidoc.element.tap.Spawn.super_.prototype.push)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>setTimeout (n)](#apidoc.element.tap.Spawn.super_.prototype.setTimeout)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>setupParser (options)](#apidoc.element.tap.Spawn.super_.prototype.setupParser)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>threw (er, extra, proxy)](#apidoc.element.tap.Spawn.super_.prototype.threw)
1.  [function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>timeout (options)](#apidoc.element.tap.Spawn.super_.prototype.timeout)

#### [module tap.Stdin](#apidoc.module.tap.Stdin)
1.  [function <span class="apidocSignatureSpan">tap.</span>Stdin (options)](#apidoc.element.tap.Stdin.Stdin)
1.  [function <span class="apidocSignatureSpan">tap.Stdin.</span>super_ (options)](#apidoc.element.tap.Stdin.super_)

#### [module tap.Stdin.prototype](#apidoc.module.tap.Stdin.prototype)
1.  [function <span class="apidocSignatureSpan">tap.Stdin.prototype.</span>main (cb)](#apidoc.element.tap.Stdin.prototype.main)
1.  [function <span class="apidocSignatureSpan">tap.Stdin.prototype.</span>threw (er, extra, proxy)](#apidoc.element.tap.Stdin.prototype.threw)

#### [module tap.Test](#apidoc.module.tap.Test)
1.  [function <span class="apidocSignatureSpan">tap.</span>Test (options)](#apidoc.element.tap.Test.Test)
1.  [function <span class="apidocSignatureSpan">tap.Test.</span>super_ (options)](#apidoc.element.tap.Test.super_)

#### [module tap.Test.prototype](#apidoc.module.tap.Test.prototype)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>addAssert (name, length, fn)](#apidoc.element.tap.Test.prototype.addAssert)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>afterEach (fn)](#apidoc.element.tap.Test.prototype.afterEach)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>autoend ()](#apidoc.element.tap.Test.prototype.autoend)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>bailout (message)](#apidoc.element.tap.Test.prototype.bailout)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>beforeEach (fn)](#apidoc.element.tap.Test.prototype.beforeEach)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>comment ()](#apidoc.element.tap.Test.prototype.comment)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>current ()](#apidoc.element.tap.Test.prototype.current)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>done (implicit)](#apidoc.element.tap.Test.prototype.done)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>emitSubTeardown (p)](#apidoc.element.tap.Test.prototype.emitSubTeardown)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>end (implicit)](#apidoc.element.tap.Test.prototype.end)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>endAll (sub)](#apidoc.element.tap.Test.prototype.endAll)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>fail (message, extra)](#apidoc.element.tap.Test.prototype.fail)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>main (cb)](#apidoc.element.tap.Test.prototype.main)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>maybeAutoend ()](#apidoc.element.tap.Test.prototype.maybeAutoend)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>onbufferedend (p, er)](#apidoc.element.tap.Test.prototype.onbufferedend)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>onindentedend (p, er)](#apidoc.element.tap.Test.prototype.onindentedend)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>pass (message, extra)](#apidoc.element.tap.Test.prototype.pass)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>plan (n, comment)](#apidoc.element.tap.Test.prototype.plan)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>pragma (set)](#apidoc.element.tap.Test.prototype.pragma)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>printResult (ok, message, extra, front)](#apidoc.element.tap.Test.prototype.printResult)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>process ()](#apidoc.element.tap.Test.prototype.process)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>processSubtest (p)](#apidoc.element.tap.Test.prototype.processSubtest)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>runAfterEach (who, cb)](#apidoc.element.tap.Test.prototype.runAfterEach)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>runBeforeEach (who, cb)](#apidoc.element.tap.Test.prototype.runBeforeEach)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>shouldAutoend ()](#apidoc.element.tap.Test.prototype.shouldAutoend)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>spawn (cmd, args, options, name)](#apidoc.element.tap.Test.prototype.spawn)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>stdin (name, extra)](#apidoc.element.tap.Test.prototype.stdin)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>sub (Class, extra, caller)](#apidoc.element.tap.Test.prototype.sub)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>tearDown (fn)](#apidoc.element.tap.Test.prototype.tearDown)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>teardown (fn)](#apidoc.element.tap.Test.prototype.teardown)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>test (name, extra, cb)](#apidoc.element.tap.Test.prototype.test)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>threw (er, extra, proxy)](#apidoc.element.tap.Test.prototype.threw)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>timeout (options)](#apidoc.element.tap.Test.prototype.timeout)
1.  [function <span class="apidocSignatureSpan">tap.Test.prototype.</span>writeSubComment (p, cb)](#apidoc.element.tap.Test.prototype.writeSubComment)

#### [module tap.asserts](#apidoc.module.tap.asserts)
1.  [function <span class="apidocSignatureSpan">tap.asserts.</span>decorate (t)](#apidoc.element.tap.asserts.decorate)

#### [module tap.mocha](#apidoc.module.tap.mocha)
1.  [function <span class="apidocSignatureSpan">tap.mocha.</span>after (name, fn)](#apidoc.element.tap.mocha.after)
1.  [function <span class="apidocSignatureSpan">tap.mocha.</span>afterEach (fn)](#apidoc.element.tap.mocha.afterEach)
1.  [function <span class="apidocSignatureSpan">tap.mocha.</span>before (name, fn)](#apidoc.element.tap.mocha.before)
1.  [function <span class="apidocSignatureSpan">tap.mocha.</span>beforeEach (fn)](#apidoc.element.tap.mocha.beforeEach)
1.  [function <span class="apidocSignatureSpan">tap.mocha.</span>context (name, fn)](#apidoc.element.tap.mocha.context)
1.  [function <span class="apidocSignatureSpan">tap.mocha.</span>describe (name, fn)](#apidoc.element.tap.mocha.describe)
1.  [function <span class="apidocSignatureSpan">tap.mocha.</span>global ()](#apidoc.element.tap.mocha.global)
1.  [function <span class="apidocSignatureSpan">tap.mocha.</span>it (name, fn)](#apidoc.element.tap.mocha.it)
1.  [function <span class="apidocSignatureSpan">tap.mocha.</span>specify (name, fn)](#apidoc.element.tap.mocha.specify)

#### [module tap.stack](#apidoc.module.tap.stack)
1.  [function <span class="apidocSignatureSpan">tap.stack.</span>_wrapCallSite (frame)](#apidoc.element.tap.stack._wrapCallSite)
1.  object <span class="apidocSignatureSpan">tap.stack.</span>_internals
1.  string <span class="apidocSignatureSpan">tap.stack.</span>_cwd



# <a name="apidoc.module.tap"></a>[module tap](#apidoc.module.tap)

#### <a name="apidoc.element.tap.Spawn"></a>[function <span class="apidocSignatureSpan">tap.</span>Spawn (options)](#apidoc.element.tap.Spawn)
- description and source-code
```javascript
function Spawn(options) {
  options = options || {}
  if (!(this instanceof Spawn))
    return new Spawn(options)

  Base.call(this, options)

  this.command = options.command

  if (!this.command)
    throw new TypeError('no command provided')

  this.args = options.args
  // stdout must be a pipe
  if (options.stdio) {
    if (typeof options.stdio === 'string')
      this.stdio = [ options.stdio, 'pipe', options.stdio ]
    else
      this.stdio = options.stdio.slice(0)
  } else
    this.stdio = [ 0, 'pipe', 2 ]

  this.stdio[1] = 'pipe'
  var env = options.env || process.env
  this.env = Object.keys(env).reduce(function (e, k) {
    e[k] = env[k]
    return e
  }, {})

  this.env.TAP = '1'
  if (this.bail)
    this.env.TAP_BAIL = '1'

  this.cwd = ownOr(options, 'cwd', process.cwd())
  options.cwd = this.cwd
  if (!this.name) {
    if (this.command === process.execPath) {
      this.name = path.basename(process.execPath) + ' ' +
        this.args.map(function (a) {
          if (a.indexOf(this.cwd) === 0) {
            return './' +
              a.substr(this.cwd.length + 1).replace(/\\/g, '/')
          } else {
            return a
          }
        }, this).join(' ')
    } else {
      this.name = this.command + ' ' + this.args.join(' ')
    }
  }

  this.proc = null
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_"></a>[function <span class="apidocSignatureSpan">tap.</span>Spawn.super_ (options)](#apidoc.element.tap.Spawn.super_)
- description and source-code
```javascript
function Base(options) {
  this.start = 0
  this.hrtime = null
  this.time = null
  this.readyToProcess = false
  this.options = options
  this.parent = ownOr(options, 'parent', null)
  this.bail = ownOrEnv(options, 'bail', 'TAP_BAIL', true)
  this.name = ownOr(options, 'name', '')
  if (!this.name)
    this.name = ''
  else
    this.name = this.name.replace(/[\n\r\s\t]/g, ' ')
  this.indent = ownOr(options, 'indent', '')
  this.silent = !!options.silent
  this.buffered = !!options.buffered || !!options.silent
  this.finished = false
  this.strict = ownOrEnv(options, 'strict', 'TAP_STRICT', true)
  this.omitVersion = !!options.omitVersion
  this.preserveWhitespace = ownOr(options, 'preserveWhitespace', true)
  this.jobs = +ownOrEnv(options, 'jobs', 'TAP_JOBS') || 0
  this.skip = ownOr(options, 'skip', false)
  this.todo = ownOr(options, 'todo', false)
  this.setupParser(options)
  this.finished = false
  this.output = ''
  this.results = null
  this.bailedOut = false
  if (this.skip || this.todo)
    this.main = Base.prototype.main

  Readable.apply(this, options)

  domain.create().add(this)
  this.domain.on('error', this.threw.bind(this))

  if (typeof options.debug === 'boolean')
    this.debug = options.debug ? debug : nodebug
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Stdin"></a>[function <span class="apidocSignatureSpan">tap.</span>Stdin (options)](#apidoc.element.tap.Stdin)
- description and source-code
```javascript
function Stdin(options) {
  options = options || {}
  if (!(this instanceof Stdin))
    return new Stdin(options)

  options.name = ownOr(options, 'name', '/dev/stdin')
  Base.call(this, options)

  // This has to be here for node 0.10's wonky streams
  this.stream = ownOr(options, 'tapStream', process.stdin)
  this.stream.pause()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test"></a>[function <span class="apidocSignatureSpan">tap.</span>Test (options)](#apidoc.element.tap.Test)
- description and source-code
```javascript
function Test(options) {
  options = options || {}
  if (!(this instanceof Test))
    return new Test(options)

  Base.call(this, options)
  this.pushedEnd = false
  this.jobs = ownOr(options, 'jobs', 1)
  this.subtests = []
  this.pool = new Pool()
  this.queue = ['TAP version 13\n']
  this.noparallel = false
  this.cb = this.domain.bind(options.cb)
  this.occupied = false
  this.currentAssert = null
  this.count = 0
  this.n = 0
  this.ended = false
  this.explicitEnded = false
  this.multiEndThrew = false
  this.currentAssert = null
  this.assertAt = null
  this.assertStack = null
  this.planEnd = -1
  this.onBeforeEach = []
  this.onAfterEach = []
  this.ranAfterEach = false

  // bind all methods to this object, so we can pass t.end as a callback
  // and do 'var test = require('tap').test' like people do.
  var bound = Object.create(null)
  bindObj(this, this, bound)
  bindObj(this, Object.getPrototypeOf(this), bound)
  bindObj(this, Test.prototype, bound)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.addAssert"></a>[function <span class="apidocSignatureSpan">tap.</span>addAssert ()](#apidoc.element.tap.addAssert)
- description and source-code
```javascript
addAssert = function () { [native code] }
```
- example usage
```shell
...
// typically, a plugin would do this on a specific instance, eg on
// the root test harness instance.  but we do this here to add some
// useful prototype methods.

exports.decorate = decorate

function decorate (t) {
t.addAssert('ok', 1, function (obj, message, extra) {
  message = message || 'expect truthy value'
  if (obj) {
    return this.pass(message, extra)
  }

  return this.fail(message, extra)
})
...
```

#### <a name="apidoc.element.tap.afterEach"></a>[function <span class="apidocSignatureSpan">tap.</span>afterEach ()](#apidoc.element.tap.afterEach)
- description and source-code
```javascript
afterEach = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.autoend"></a>[function <span class="apidocSignatureSpan">tap.</span>autoend ()](#apidoc.element.tap.autoend)
- description and source-code
```javascript
autoend = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.bailout"></a>[function <span class="apidocSignatureSpan">tap.</span>bailout ()](#apidoc.element.tap.bailout)
- description and source-code
```javascript
bailout = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.beforeEach"></a>[function <span class="apidocSignatureSpan">tap.</span>beforeEach ()](#apidoc.element.tap.beforeEach)
- description and source-code
```javascript
beforeEach = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.cb"></a>[function <span class="apidocSignatureSpan">tap.</span>cb ()](#apidoc.element.tap.cb)
- description and source-code
```javascript
cb = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.comment"></a>[function <span class="apidocSignatureSpan">tap.</span>comment ()](#apidoc.element.tap.comment)
- description and source-code
```javascript
comment = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.current"></a>[function <span class="apidocSignatureSpan">tap.</span>current ()](#apidoc.element.tap.current)
- description and source-code
```javascript
current = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.done"></a>[function <span class="apidocSignatureSpan">tap.</span>done ()](#apidoc.element.tap.done)
- description and source-code
```javascript
done = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.emitSubTeardown"></a>[function <span class="apidocSignatureSpan">tap.</span>emitSubTeardown ()](#apidoc.element.tap.emitSubTeardown)
- description and source-code
```javascript
emitSubTeardown = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.end"></a>[function <span class="apidocSignatureSpan">tap.</span>end ()](#apidoc.element.tap.end)
- description and source-code
```javascript
end = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.endAll"></a>[function <span class="apidocSignatureSpan">tap.</span>endAll ()](#apidoc.element.tap.endAll)
- description and source-code
```javascript
endAll = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.fail"></a>[function <span class="apidocSignatureSpan">tap.</span>fail ()](#apidoc.element.tap.fail)
- description and source-code
```javascript
fail = function () { [native code] }
```
- example usage
```shell
...
function decorate (t) {
t.addAssert('ok', 1, function (obj, message, extra) {
  message = message || 'expect truthy value'
  if (obj) {
    return this.pass(message, extra)
  }

  return this.fail(message, extra)
})

t.addAssert('notOk', 1, function (obj, message, extra) {
  message = message || 'expect falsey value'
  return this.ok(!obj, message, extra)
})
...
```

#### <a name="apidoc.element.tap.main"></a>[function <span class="apidocSignatureSpan">tap.</span>main ()](#apidoc.element.tap.main)
- description and source-code
```javascript
main = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.maybeAutoend"></a>[function <span class="apidocSignatureSpan">tap.</span>maybeAutoend ()](#apidoc.element.tap.maybeAutoend)
- description and source-code
```javascript
maybeAutoend = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.mochaGlobals"></a>[function <span class="apidocSignatureSpan">tap.</span>mochaGlobals ()](#apidoc.element.tap.mochaGlobals)
- description and source-code
```javascript
mochaGlobals = function () {
  Object.keys(exports).forEach(function (g) {
    global[g] = exports[g]
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.onbail"></a>[function <span class="apidocSignatureSpan">tap.</span>onbail ()](#apidoc.element.tap.onbail)
- description and source-code
```javascript
onbail = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.onbeforeend"></a>[function <span class="apidocSignatureSpan">tap.</span>onbeforeend ()](#apidoc.element.tap.onbeforeend)
- description and source-code
```javascript
onbeforeend = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.onbufferedend"></a>[function <span class="apidocSignatureSpan">tap.</span>onbufferedend ()](#apidoc.element.tap.onbufferedend)
- description and source-code
```javascript
onbufferedend = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.ondone"></a>[function <span class="apidocSignatureSpan">tap.</span>ondone ()](#apidoc.element.tap.ondone)
- description and source-code
```javascript
ondone = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.onindentedend"></a>[function <span class="apidocSignatureSpan">tap.</span>onindentedend ()](#apidoc.element.tap.onindentedend)
- description and source-code
```javascript
onindentedend = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.pass"></a>[function <span class="apidocSignatureSpan">tap.</span>pass ()](#apidoc.element.tap.pass)
- description and source-code
```javascript
pass = function () { [native code] }
```
- example usage
```shell
...

exports.decorate = decorate

function decorate (t) {
t.addAssert('ok', 1, function (obj, message, extra) {
  message = message || 'expect truthy value'
  if (obj) {
    return this.pass(message, extra)
  }

  return this.fail(message, extra)
})

t.addAssert('notOk', 1, function (obj, message, extra) {
  message = message || 'expect falsey value'
...
```

#### <a name="apidoc.element.tap.patchProcess"></a>[function <span class="apidocSignatureSpan">tap.</span>patchProcess ()](#apidoc.element.tap.patchProcess)
- description and source-code
```javascript
patchProcess = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.pipe"></a>[function <span class="apidocSignatureSpan">tap.</span>pipe ()](#apidoc.element.tap.pipe)
- description and source-code
```javascript
pipe = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.plan"></a>[function <span class="apidocSignatureSpan">tap.</span>plan ()](#apidoc.element.tap.plan)
- description and source-code
```javascript
plan = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.pragma"></a>[function <span class="apidocSignatureSpan">tap.</span>pragma ()](#apidoc.element.tap.pragma)
- description and source-code
```javascript
pragma = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.printResult"></a>[function <span class="apidocSignatureSpan">tap.</span>printResult ()](#apidoc.element.tap.printResult)
- description and source-code
```javascript
printResult = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.process"></a>[function <span class="apidocSignatureSpan">tap.</span>process ()](#apidoc.element.tap.process)
- description and source-code
```javascript
process = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.processSubtest"></a>[function <span class="apidocSignatureSpan">tap.</span>processSubtest ()](#apidoc.element.tap.processSubtest)
- description and source-code
```javascript
processSubtest = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.push"></a>[function <span class="apidocSignatureSpan">tap.</span>push ()](#apidoc.element.tap.push)
- description and source-code
```javascript
push = function () { [native code] }
```
- example usage
```shell
...
  })
  return obj
}

function multiword_ (str) {
  var res = [ str ]
  if (str.match(/[A-Z]/)) {
    res.push(str.toLowerCase())
    res.push(str.replace(/[A-Z]/g, function ($0) {
      return '_' + $0.toLowerCase()
    }))
  }
  return res
}
...
```

#### <a name="apidoc.element.tap.runAfterEach"></a>[function <span class="apidocSignatureSpan">tap.</span>runAfterEach ()](#apidoc.element.tap.runAfterEach)
- description and source-code
```javascript
runAfterEach = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.runBeforeEach"></a>[function <span class="apidocSignatureSpan">tap.</span>runBeforeEach ()](#apidoc.element.tap.runBeforeEach)
- description and source-code
```javascript
runBeforeEach = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.shouldAutoend"></a>[function <span class="apidocSignatureSpan">tap.</span>shouldAutoend ()](#apidoc.element.tap.shouldAutoend)
- description and source-code
```javascript
shouldAutoend = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.spawn"></a>[function <span class="apidocSignatureSpan">tap.</span>spawn ()](#apidoc.element.tap.spawn)
- description and source-code
```javascript
spawn = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.stdin"></a>[function <span class="apidocSignatureSpan">tap.</span>stdin ()](#apidoc.element.tap.stdin)
- description and source-code
```javascript
stdin = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.sub"></a>[function <span class="apidocSignatureSpan">tap.</span>sub ()](#apidoc.element.tap.sub)
- description and source-code
```javascript
sub = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.tearDown"></a>[function <span class="apidocSignatureSpan">tap.</span>tearDown ()](#apidoc.element.tap.tearDown)
- description and source-code
```javascript
tearDown = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.teardown"></a>[function <span class="apidocSignatureSpan">tap.</span>teardown ()](#apidoc.element.tap.teardown)
- description and source-code
```javascript
teardown = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.test"></a>[function <span class="apidocSignatureSpan">tap.</span>test ()](#apidoc.element.tap.test)
- description and source-code
```javascript
test = function () { [native code] }
```
- example usage
```shell
...
  if (source.stack)
    target.stack = source.stack
  return false
}

return !(propertyName === 'todo' ||
propertyName === 'time' ||
/^_?tapChild/.test(propertyName) ||
/^tapStream/.test(propertyName) ||
/^tapMochaTest/.test(propertyName) ||
propertyName === 'cb' ||
propertyName === 'name' ||
propertyName === 'indent' ||
propertyName === 'skip' ||
propertyName === 'bail' ||
...
```

#### <a name="apidoc.element.tap.threw"></a>[function <span class="apidocSignatureSpan">tap.</span>threw ()](#apidoc.element.tap.threw)
- description and source-code
```javascript
threw = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.timeout"></a>[function <span class="apidocSignatureSpan">tap.</span>timeout ()](#apidoc.element.tap.timeout)
- description and source-code
```javascript
timeout = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.writeSubComment"></a>[function <span class="apidocSignatureSpan">tap.</span>writeSubComment ()](#apidoc.element.tap.writeSubComment)
- description and source-code
```javascript
writeSubComment = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tap.Spawn"></a>[module tap.Spawn](#apidoc.module.tap.Spawn)

#### <a name="apidoc.element.tap.Spawn.Spawn"></a>[function <span class="apidocSignatureSpan">tap.</span>Spawn (options)](#apidoc.element.tap.Spawn.Spawn)
- description and source-code
```javascript
function Spawn(options) {
  options = options || {}
  if (!(this instanceof Spawn))
    return new Spawn(options)

  Base.call(this, options)

  this.command = options.command

  if (!this.command)
    throw new TypeError('no command provided')

  this.args = options.args
  // stdout must be a pipe
  if (options.stdio) {
    if (typeof options.stdio === 'string')
      this.stdio = [ options.stdio, 'pipe', options.stdio ]
    else
      this.stdio = options.stdio.slice(0)
  } else
    this.stdio = [ 0, 'pipe', 2 ]

  this.stdio[1] = 'pipe'
  var env = options.env || process.env
  this.env = Object.keys(env).reduce(function (e, k) {
    e[k] = env[k]
    return e
  }, {})

  this.env.TAP = '1'
  if (this.bail)
    this.env.TAP_BAIL = '1'

  this.cwd = ownOr(options, 'cwd', process.cwd())
  options.cwd = this.cwd
  if (!this.name) {
    if (this.command === process.execPath) {
      this.name = path.basename(process.execPath) + ' ' +
        this.args.map(function (a) {
          if (a.indexOf(this.cwd) === 0) {
            return './' +
              a.substr(this.cwd.length + 1).replace(/\\/g, '/')
          } else {
            return a
          }
        }, this).join(' ')
    } else {
      this.name = this.command + ' ' + this.args.join(' ')
    }
  }

  this.proc = null
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_"></a>[function <span class="apidocSignatureSpan">tap.Spawn.</span>super_ (options)](#apidoc.element.tap.Spawn.super_)
- description and source-code
```javascript
function Base(options) {
  this.start = 0
  this.hrtime = null
  this.time = null
  this.readyToProcess = false
  this.options = options
  this.parent = ownOr(options, 'parent', null)
  this.bail = ownOrEnv(options, 'bail', 'TAP_BAIL', true)
  this.name = ownOr(options, 'name', '')
  if (!this.name)
    this.name = ''
  else
    this.name = this.name.replace(/[\n\r\s\t]/g, ' ')
  this.indent = ownOr(options, 'indent', '')
  this.silent = !!options.silent
  this.buffered = !!options.buffered || !!options.silent
  this.finished = false
  this.strict = ownOrEnv(options, 'strict', 'TAP_STRICT', true)
  this.omitVersion = !!options.omitVersion
  this.preserveWhitespace = ownOr(options, 'preserveWhitespace', true)
  this.jobs = +ownOrEnv(options, 'jobs', 'TAP_JOBS') || 0
  this.skip = ownOr(options, 'skip', false)
  this.todo = ownOr(options, 'todo', false)
  this.setupParser(options)
  this.finished = false
  this.output = ''
  this.results = null
  this.bailedOut = false
  if (this.skip || this.todo)
    this.main = Base.prototype.main

  Readable.apply(this, options)

  domain.create().add(this)
  this.domain.on('error', this.threw.bind(this))

  if (typeof options.debug === 'boolean')
    this.debug = options.debug ? debug : nodebug
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tap.Spawn.prototype"></a>[module tap.Spawn.prototype](#apidoc.module.tap.Spawn.prototype)

#### <a name="apidoc.element.tap.Spawn.prototype.endAll"></a>[function <span class="apidocSignatureSpan">tap.Spawn.prototype.</span>endAll ()](#apidoc.element.tap.Spawn.prototype.endAll)
- description and source-code
```javascript
endAll = function () {
  if (this.proc)
    this.proc.kill('SIGKILL')
  this.parser.abort('test unfinished')
  this.cb()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.prototype.main"></a>[function <span class="apidocSignatureSpan">tap.Spawn.prototype.</span>main (cb)](#apidoc.element.tap.Spawn.prototype.main)
- description and source-code
```javascript
main = function (cb) {
  this.cb = cb
  this.setTimeout(this.options.timeout)
  var options = Object.keys(this.options).reduce(function (o, k) {
    o[k] = this.options[k]
    return o
  }.bind(this), {
    cwd: this.cwd,
    env: this.env,
    stdio: this.stdio
  })
  try {
    var proc = this.proc = spawn(this.command, this.args, options)
    proc.stdout.pipe(this.parser)
    proc.on('close', this.onprocclose.bind(this))
    proc.on('error', this.threw.bind(this))
  } catch (er) {
    this.threw(er)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.prototype.onprocclose"></a>[function <span class="apidocSignatureSpan">tap.Spawn.prototype.</span>onprocclose (code, signal)](#apidoc.element.tap.Spawn.prototype.onprocclose)
- description and source-code
```javascript
onprocclose = function (code, signal) {
  this.debug('SPAWN close %j %s', code, signal)
  this.options.exitCode = code
  if (signal)
    this.options.signal = signal
  this.results = this.results || {}

  // spawn closing with no tests is treated as a skip.
  if (this.results.plan && this.results.plan.skipAll && !code && !signal)
    this.options.skip = this.results.plan.skipReason || true

  if (code || signal) {
    this.results.ok = false
    this.parser.ok = false
  }
  return this.cb()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.prototype.threw"></a>[function <span class="apidocSignatureSpan">tap.Spawn.prototype.</span>threw (er, extra, proxy)](#apidoc.element.tap.Spawn.prototype.threw)
- description and source-code
```javascript
threw = function (er, extra, proxy) {
  extra = Base.prototype.threw.call(this, er, extra, proxy)
  extra = cleanYamlObject(extra)
  // unhook entirely
  this.parser.abort(er.message, extra)
  if (this.proc) {
    this.proc.stdout.removeAllListeners('data')
    this.proc.stdout.removeAllListeners('end')
    this.proc.removeAllListeners('close')
    this.proc.kill('SIGKILL')
  }
  this.cb()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.prototype.timeout"></a>[function <span class="apidocSignatureSpan">tap.Spawn.prototype.</span>timeout (extra)](#apidoc.element.tap.Spawn.prototype.timeout)
- description and source-code
```javascript
timeout = function (extra) {
  if (this.proc)
    this.proc.kill('SIGTERM')
  var t = setTimeout(function () {
    if (!this.options.signal && this.options.exitCode === undefined) {
      Base.prototype.timeout.call(this, extra)
      this.proc.kill('SIGKILL')
    }
  }.bind(this), 1000)
  if (t.unref)
    t.unref()
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tap.Spawn.super_"></a>[module tap.Spawn.super_](#apidoc.module.tap.Spawn.super_)

#### <a name="apidoc.element.tap.Spawn.super_.super_"></a>[function <span class="apidocSignatureSpan">tap.Spawn.</span>super_ (options)](#apidoc.element.tap.Spawn.super_.super_)
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



# <a name="apidoc.module.tap.Spawn.super_.prototype"></a>[module tap.Spawn.super_.prototype](#apidoc.module.tap.Spawn.super_.prototype)

#### <a name="apidoc.element.tap.Spawn.super_.prototype._read"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>_read (n)](#apidoc.element.tap.Spawn.super_.prototype._read)
- description and source-code
```javascript
_read = function (n) {
  // this.emit('readable')
  // this.debug('_read %j', this.name, arguments)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_.prototype.debug"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>debug ()](#apidoc.element.tap.Spawn.super_.prototype.debug)
- description and source-code
```javascript
function nodebug() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_.prototype.inspect"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>inspect ()](#apidoc.element.tap.Spawn.super_.prototype.inspect)
- description and source-code
```javascript
inspect = function () {
  return this.constructor.name + ' ' + util.inspect({
    name: this.name,
    jobs: this.jobs,
    buffered: this.buffered,
    occupied: this.occupied,
    pool: this.pool,
    queue: this.queue,
    subtests: this.subtests,
    output: this.output,
    skip: this.skip,
    todo: this.todo,
    results: this.results,
    options: [
      'autoend',
      'command',
      'args',
      'stdio',
      'env',
      'cwd',
      'exitCode',
      'signal',
      'expired',
      'timeout',
      'at',
      'skip',
      'todo'
    ].reduce(function (set, k) {
      if (this.options[k] !== undefined)
        set[k] = this.options[k]
      return set
    }.bind(this), {})
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_.prototype.main"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>main (cb)](#apidoc.element.tap.Spawn.super_.prototype.main)
- description and source-code
```javascript
main = function (cb) {
  cb()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_.prototype.onbail"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>onbail (reason)](#apidoc.element.tap.Spawn.super_.prototype.onbail)
- description and source-code
```javascript
onbail = function (reason) {
  this.bailedOut = reason || true
  this.emit('bailout', reason)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_.prototype.onbeforeend"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>onbeforeend ()](#apidoc.element.tap.Spawn.super_.prototype.onbeforeend)
- description and source-code
```javascript
onbeforeend = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_.prototype.oncomplete"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>oncomplete (results)](#apidoc.element.tap.Spawn.super_.prototype.oncomplete)
- description and source-code
```javascript
oncomplete = function (results) {
  if (this.hrtime) {
    this.hrtime = process.hrtime(this.hrtime)
    this.time = Math.round(this.hrtime[0] * 1e6 + this.hrtime[1] / 1e3) / 1e3
  }

  this.debug('ONCOMPLETE %j %j', this.name, results)

  if (this.results)
    Object.keys(this.results).forEach(function (k) {
      results[k] = this.results[k]
    }, this)

  this.results = results
  this.emit('complete', results)
  var failures = results.failures.filter(function (f) {
    delete f.diag
    delete f.ok
    return f.tapError
  })

  if (failures.length)
    this.options.failures = failures

  this.onbeforeend()
  this.emit('end')
  this.ondone()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_.prototype.ondone"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>ondone ()](#apidoc.element.tap.Spawn.super_.prototype.ondone)
- description and source-code
```javascript
ondone = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_.prototype.online"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>online (line)](#apidoc.element.tap.Spawn.super_.prototype.online)
- description and source-code
```javascript
online = function (line) {
  this.debug('LINE %j', line)
  return this.push(this.indent + line)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_.prototype.passing"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>passing ()](#apidoc.element.tap.Spawn.super_.prototype.passing)
- description and source-code
```javascript
passing = function () {
  return this.parser.ok
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_.prototype.push"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>push (c, e)](#apidoc.element.tap.Spawn.super_.prototype.push)
- description and source-code
```javascript
push = function (c, e) {
  assert.equal(typeof c, 'string')
  assert.equal(c.substr(-1), '\n')

  if (this.buffered) {
    this.output += c
    return true
  }

  // We *always* want data coming out immediately.  Test runners have a
  // very special relationship with zalgo. It's more important to ensure
  // that any console.log() lines that appear in the midst of tests are
  // not taken out of context
  if (this._readableState) {
    this._readableState.sync = false
  }

  // this.debug(this._readableState)
  return Readable.prototype.push.call(this, c, e)
}
```
- example usage
```shell
...
  })
  return obj
}

function multiword_ (str) {
  var res = [ str ]
  if (str.match(/[A-Z]/)) {
    res.push(str.toLowerCase())
    res.push(str.replace(/[A-Z]/g, function ($0) {
      return '_' + $0.toLowerCase()
    }))
  }
  return res
}
...
```

#### <a name="apidoc.element.tap.Spawn.super_.prototype.setTimeout"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>setTimeout (n)](#apidoc.element.tap.Spawn.super_.prototype.setTimeout)
- description and source-code
```javascript
setTimeout = function (n) {
  if (!this.hrtime)
    this.hrtime = process.hrtime()

  if (!n) {
    clearTimeout(this.timer)
    this.timer = null
  } else {
    this.start = Date.now()
    this.timer = setTimeout(this.timeout.bind(this), n)
    if (this.timer.unref)
      this.timer.unref()
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_.prototype.setupParser"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>setupParser (options)](#apidoc.element.tap.Spawn.super_.prototype.setupParser)
- description and source-code
```javascript
setupParser = function (options) {
  this.parser = new Parser({
    bail: this.bail,
    strict: this.strict,
    omitVersion: this.omitVersion,
    preserveWhitespace: this.preserveWhitespace
  })
  assert(this.parser.preserveWhitespace)
  this.parser.on('line', this.online.bind(this))
  this.parser.once('bailout', this.onbail.bind(this))
  this.parser.on('complete', this.oncomplete.bind(this))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_.prototype.threw"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>threw (er, extra, proxy)](#apidoc.element.tap.Spawn.super_.prototype.threw)
- description and source-code
```javascript
threw = function (er, extra, proxy) {
  if (this.name && !proxy)
    er.test = this.name

  var message = er.message

  if (!extra)
    extra = extraFromError(er, extra, this.options)

  if (this.results || this.ended) {
    this.results.ok = false
    if (this.parent)
      this.parent.threw(er, extra, true)
    else if (!er.stack)
      console.error(er)
    else {
      er.message = message
      delete extra.stack
      delete extra.at
      console.error('%s: %s', er.name || 'Error', message)
      console.error(er.stack.split(/\n/).slice(1).join('\n'))
      console.error(extra)
    }
  } else
    this.parser.ok = false

  return extra
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Spawn.super_.prototype.timeout"></a>[function <span class="apidocSignatureSpan">tap.Spawn.super_.prototype.</span>timeout (options)](#apidoc.element.tap.Spawn.super_.prototype.timeout)
- description and source-code
```javascript
timeout = function (options) {
  this.setTimeout(false)
  var er = new Error('timeout!')
  options = options || {}
  options.expired = options.expired || this.name
  this.threw(new Error('timeout!'), options)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tap.Stdin"></a>[module tap.Stdin](#apidoc.module.tap.Stdin)

#### <a name="apidoc.element.tap.Stdin.Stdin"></a>[function <span class="apidocSignatureSpan">tap.</span>Stdin (options)](#apidoc.element.tap.Stdin.Stdin)
- description and source-code
```javascript
function Stdin(options) {
  options = options || {}
  if (!(this instanceof Stdin))
    return new Stdin(options)

  options.name = ownOr(options, 'name', '/dev/stdin')
  Base.call(this, options)

  // This has to be here for node 0.10's wonky streams
  this.stream = ownOr(options, 'tapStream', process.stdin)
  this.stream.pause()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Stdin.super_"></a>[function <span class="apidocSignatureSpan">tap.Stdin.</span>super_ (options)](#apidoc.element.tap.Stdin.super_)
- description and source-code
```javascript
function Base(options) {
  this.start = 0
  this.hrtime = null
  this.time = null
  this.readyToProcess = false
  this.options = options
  this.parent = ownOr(options, 'parent', null)
  this.bail = ownOrEnv(options, 'bail', 'TAP_BAIL', true)
  this.name = ownOr(options, 'name', '')
  if (!this.name)
    this.name = ''
  else
    this.name = this.name.replace(/[\n\r\s\t]/g, ' ')
  this.indent = ownOr(options, 'indent', '')
  this.silent = !!options.silent
  this.buffered = !!options.buffered || !!options.silent
  this.finished = false
  this.strict = ownOrEnv(options, 'strict', 'TAP_STRICT', true)
  this.omitVersion = !!options.omitVersion
  this.preserveWhitespace = ownOr(options, 'preserveWhitespace', true)
  this.jobs = +ownOrEnv(options, 'jobs', 'TAP_JOBS') || 0
  this.skip = ownOr(options, 'skip', false)
  this.todo = ownOr(options, 'todo', false)
  this.setupParser(options)
  this.finished = false
  this.output = ''
  this.results = null
  this.bailedOut = false
  if (this.skip || this.todo)
    this.main = Base.prototype.main

  Readable.apply(this, options)

  domain.create().add(this)
  this.domain.on('error', this.threw.bind(this))

  if (typeof options.debug === 'boolean')
    this.debug = options.debug ? debug : nodebug
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tap.Stdin.prototype"></a>[module tap.Stdin.prototype](#apidoc.module.tap.Stdin.prototype)

#### <a name="apidoc.element.tap.Stdin.prototype.main"></a>[function <span class="apidocSignatureSpan">tap.Stdin.prototype.</span>main (cb)](#apidoc.element.tap.Stdin.prototype.main)
- description and source-code
```javascript
main = function (cb) {
  this.domain.add(this.stream)
  this.setTimeout(this.options.timeout)
  this.stream.pipe(this.parser)
  this.stream.resume()
  this.once('end', cb)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Stdin.prototype.threw"></a>[function <span class="apidocSignatureSpan">tap.Stdin.prototype.</span>threw (er, extra, proxy)](#apidoc.element.tap.Stdin.prototype.threw)
- description and source-code
```javascript
threw = function (er, extra, proxy) {
  extra = Base.prototype.threw.call(this, er, extra, proxy)
  this.options = extra
  this.parser.abort(er.message, extra)
  this.parser.end()
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tap.Test"></a>[module tap.Test](#apidoc.module.tap.Test)

#### <a name="apidoc.element.tap.Test.Test"></a>[function <span class="apidocSignatureSpan">tap.</span>Test (options)](#apidoc.element.tap.Test.Test)
- description and source-code
```javascript
function Test(options) {
  options = options || {}
  if (!(this instanceof Test))
    return new Test(options)

  Base.call(this, options)
  this.pushedEnd = false
  this.jobs = ownOr(options, 'jobs', 1)
  this.subtests = []
  this.pool = new Pool()
  this.queue = ['TAP version 13\n']
  this.noparallel = false
  this.cb = this.domain.bind(options.cb)
  this.occupied = false
  this.currentAssert = null
  this.count = 0
  this.n = 0
  this.ended = false
  this.explicitEnded = false
  this.multiEndThrew = false
  this.currentAssert = null
  this.assertAt = null
  this.assertStack = null
  this.planEnd = -1
  this.onBeforeEach = []
  this.onAfterEach = []
  this.ranAfterEach = false

  // bind all methods to this object, so we can pass t.end as a callback
  // and do 'var test = require('tap').test' like people do.
  var bound = Object.create(null)
  bindObj(this, this, bound)
  bindObj(this, Object.getPrototypeOf(this), bound)
  bindObj(this, Test.prototype, bound)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.super_"></a>[function <span class="apidocSignatureSpan">tap.Test.</span>super_ (options)](#apidoc.element.tap.Test.super_)
- description and source-code
```javascript
function Base(options) {
  this.start = 0
  this.hrtime = null
  this.time = null
  this.readyToProcess = false
  this.options = options
  this.parent = ownOr(options, 'parent', null)
  this.bail = ownOrEnv(options, 'bail', 'TAP_BAIL', true)
  this.name = ownOr(options, 'name', '')
  if (!this.name)
    this.name = ''
  else
    this.name = this.name.replace(/[\n\r\s\t]/g, ' ')
  this.indent = ownOr(options, 'indent', '')
  this.silent = !!options.silent
  this.buffered = !!options.buffered || !!options.silent
  this.finished = false
  this.strict = ownOrEnv(options, 'strict', 'TAP_STRICT', true)
  this.omitVersion = !!options.omitVersion
  this.preserveWhitespace = ownOr(options, 'preserveWhitespace', true)
  this.jobs = +ownOrEnv(options, 'jobs', 'TAP_JOBS') || 0
  this.skip = ownOr(options, 'skip', false)
  this.todo = ownOr(options, 'todo', false)
  this.setupParser(options)
  this.finished = false
  this.output = ''
  this.results = null
  this.bailedOut = false
  if (this.skip || this.todo)
    this.main = Base.prototype.main

  Readable.apply(this, options)

  domain.create().add(this)
  this.domain.on('error', this.threw.bind(this))

  if (typeof options.debug === 'boolean')
    this.debug = options.debug ? debug : nodebug
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tap.Test.prototype"></a>[module tap.Test.prototype](#apidoc.module.tap.Test.prototype)

#### <a name="apidoc.element.tap.Test.prototype.addAssert"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>addAssert (name, length, fn)](#apidoc.element.tap.Test.prototype.addAssert)
- description and source-code
```javascript
addAssert = function (name, length, fn) {
  if (!name)
    throw new TypeError('name is required for addAssert')

  if (!(typeof length === 'number' && length >= 0))
    throw new TypeError('number of args required')

  if (typeof fn !== 'function')
    throw new TypeError('function required for addAssert')

  if (Test.prototype[name] || this[name])
    throw new TypeError('attempt to re-define '' + name + '' assert')

  this[name] = function ASSERT () {
    if (!this.currentAssert) {
      this.currentAssert = ASSERT
    }
    var args = new Array(length + 2)
    for (var i = 0; i < length; i++) {
      args[i] = arguments[i]
    }
    if (typeof arguments[length] === 'object') {
      args[length] = ''
      args[length + 1] = arguments[length]
    } else {
      args[length] = arguments[length] || ''
      args[length + 1] = arguments[length + 1] || {}
    }

    return fn.apply(this, args)
  }
}
```
- example usage
```shell
...
// typically, a plugin would do this on a specific instance, eg on
// the root test harness instance.  but we do this here to add some
// useful prototype methods.

exports.decorate = decorate

function decorate (t) {
t.addAssert('ok', 1, function (obj, message, extra) {
  message = message || 'expect truthy value'
  if (obj) {
    return this.pass(message, extra)
  }

  return this.fail(message, extra)
})
...
```

#### <a name="apidoc.element.tap.Test.prototype.afterEach"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>afterEach (fn)](#apidoc.element.tap.Test.prototype.afterEach)
- description and source-code
```javascript
afterEach = function (fn) {
  this.onAfterEach.push(fn)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.autoend"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>autoend ()](#apidoc.element.tap.Test.prototype.autoend)
- description and source-code
```javascript
autoend = function () {
  this.options.autoend = true
  this.maybeAutoend()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.bailout"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>bailout (message)](#apidoc.element.tap.Test.prototype.bailout)
- description and source-code
```javascript
bailout = function (message) {
  if (this.parent && (this.results || this.ended))
    this.parent.bailout(message)
  else {
    this.process()
    message = message ? ' ' + ('' + message).trim() : ''
    message = message.replace(/[\r\n]/g, ' ')
    this.parser.write('Bail out!' + message + '\n')
  }
  this.end(IMPLICIT)
  this.process()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.beforeEach"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>beforeEach (fn)](#apidoc.element.tap.Test.prototype.beforeEach)
- description and source-code
```javascript
beforeEach = function (fn) {
  this.onBeforeEach.push(fn)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.comment"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>comment ()](#apidoc.element.tap.Test.prototype.comment)
- description and source-code
```javascript
comment = function () {
  var message = util.format.apply(util, arguments)
  message = '# ' + message.split(/\r?\n/).join('\n# ') + '\n'

  if (this.results)
    this.push(message)
  else
    this.queue.push(message)
  this.process()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.current"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>current ()](#apidoc.element.tap.Test.prototype.current)
- description and source-code
```javascript
current = function () {
  throw new Error('Test.current() as been removed and is no more')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.done"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>done (implicit)](#apidoc.element.tap.Test.prototype.done)
- description and source-code
```javascript
done = function (implicit) {
  this.debug('END implicit=%j', implicit === IMPLICIT)
  if (this.ended && implicit === IMPLICIT)
    return

  // beyond here we have to be actually done with things, or else
  // the semantic checks on counts and such will be off.
  if (!queueEmpty(this) || this.occupied) {
    if (!this.pushedEnd)
      this.queue.push(['end', implicit])
    this.pushedEnd = true
    return this.process()
  }

  if (!this.ranAfterEach && this.parent) {
    this.ranAfterEach = true
    this.parent.runAfterEach(this, end.bind(this, implicit))
  } else
    end.call(this, implicit)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.emitSubTeardown"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>emitSubTeardown (p)](#apidoc.element.tap.Test.prototype.emitSubTeardown)
- description and source-code
```javascript
emitSubTeardown = function (p) {
  try {
    p.emit('teardown')
  } catch (er) {
    delete p.options.time
    p.threw(er)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.end"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>end (implicit)](#apidoc.element.tap.Test.prototype.end)
- description and source-code
```javascript
end = function (implicit) {
  this.debug('END implicit=%j', implicit === IMPLICIT)
  if (this.ended && implicit === IMPLICIT)
    return

  // beyond here we have to be actually done with things, or else
  // the semantic checks on counts and such will be off.
  if (!queueEmpty(this) || this.occupied) {
    if (!this.pushedEnd)
      this.queue.push(['end', implicit])
    this.pushedEnd = true
    return this.process()
  }

  if (!this.ranAfterEach && this.parent) {
    this.ranAfterEach = true
    this.parent.runAfterEach(this, end.bind(this, implicit))
  } else
    end.call(this, implicit)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.endAll"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>endAll (sub)](#apidoc.element.tap.Test.prototype.endAll)
- description and source-code
```javascript
endAll = function (sub) {
  this.processing = true
  if (this.occupied) {
    var p = this.occupied
    if (p.endAll)
      p.endAll(true)
    else {
      p.parser.abort('test unfinished')
    }
  } else if (sub) {
    this.process()
    if (queueEmpty(this)) {
      var options = Object.keys(this.options).reduce(function (o, k) {
        o[k] = this.options[k]
        return o
      }.bind(this), {})
      this.options.at = null
      this.options.stack = ''
      options.test = this.name
      this.fail('test unfinished', options)
    }
  }
  if (this.promise && this.promise.tapAbortPromise)
    this.promise.tapAbortPromise()
  if (this.occupied) {
    this.queue.unshift(this.occupied)
    this.occupied = null
  }
  endAllQueue(this.queue)
  this.processing = false
  this.process()
  this.parser.end()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.fail"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>fail (message, extra)](#apidoc.element.tap.Test.prototype.fail)
- description and source-code
```javascript
function fail(message, extra) {
  if (!this.currentAssert) {
    this.currentAssert = fail
  }

  if (message && typeof message === 'object') {
    extra = message
    message = ''
  } else {
    if (!message) {
      message = ''
    }
    if (!extra) {
      extra = {}
    }
  }

  this.printResult(false, message, extra)

  var ret = true
  if (!extra.todo && !extra.skip)
    ret = false

  return ret
}
```
- example usage
```shell
...
function decorate (t) {
t.addAssert('ok', 1, function (obj, message, extra) {
  message = message || 'expect truthy value'
  if (obj) {
    return this.pass(message, extra)
  }

  return this.fail(message, extra)
})

t.addAssert('notOk', 1, function (obj, message, extra) {
  message = message || 'expect falsey value'
  return this.ok(!obj, message, extra)
})
...
```

#### <a name="apidoc.element.tap.Test.prototype.main"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>main (cb)](#apidoc.element.tap.Test.prototype.main)
- description and source-code
```javascript
main = function (cb) {
  this.setTimeout(this.options.timeout)
  this.debug('MAIN pre', this)

  var self = this
  try {
    var ret = this.cb(this)
  } catch (er) {
    this.threw(er)
  }

  if (ret && ret.then) {
    this.promise = ret
    ret.tapAbortPromise = done
    ret.then(end, done)
  } else
    done()

  function end () {
    self.debug(' > implicit end for promise')
    self.end(IMPLICIT)
    done()
  }

  function done (er) {
    if (er)
      self.threw(er)

    if (self.results || self.bailedOut)
      cb()
    else
      self.ondone = cb
  }

  this.debug('MAIN post', this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.maybeAutoend"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>maybeAutoend ()](#apidoc.element.tap.Test.prototype.maybeAutoend)
- description and source-code
```javascript
maybeAutoend = function () {
  if (this.autoendTimer)
    clearTimeout(this.autoendTimer)

  if (this.shouldAutoend()) {
    var self = this
    self.autoendTimer = setTimeout(function () {
      if (self.shouldAutoend()) {
        self.autoendTimer = setTimeout(function () {
          if (self.shouldAutoend()) {
            self.end(IMPLICIT)
          }
        })
      }
    })
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.onbufferedend"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>onbufferedend (p, er)](#apidoc.element.tap.Test.prototype.onbufferedend)
- description and source-code
```javascript
onbufferedend = function (p, er) {
  delete p.ondone
  p.results = p.results || {}
  p.readyToProcess = true
  var to = p.options.timeout
  if (to && p.passing())
    var dur = Date.now() - p.start
  if (dur && dur > to)
    p.timeout()
  else
    p.setTimeout(false)
  this.debug('%s.onbufferedend', this.name, p.name, p.results.bailout)
  this.pool.remove(p)
  p.options.tapChildBuffer = p.output || ''
  p.options.stack = ''
  if (p.time)
    p.options.time = p.time
  if (this.occupied === p)
    this.occupied = null
  if (er)
    this.threw(er)
  p.deferred.resolve(this)
  this.process()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.onindentedend"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>onindentedend (p, er)](#apidoc.element.tap.Test.prototype.onindentedend)
- description and source-code
```javascript
onindentedend = function (p, er) {
  delete p.ondone
  this.debug('onindentedend', p)
  this.noparallel = false
  var sti = this.subtests.indexOf(p)
  if (sti !== -1)
    this.subtests.splice(sti, 1)
  p.readyToProcess = true
  p.results = p.results || {}
  if (p.time)
    p.options.time = p.time
  var to = p.options.timeout
  if (to && p.passing())
    var dur = Date.now() - p.start
  if (dur && dur > to)
    p.timeout()
  else
    p.setTimeout(false)
  this.debug('onindentedend %s(%s)', this.name, p.name, er || 'ok')
  assert(this.occupied === p)
  this.occupied = null
  this.debug('OIE(%s) b>shift into queue', this.name, this.queue)
  p.options.stack = ''

  this.queue.unshift(['emitSubTeardown', p])
  this.printResult(p.passing(), p.name, p.options, true)

  this.debug('OIE(%s) shifted into queue', this.name, this.queue)
  if (er)
    this.threw(er)
  p.deferred.resolve(this)
  this.process()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.pass"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>pass (message, extra)](#apidoc.element.tap.Test.prototype.pass)
- description and source-code
```javascript
function pass(message, extra) {
  if (!this.currentAssert) {
    this.currentAssert = pass
  }
  this.printResult(true, message || '(unnamed test)', extra)
  return true
}
```
- example usage
```shell
...

exports.decorate = decorate

function decorate (t) {
t.addAssert('ok', 1, function (obj, message, extra) {
  message = message || 'expect truthy value'
  if (obj) {
    return this.pass(message, extra)
  }

  return this.fail(message, extra)
})

t.addAssert('notOk', 1, function (obj, message, extra) {
  message = message || 'expect falsey value'
...
```

#### <a name="apidoc.element.tap.Test.prototype.plan"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>plan (n, comment)](#apidoc.element.tap.Test.prototype.plan)
- description and source-code
```javascript
plan = function (n, comment) {
  if (this.bailedOut)
    return

  if (this.planEnd !== -1) {
    throw new Error('Cannot set plan more than once')
  }

  if (typeof n !== 'number' || n < 0) {
    throw new TypeError('plan must be a number')
  }

  // Cannot get any tests after a trailing plan, or a plan of 0
  var ending = false
  if (this.count !== 0 || n === 0) {
    ending = true
  }

  if (n === 0)
    this.skip = comment || true

  this.planEnd = n
  comment = comment ? ' # ' + comment.trim() : ''
  this.queue.push('1..' + n + comment + '\n')

  if (ending)
    this.end(IMPLICIT)
  else
    this.process()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.pragma"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>pragma (set)](#apidoc.element.tap.Test.prototype.pragma)
- description and source-code
```javascript
pragma = function (set) {
  var p = ''
  Object.keys(set).forEach(function (i) {
    p += 'pragma ' + (set[i] ? '+' : '-') + i + '\n'
  })
  this.queue.push(p)
  this.process()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.printResult"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>printResult (ok, message, extra, front)](#apidoc.element.tap.Test.prototype.printResult)
- description and source-code
```javascript
function pR(ok, message, extra, front) {
  var n = this.count + 1
  if (this.planEnd !== -1 && n > this.planEnd) {
    if (!this.passing())
      return

    var failMessage = this.explicitEnded
        ? 'test after end() was called'
        : 'test count exceeds plan'

    var er = new Error(failMessage)
    Error.captureStackTrace(er, this.currentAssert || pR)
    er.test = this.name
    er.plan = this.planEnd
    this.threw(er)
    return
  }

  extra = extra || {}

  if (this.assertAt) {
    extra.at = this.assertAt
    this.assertAt = null
  }

  if (this.assertStack) {
    extra.stack = this.assertStack
    this.assertStack = null
  }

  if (hasOwn(extra, 'stack') && !hasOwn(extra, 'at'))
    extra.at = stack.parseLine(extra.stack.split('\n')[0])

  var fn = this.currentAssert || pR
  this.currentAssert = null
  if (!ok && !extra.skip && !hasOwn(extra, 'at')) {
    assert.equal(typeof fn, 'function')
    extra.at = stack.at(fn)
    if (!extra.todo)
      extra.stack = stack.captureString(80, fn)
  }

  var diagnostic
  if (!ok)
    diagnostic = true

  if (extra.skip)
    diagnostic = false

  if (process.env.TAP_DIAG === '0')
    diagnostic = false

  if (typeof extra.diagnostic === 'boolean')
    diagnostic = extra.diagnostic

  if (diagnostic)
    extra.diagnostic = true

  this.count = n
  var res = { ok: ok, message: message, extra: extra }
  var output = new TestPoint(ok, message, extra)
  // when we jump the queue, skip an extra line
  if (front)
    output.message = output.message.trimRight() + '\n\n'

  if (front) {
    this.emit('result', res)
    this.parser.write(output.ok + (++this.n) + output.message)
  } else
    this.queue.push(['emit', 'result', res], output)

  if (this.planEnd === this.count)
    this.end(IMPLICIT)

  this.process()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.process"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>process ()](#apidoc.element.tap.Test.prototype.process)
- description and source-code
```javascript
process = function () {
  if (this.processing)
    return this.debug(' < already processing')

  this.debug('\nPROCESSING(%s)', this.name, this.queue.length)
  this.processing = true

  var p

  while (!this.occupied && (p = this.queue.shift())) {
    this.debug('PROCESS(%s)', this.name, p)
    if (p instanceof Base) {
      this.processSubtest(p)
    } else if (p === EOF) {
      this.debug(' > EOF', this.name)
      // I AM BECOME EOF, DESTROYER OF STREAMS
      this.parser.end()
    } else if (p instanceof TestPoint) {
      this.debug(' > TESTPOINT')
      this.parser.write(p.ok + (++this.n) + p.message)
    } else if (typeof p === 'string') {
      this.debug(' > STRING')
      this.parser.write(p)
    } else if (Array.isArray(p)) {
      this.debug(' > METHOD')
      var m = p.shift()
      this[m].apply(this, p)
    } else {
      throw new Error('weird thing got in the queue')
    }
  }

  while (!this.noparallel &&
         this.pool.length < this.jobs &&
         (p = this.subtests.shift())) {
    if (!p.buffered) {
      this.noparallel = true
      break
    }
    this.debug('start subtest', p)
    this.pool.add(p)
    if (this.bailedOut)
      this.onbufferedend(p)
    else
      this.runBeforeEach(p,
        p.main.bind(p,
          this.onbufferedend.bind(this, p)))
  }

  this.debug('done processing', this.queue, this.occupied)
  this.processing = false

  // just in case any tests ended, and we have sync stuff still
  // waiting around in the queue to be processed
  if (!this.occupied && this.queue.length)
    this.process()

  this.maybeAutoend()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.processSubtest"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>processSubtest (p)](#apidoc.element.tap.Test.prototype.processSubtest)
- description and source-code
```javascript
processSubtest = function (p) {
  this.debug(' > subtest')
  this.occupied = p
  if (!p.buffered) {
    if (this.bailedOut)
      return this.onindentedend(p)
    this.debug(' > subtest indented')
    p.pipe(this.parser, { end: false })
    this.runBeforeEach(p,
      this.writeSubComment.bind(this, p,
        p.main.bind(p,
          this.onindentedend.bind(this, p))))
  } else if (p.readyToProcess) {
    this.debug(' > subtest buffered, finished')
    // finished!  do the thing!
    this.occupied = null
    if (!p.passing() || !p.silent) {
      this.queue.unshift(['emitSubTeardown', p])
      this.printResult(p.passing(), p.name, p.options, true)
    }
  } else {
    this.occupied = p
    this.debug(' > subtest buffered, unfinished', p)
    // unfinished buffered test.
    // nothing to do yet, just leave it there.
    this.queue.unshift(p)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.runAfterEach"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>runAfterEach (who, cb)](#apidoc.element.tap.Test.prototype.runAfterEach)
- description and source-code
```javascript
runAfterEach = function (who, cb) {
  var self = this
  loop(who, self.onAfterEach, function () {
    if (self.parent)
      self.parent.runAfterEach(who, cb)
    else
      cb()
  }, who.threw)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.runBeforeEach"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>runBeforeEach (who, cb)](#apidoc.element.tap.Test.prototype.runBeforeEach)
- description and source-code
```javascript
runBeforeEach = function (who, cb) {
  var self = this
  if (this.parent)
    this.parent.runBeforeEach(who, function () {
      loop(who, self.onBeforeEach, cb, who.threw)
    })
  else
    loop(who, self.onBeforeEach, cb, who.threw)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.shouldAutoend"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>shouldAutoend ()](#apidoc.element.tap.Test.prototype.shouldAutoend)
- description and source-code
```javascript
shouldAutoend = function () {
  var should = (
    this.options.autoend &&
    !this.ended &&
    !this.occupied &&
    queueEmpty(this) &&
    !this.pool.length &&
    !this.subtests.length &&
    this.planEnd === -1
  )
  return should
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.spawn"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>spawn (cmd, args, options, name)](#apidoc.element.tap.Test.prototype.spawn)
- description and source-code
```javascript
function spawn(cmd, args, options, name) {
  if (typeof args === 'string') {
    args = [ args ]
  }

  args = args || []

  if (typeof options === 'string') {
    name = options
    options = {}
  }

  options = options || {}
  options.name = ownOr(options, 'name', name)
  options.command = cmd
  options.args = args

  return this.sub(Spawn, options, spawn)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.stdin"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>stdin (name, extra)](#apidoc.element.tap.Test.prototype.stdin)
- description and source-code
```javascript
function stdin(name, extra) {
  extra = parseTestArgs(name, extra, function () {}, '/dev/stdin')
  return this.sub(Stdin, extra || {}, stdin)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.sub"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>sub (Class, extra, caller)](#apidoc.element.tap.Test.prototype.sub)
- description and source-code
```javascript
sub = function (Class, extra, caller) {
  if (extra && (extra.todo || extra.skip)) {
    this.pass(extra.name, extra)
    return Promise.resolve(this)
  }

  extra.indent = '    '
  if (this.jobs > 1 && process.env.TAP_BUFFER === undefined)
    extra.buffered = ownOr(extra, 'buffered', true)
  else
    extra.buffered = ownOrEnv(extra, 'buffered', 'TAP_BUFFER', true)

  extra.bail = ownOr(extra, 'bail', this.bail)
  extra.parent = this
  extra.stack = stack.captureString(80, caller)
  var t = new Class(extra)

  this.queue.push(t)
  this.subtests.push(t)

  var d = new Deferred()
  t.deferred = d
  this.process()
  return d.promise
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.tearDown"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>tearDown (fn)](#apidoc.element.tap.Test.prototype.tearDown)
- description and source-code
```javascript
tearDown = function (fn) {
  this.on('teardown', fn)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.teardown"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>teardown (fn)](#apidoc.element.tap.Test.prototype.teardown)
- description and source-code
```javascript
teardown = function (fn) {
  this.on('teardown', fn)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.test"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>test (name, extra, cb)](#apidoc.element.tap.Test.prototype.test)
- description and source-code
```javascript
function test(name, extra, cb) {
  extra = parseTestArgs(name, extra, cb)
  return this.sub(Test, extra, test)
}
```
- example usage
```shell
...
  if (source.stack)
    target.stack = source.stack
  return false
}

return !(propertyName === 'todo' ||
propertyName === 'time' ||
/^_?tapChild/.test(propertyName) ||
/^tapStream/.test(propertyName) ||
/^tapMochaTest/.test(propertyName) ||
propertyName === 'cb' ||
propertyName === 'name' ||
propertyName === 'indent' ||
propertyName === 'skip' ||
propertyName === 'bail' ||
...
```

#### <a name="apidoc.element.tap.Test.prototype.threw"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>threw (er, extra, proxy)](#apidoc.element.tap.Test.prototype.threw)
- description and source-code
```javascript
threw = function (er, extra, proxy) {
  this.debug('THREW', er.message, extra, proxy)

  // event emitters 'error' events need to re-throw so that they
  // can jump out of the flow like a normal throw.  They'll just
  // end up back here once that happens, though, unless there's a
  // try/catch somewhere in the call stack.
  if (er.domainEmitter) {
    delete er.domainEmitter
    throw er
  }

  if (this.name && !proxy)
    er.test = this.name
  if (!proxy)
    extra = extraFromError(er, extra, this.options)
  Base.prototype.threw.call(this, er, extra, proxy)

  if (!this.results) {
    this.fail(extra.message || er.message, extra)
    if (!proxy)
      this.end(IMPLICIT)
  }
  this.process()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.timeout"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>timeout (options)](#apidoc.element.tap.Test.prototype.timeout)
- description and source-code
```javascript
timeout = function (options) {
  options = options || {}
  options.expired = options.expired || this.name
  if (this.occupied)
    this.occupied.timeout(options)
  else
    Base.prototype.timeout.call(this, options)
  this.end(IMPLICIT)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.Test.prototype.writeSubComment"></a>[function <span class="apidocSignatureSpan">tap.Test.prototype.</span>writeSubComment (p, cb)](#apidoc.element.tap.Test.prototype.writeSubComment)
- description and source-code
```javascript
writeSubComment = function (p, cb) {
  var comment = '# Subtest'
  if (p.name)
    comment += ': ' + p.name
  comment += '\n'
  this.parser.write(comment)
  cb()
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tap.asserts"></a>[module tap.asserts](#apidoc.module.tap.asserts)

#### <a name="apidoc.element.tap.asserts.decorate"></a>[function <span class="apidocSignatureSpan">tap.asserts.</span>decorate (t)](#apidoc.element.tap.asserts.decorate)
- description and source-code
```javascript
function decorate(t) {
  t.addAssert('ok', 1, function (obj, message, extra) {
    message = message || 'expect truthy value'
    if (obj) {
      return this.pass(message, extra)
    }

    return this.fail(message, extra)
  })

  t.addAssert('notOk', 1, function (obj, message, extra) {
    message = message || 'expect falsey value'
    return this.ok(!obj, message, extra)
  })

  t.addAssert('error', 1, function (er, message, extra) {
    if (!er) {
      return this.pass(message || 'should not error', extra)
    }

    if (!(er instanceof Error)) {
      extra.found = er
      return this.fail(message || 'non-Error error encountered', extra)
    }

    message = message || er.message
    extra.found = er
    return this.fail(message, extra)
  })

  t.addAssert('equal', 2, function (f, w, m, e) {
    m = m || 'should be equal'
    if (f === w) {
      return this.pass(m, e)
    }

    e.found = f
    e.wanted = w
    e.compare = '==='

    if (typeof f === 'object' &&
        typeof w === 'object' &&
        f &&
        w &&
        shallower(f, w)) {
      e.note = 'Objects never === one another'
    }

    return this.fail(m, e)
  })

  t.addAssert('not', 2, function (f, w, m, e) {
    m = m || 'should not be equal'
    if (f !== w) {
      return this.pass(m, e)
    }

    e.found = f
    e.doNotWant = w
    e.compare = '!=='

    return this.fail(m, e)
  })

  t.addAssert('same', 2, function (f, w, m, e) {
    m = m || 'should be equivalent'
    e.found = f
    e.wanted = w
    return this.ok(shallower(f, w), m, e)
  })

  t.addAssert('notSame', 2, function (f, w, m, e) {
    m = m || 'should not be equivalent'
    e.found = f
    e.doNotWant = w
    return this.notOk(shallower(f, w), m, e)
  })

  t.addAssert('strictSame', 2, function (f, w, m, e) {
    m = m || 'should be equivalent strictly'
    e.found = f
    e.wanted = w
    return this.ok(deeper(f, w), m, e)
  })

  t.addAssert('strictNotSame', 2, function (f, w, m, e) {
    m = m || 'should be equivalent strictly'
    e.found = f
    e.doNotWant = w
    return this.notOk(deeper(f, w), m, e)
  })

  t.addAssert('match', 2, function (f, w, m, e) {
    m = m || 'should match pattern provided'
    e.found = f
    e.pattern = w
    return this.ok(tmatch(f, w), m, e)
  })

  t.addAssert('notMatch', 2, function (f, w, m, e) {
    m = m || 'should not match pattern provided'
    e.found = f
    e.pattern = w
    return this.ok(!tmatch(f, w), m, e)
  })

  t.addAssert('type', 2, function (obj, klass, m, e) {
    var name = klass
    if (typeof name === 'function') {
      name = name.name || '(anonymous constructor)'
    }
    m = m || 'type is ' + name

    // simplest case, it literally is the same thing
    if (obj === klass) {
      return this.pass(m, e)
    }

    var type = typeof obj
    if (!obj && type === 'object') {
      type = 'null'
    }

    if (type === 'object' && klass !== 'object') {
      if (typeof klass === 'function') {
        e.found = Object.getPrototypeOf(obj).constructor.name
        e.wanted = name
        return this.ok(obj instanceof klass, m, e)
      }

      // check prototype chain for name
      // at this point, we already know klass is not a function
      // if the klass specified is an obj in the proto chain, pass
      // if the name specified is the name of a ctor in the chain, pass
      var p = obj
      do {
        var ctor = p.constructor && p.constructor.name
        if (p === klass || ctor === name) {
          return this.pass(m, e)
        }
        p = Object.getPrototypeOf(p)
      } while (p)
    }

    return this.equal(type, name, m, e)
  })

  t.addAssert('throws', 4, function (fn_, wanted_, m_, e_, m, e__) {
    var fn, wanted, e
    for (var i = 0; i < arguments.length - 1; i++) {
      var arg = arguments[i]
      if (typeof arg === 'function') {
        if (arg === Error || arg.prototype instanceof Error) {
          wanted = arg
        } else if (!fn) {
          fn = arg
        }
      } else if (typeof arg === 'string' && arg) {
        m = arg
      } else if (typeof arg === 'object') {
        if ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tap.mocha"></a>[module tap.mocha](#apidoc.module.tap.mocha)

#### <a name="apidoc.element.tap.mocha.after"></a>[function <span class="apidocSignatureSpan">tap.mocha.</span>after (name, fn)](#apidoc.element.tap.mocha.after)
- description and source-code
```javascript
function after(name, fn) {
  var suite = suiteStack[ suiteStack.length - 1 ]
  if (!suite)
    throw new Error('cannot call "after" outside of describe()')
  if (fn)
    suite.after.push([name, fn])
  else
    suite.after.push([name])
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.mocha.afterEach"></a>[function <span class="apidocSignatureSpan">tap.mocha.</span>afterEach (fn)](#apidoc.element.tap.mocha.afterEach)
- description and source-code
```javascript
function afterEach(fn) {
  moment('afterEach', fn)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.mocha.before"></a>[function <span class="apidocSignatureSpan">tap.mocha.</span>before (name, fn)](#apidoc.element.tap.mocha.before)
- description and source-code
```javascript
function before(name, fn) {
  if (typeof name === 'function')
    fn = name, name = null
  if (fn && fn.name && !name)
    name = fn.name
  var todo = !fn
  var suite = suiteStack[ suiteStack.length - 1 ]
  var t = tapStack[ tapStack.length - 1 ]
  if (!name)
    name = ''
  t.test(name, { todo: todo, silent: true }, function (tt) {
    var ret = fn.call(suite, done(tt))
    if (!ret && fn.length === 0)
      tt.end()
    else
      return ret
  })

  function done (tt) { return function (er) {
    if (er)
      tt.threw(er)
    else
      tt.end()
  }}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.mocha.beforeEach"></a>[function <span class="apidocSignatureSpan">tap.mocha.</span>beforeEach (fn)](#apidoc.element.tap.mocha.beforeEach)
- description and source-code
```javascript
function beforeEach(fn) {
  moment('beforeEach', fn)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.mocha.context"></a>[function <span class="apidocSignatureSpan">tap.mocha.</span>context (name, fn)](#apidoc.element.tap.mocha.context)
- description and source-code
```javascript
function describe(name, fn) {
  new Suite(name, fn)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.mocha.describe"></a>[function <span class="apidocSignatureSpan">tap.mocha.</span>describe (name, fn)](#apidoc.element.tap.mocha.describe)
- description and source-code
```javascript
function describe(name, fn) {
  new Suite(name, fn)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.mocha.global"></a>[function <span class="apidocSignatureSpan">tap.mocha.</span>global ()](#apidoc.element.tap.mocha.global)
- description and source-code
```javascript
global = function () {
  Object.keys(exports).forEach(function (g) {
    global[g] = exports[g]
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.mocha.it"></a>[function <span class="apidocSignatureSpan">tap.mocha.</span>it (name, fn)](#apidoc.element.tap.mocha.it)
- description and source-code
```javascript
function it(name, fn) {
  if (typeof name === 'function')
    fn = name, name = null
  if (fn && fn.name && !name)
    name = fn.name
  var todo = !fn
  var suite = suiteStack[ suiteStack.length - 1 ]
  var t = tapStack[ tapStack.length - 1 ]
  if (!name)
    name = ''
  t.test(name, { todo: todo, tapMochaTest: true }, function (tt) {
    var ret = fn.call(tt, done(tt))
    if (ret && ret.then)
      return ret
    else if (fn.length === 0)
      tt.end()
  })

  function done (tt) { return function (er) {
    if (er)
      tt.threw(er)
    else
      tt.end()
  }}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.tap.mocha.specify"></a>[function <span class="apidocSignatureSpan">tap.mocha.</span>specify (name, fn)](#apidoc.element.tap.mocha.specify)
- description and source-code
```javascript
function it(name, fn) {
  if (typeof name === 'function')
    fn = name, name = null
  if (fn && fn.name && !name)
    name = fn.name
  var todo = !fn
  var suite = suiteStack[ suiteStack.length - 1 ]
  var t = tapStack[ tapStack.length - 1 ]
  if (!name)
    name = ''
  t.test(name, { todo: todo, tapMochaTest: true }, function (tt) {
    var ret = fn.call(tt, done(tt))
    if (ret && ret.then)
      return ret
    else if (fn.length === 0)
      tt.end()
  })

  function done (tt) { return function (er) {
    if (er)
      tt.threw(er)
    else
      tt.end()
  }}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.tap.stack"></a>[module tap.stack](#apidoc.module.tap.stack)

#### <a name="apidoc.element.tap.stack._wrapCallSite"></a>[function <span class="apidocSignatureSpan">tap.stack.</span>_wrapCallSite (frame)](#apidoc.element.tap.stack._wrapCallSite)
- description and source-code
```javascript
function wrapCallSite(frame) {
  if(frame.isNative()) {
    return frame;
  }

  // Most call sites will return the source file from getFileName(), but code
  // passed to eval() ending in "//# sourceURL=..." will return the source file
  // from getScriptNameOrSourceURL() instead
  var source = frame.getFileName() || frame.getScriptNameOrSourceURL();
  if (source) {
    var line = frame.getLineNumber();
    var column = frame.getColumnNumber() - 1;

    // Fix position in Node where some (internal) code is prepended.
    // See https://github.com/evanw/node-source-map-support/issues/36
    if (line === 1 && !isInBrowser() && !frame.isEval()) {
      column -= 62;
    }

    var position = mapSourcePosition({
      source: source,
      line: line,
      column: column
    });
    frame = cloneCallSite(frame);
    frame.getFileName = function() { return position.source; };
    frame.getLineNumber = function() { return position.line; };
    frame.getColumnNumber = function() { return position.column + 1; };
    frame.getScriptNameOrSourceURL = function() { return position.source; };
    return frame;
  }

  // Code called using eval() needs special handling
  var origin = frame.isEval() && frame.getEvalOrigin();
  if (origin) {
    origin = mapEvalOrigin(origin);
    frame = cloneCallSite(frame);
    frame.getEvalOrigin = function() { return origin; };
    return frame;
  }

  // If we get here then we were unable to change the source position
  return frame;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
