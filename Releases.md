### 0.145.0 / 2022.06.23

- fix(wasi): Fix WASI initialize() (#2372)
- feat(encoding): add json/stream.ts (#2231)
- feat(flags): infer argument types, names and defaults (#2180)
- feat(media_types): Improve contentType type definition (#2357)
- feat(node): add missing modules node/util/types.ts node/diagnostics_channel.ts
  (#2369)
- fix(encoding/csv/stream): properly handle CR characters (#2325)
- fix(http): Disable `console.error` if `opts.quiet` is true (#2379)
- fix(node): make performance object event target (#2371)
- fix(testing/bdd): fix flat test grouping context (#2308)
- node: improve error for unsupported import (#2380)

### 0.144.0 / 2022.06.15

- Add warning on usage of collections/mod.ts (#2321, #2346)
- encoding: add front matter module (#2335)
- feat(node): add missing TTY methods to stdout,stderr (#2337)
- fix: update ci script and fix type errors (#2344)

### 0.143.0 / 2022.06.09

- BREAKING feat(http): improve type safety and docs for http_status (#2297)
- BREAKING(flags): introduce negatable option (#2301)
- feat(encoding): add unsigned LEB128 varint encoding (#2265)
- feat(node/assert): add deepEqual and notDeepEqual (#2288)
- fix(dotenv): support inline comment (#2316)
- fix(media_types): work around type issues under Node.js (#2304)
- fix: pass resolved ephemeral port to onListen (#2311)

### 0.142.0 / 2022.06.02

- feat(crypto): add fnv algorithms (#2200)
- feat: add media_types (#2286)
- fix(node): type checking on AsyncResource (#2289)
- fix: assertSnapshot errors on empty snapshot in non-update mode (#2269)
- fix: put TextLineStream CR handling behind option (#2277)

### 0.141.0 / 2022.05.27

- BREAKING(flags): introduce `collect` option (#2247)
- BREAKING(testing): use Object.is() for strict equality (#2244)
- BREAKING(testing/asserts): remove implicit any types from assert signatures.
  (#2203)
- feat(http/util): add compareEtag (#2259)
- feat(node/crypto): stub out missing exports (#2263)
- feat(node/dns): `NAPTR`, `NS`, `CAA`, and `SOA` support (#2233)
- feat(streams): toTransformStream (#2227)
- feat(streams/delimiter): support `\r` in `TextLineStream` (#2267)
- feat(streams/merge): earlyZipReadableStreams (#2264)
- feat(testing/asserts): return error from `assertRejects` and `assertThrows`
  (#2226)
- fix(async/pooledMap): return ordered result (#2239)
- fix(node/fs): export fs.ReadStream (#2253)

### 0.140.0 / 2022.05.18

- feat(http): add onListen option to serve (#2218)
- feat(node/dgram): support dgram (udp) node module compat (#2205)
- fix(assertRejects): fails on synchronous throw #1302 (#2234)
- fix(collections): prevent cycles in deepMerge() (#2228)
- fix(encoding/csv): improve error message for csv's parse function (#2191)
- fix(http/file_server): fix handling of 'W/' prefixed etag (#2229)
- fix(testing/bdd): support using bdd tests with dnt (#2235)
- fix: add toJSON to node/perf_hooks.ts (#2209)

### 0.139.0 / 2022.05.12

- feat(encoding): add jsonc parser (#2154)
- feat(node/dns): Implement Resolver APIs (#2201)
- feat(node/net): unix domain socket support (#2146)
- feat(testing/snapshot): add "assertSnapshot" options overload (#2179)
- fix(node/module): interpret length parameter as optional in blitBuffer (#2199)
- fix(node/timers): set custom promisify function (#2198)

### 0.138.0 / 2022.05.05

- fix: Export equalSimd and equalsNaive (#2187)
- BREAKING(testing/snapshot): change multiline string serialization (#2166)
- feat(node/dns): support dns promises lookup (#2164)
- feat(testing): assertFalse (#2093)
- fix(node/dns): export more types (#2185)
- fix(node/worker_threads): Don't wait for parent message in web worker (#2182)
- fix(testing): Compare circular objects (#2172)

### 0.137.0 / 2022.04.28

- feat(testing): infer stub and spy return types from properties (#2137)
- fix(http): export interface ServeTlsInit (#2148)
- fix(node): use Web Crypto API via globalThis (#2115)
- fix(wasi): ContextOptions is an optional argument (#2138)
- http: serve() should log where it is listening (#1641)

### 0.136.0 / 2022.04.21

- feat(testing): Implement "assertSnapshot" (#2039)
- feat(testing): add TestContext argument to "it" function (#2117)
- fix(http): use the `addEventListener` method instead of `onabort` properties
  (#2124)
- fix(node/crypto): fix randomInt (#2101)
- perf(http): optimize file server (#2116)

### 0.135.0 / 2022.04.14

- BREAKING(io/readers): use an array as a MultiReader constructor parameter to
  avoid Maximum call stack size exceeded (#2016)
- BREAKING(mime/multipart): deprecate mime/multipart module (#2105)
- BREAKING(testing/bench): deprecate testing/bench module (#2104)
- feat(node): `Duplex.fromWeb` (#2086)
- feat(testing): add behavior-driven development (#2067)
- feat(testing): add utility for faking time (#2069)
- fix(node): Make global.ts evaluate synchronously (#2098)

### 0.134.0 / 2022.04.07

- feat(node/child_process): support `signal` parameter for `ChildProcess.kill`
  (#2083)
- feat(node/net): add server.ref/unref methods (#2087)
- feat: web streams based encoding/csv (#1993)
- fix(log): fix log formatter issue (#2070)
- fix(node/fs): fix writing redundant data (#2076)

### 0.133.0 / 2022.03.31

- BREAKING: improve bytes/ module (#2074)
- feat(testing): add mocking utilities (#2048)

### 0.132.0 / 2022.03.25

- feat(collections): Add BSTree and RBTree (#2023)
- feat(node): add ReadStream and createReadStream (#1435)
- feat(node): export URLSearchParams via url module (#2056)

### 0.131.0 / 2022.03.24

- feat(node): add NodeEventTarget (#2032)
- feat(node): add Console constructor (#2037)
- feat(node): worker_threads (#1151)
- feat(node): add process.allowedNodeEnvironmentFlags (#2049)
- feat(collections): add BinaryHeap (#2022)
- feat(async): expose asyncPromise and asyncAsyncIterable (#2034)
- fix(node/http): ignore error from `respondWith` (#2058)
- fix(node): warn on non supported event, but still register listener (#2050)
- fix(node): fix `EventEmitter` methods (#2035)
- fix(node): make global.<timerFunc> Node.js timers (#2038)

### 0.130.0 / 2022.03.16

- feat(testing): add `assertInstanceOf` (#2028)
- feat(node): shim get-caller-file (#2029)
- fix(node): fix dynamic require (#2024)
- feat(node/fs): add `fs.writevSync(fd, buffers[, position])` (#2020)

### 0.129.0 / 2022.03.10

- feat: streams based `Buffer` (#1970)
- feat(node/crypto): add crypto.publicEncrypt (#1987)
- feat(node/fs): add `fs.writev(fd, buffers[, position], callback)` (#2008)
- feat(streams): LimitedTransformStream & LimitedBytesTransformStream (#2007)
- feat(streams): TextDelimiterStream (#2006)
- feat(testing/asserts): use assertion signature for "assertStrictEquals"
  (#1984)
- fix(async): re-export abortable in mod.ts (#1959)
- fix(fmt/colors): update `ANSI_PATTERN` (#1996)
- fix(node): fix http.request for minipass-fetch 2.x (#2004)
- fix(node/process): ignore SIGBREAK binding when the platform is not windows
  (#2014)
- fix(testing): Misleading assertion error in assertNotEquals (#1989)

### 0.128.0 / 2022.03.03

- feat(node): add crypto.webcrypto (#1961)
- feat(streams): TextLineStream (#1978)
- fix(dotenv): avoid top-level-await in load.ts (#1964)
- fix(node): fix http client reqs with bodies (#1983)
- fix(testing): fix assertObjectMatch for RegExp/Map/Set (#1967)

### 0.127.0 / 2022.02.24

- feat(async): add `abortable` to async module. (#1939)
- feat(dotenv): add dotenv library (#1877)
- feat(http): expose serveDir function from file_server.ts (#1944)
- feat(node): add fs.realpath.native (#1951)
- feat(node/tls): basic support of tls.createServer (#1948)
- feat(testing): add `assertAlmostEquals` (#1906)
- fix(node): don't use globalThis.setTimeout types in node/timers (#1934)

### 0.126.0 / 2022.02.17

- feat(node): add tls.connect (#1923)
- fix(collections/group_by): improve type safety (#1880)
- fix(io/buffer): super and initialized prop (#1917)
- fix(node): add networkInterfaces to unstable (#1904)
- fix(node): fix fs.createWriteStream (#1874)
- fix(node): fix fs.write again, enable more test cases (#1892)
- fix(node): support 6-arg fs.write (#1888)
- fix(node/buffer): fix base64 decode (#1885)
- fix(node/module): fix commonjs wrapper (#1902)

### 0.125.0 / 2022.02.03

- feat(node): add punycode module (#1857)
- feat(node): add url.resolve (#1851)
- feat(node/child_process): add support for AbortSignal in ChildProcess (#1864)
- feat(node/fs): add fs.createWriteStream (#1859)
- fix(node/fs): fix fs.access when the user owns the file (#1869)
- fix(node/fs): fix fs.copyFile (support 4-arg call) (#1872)
- fix(node/http): fix http.request (#1856)
- fix(node/net): mock response.socket object (#1858)
- fix: bypass TS errors for missing --unstable (#1819)

Note 0.124.0 is the same as 0.125.0 but ignoring a typescript error related to a
new feature added setNoDelay.

### 0.123.0 / 2022.01.27

- feat(node): add os.networkInterfaces (#1846)
- feat(node): add process.uptime (#1853)
- feat(node/child_process): add execFile (#1838)
- fix(node/process): can not pass exit code as a string (#1849)
- fix(testing): `assertObjectMatch` matches ArrayBuffer views correctly (#1843)

### 0.122.0 / 2022.01.20

- BREAKING(encoding/csv): add return type to csv's parse and remove a parse func
  from args (#1724)
- feat(node): add Timeout class (#1699)
- feat(node): provide node compatible timer APIs in commonjs wrapper (#1834)
- fix(log): flush to file when buffer is full (#1782)
- fix(node): fix fs.write/fs.writeAll (#1832)
- fix(node): make stdio streams optional if not present on Deno namespace
  (#1829)
- fix(node/net): setNoDelay and setKeepAlive no-ops (#1828)
- fix(node/timers): work around |this| check in deno (#1827)

### 0.121.0 / 2022.01.12

- feat(crypto): add md4 hash (#1799)
- feat(http): add eyecandy to file_server (#1804)
- feat(http/file_server): add 'quiet' flag (#1773)
- feat(node): add zlib (#1790)
- feat(node): mock more APIs (#1802)
- feat(node): upstream caller-path package (#1801)
- feat(node/fs): fs.write()/fs.writeSync() (#1817)
- fix(node): placeholder process.getgid() (#1814)
- fix(node): process.env ownPropertyDescriptor (#1795)
- fix(node): set prototype for Module (#1797)
- fix(node/http): client emit response, trailers & abort (#1809)
- fix(node/http/client): convert response's Headers to plain Object (#1811)
- fix(node/url): format auth/search/hash corruption (#1810)

### 0.120.0 / 2022.01.05

- feat(crypto): add Tiger hash (#1749)
- feat(node): add https.request (#1746)
- feat(node): add process.execPath (#1748)
- feat(node): add vm.runInThisContext (#1747)
- feat(uuid): add function to detect RFC version of a UUID (#1766)
- fix(examples/chat): fix applyState call (#1760)
- fix(node): don't emit exit twice (#1753)
- fix(node): fix fs.readdir (#1758)
- fix(node): improve util.isDeepStrictEqual (#1765)
- fix(node/child_process): allow number and boolean env vars (#1762)
- fix(path): change default of 'extended' options of glob methods (#1719)
- fix(testing/assert): inequality of -0 and 0 (#1783)

### 0.119.0 / 2021.12.22

- feat(hash): add Tiger hash (#1729)
- feat(node): expose util.debuglog (#1735)
- feat(node/util): implement `getOwnNonIndexProperties` (#1728)
- feat(uuid): add `validate` function to check UUID (#1720)

### 0.118.0 / 2021.12.16

- [BREAKING] Remove 'findLast' from 'collections' module (#1527)
- [BREAKING] Remove 'findLastIndex' from 'collections' module (#1528)
- [BREAKING] Remove 'server_legacy' from 'http' module (#1648)
- [BREAKING] Remove 'ws' module (#1647)
- [BREAKING] Remove assertThrowsAsync from 'testing/' (#1646)
- [BREAKING] Remove Go-style address in 'http' module (#1660)
- [BREAKING] Remove onSignal from 'signals/' (#1644)
- feat(http): add onError option to serveListener and serveTls (#1679)
- feat(node): add child_process.fork (#1695)
- feat(node): add http.Agent (#1706)
- feat(node): add http.OutgoingMessage (#1705)
- feat(node): add http.request (#1712)
- feat(node): add missing url.parse (#1667)
- feat(node): add mock inspector module (#1688)
- feat(node): add mock zlib module (#1698)
- feat(node): add util.isDeepStrictEqual (#1556)
- feat(node): export fs.Stats class (#1696)
- feat(node/fs): add fs.access (#1687)
- feat(node/url): add url.resolveObject (#1691)
- feat(node/util): add util.deprecate (#1697)
- feat(toml): align keys by option (#1693)
- fix(datetime): fix bug for parse at the end of the month (#1676)
- fix(node/util/inspect): validate invalid options (#1672)
- fix(toml): parse declaration correctly (#1682)

### 0.117.0 / 2021.12.03

- feat(http): introduce onError option on ServerInit (#1621)
- feat(node/readline): Interface, createInterface (#1554)
- fix(node): use async read for stdin (#1653)
- fix(std/node): Add base64url encoding support, indexOf, lastIndexOf and
  includes to Buffer (#1636)
- test(node/fs): enable `test-fs-rm.js` (#1632)
- fix(node/util/inspect): Fix some bugs (#1637)
- fix(node): Use upstream implementation for streams (#1634)

### 0.116.0 / 2021.11.24

- feat(node/os): implement os.hostname() (#1631)
- feat(node/util): add `util.inspect` (#1592)
- fix(fmt/printf): print with rounding taken into account (#1623)
- fix(node/http): ignore server request parse errors (#1624)
- refactor(node): reorganize _next_tick.ts module (#1608)

### 0.115.1 / 2021.11.17

- fix(node): use old "process.nextTick" polyfill if Deno.core is not available
  (#1612)

### 0.115.0 / 2021.11.17

- feat(node): add wasi module (#1534)
- feat(node): process.config, process.exitCode, process._exiting (#1597)
- feat(node): process.stdin.setRawMode (#1572)
- feat(node/_fs): Add `fs.readSync` (#1598)
- feat(node/fs): add `fs.read` API (#1557)
- feat(node/fs): implement `fs.rm` and `fs.rmSync` (#1568)
- feat(node/process): add process.hrtime.bigint() (#1600)
- feat(node/util): Add `util.isBuffer` and `util._extend` (#1567)
- fix(node): Align exports and declarations for Buffer and Events module (#1570)
- fix(node): improve http.Server.listen() compat (#1574)
- fix(node/http): fix no body chunked response (#1603)
- fix(node/http): improve http.Server compatibility (#1595)
- fix(node/http): improve http.Server#close() compat (#1602)
- fix(node/util): improve test coverage (#1591)
- node: add nextTick helper module (#1584)
- node: polyfill process.nextTick using Deno.core bindings (#1588)
- node: Use upstream source for "events" module (#1558)

### 0.114.0 / 2021.11.09

- BREAKING(http): update `serve`, add `serveListener`, deprecate
  `listenAndServe` (#1506)
- BREAKING(std/collections): deprecate findLast (#1532)
- feat(http/file_server): add streaming support, fix empty file handling (#1479)
- feat(node): add readline module (#1453)
- feat(node): process.on and process.off for signals (#1466)
- feat(node/_fs): Add watchFile function (#1483)
- feat(node/http): HTTP Server/Response improvements (#1448)
- feat(node/querystring): implement qs.unescapeBuffer (#1516)
- feat(node): mock 'vm' module (#1501)
- feat(node): os.cpus() (#1500)
- feat(node): process.execArgv (#1499)
- fix(collections): prevent calling `Object.prototype.__proto__` in
  collections/deep_merge.ts (#1504)
- fix(collections): remove default selector for `findSingle` (#1232)
- fix(crypto/digest): always return the underlying ArrayBuffer (#1515)
- fix(http/file_server): don't require --allow-read for showing help message
  (#1521)
- fix(node): //@ts-ignore Error.captureStackTrace (#1533)
- fix(node): add proper module.export for 'module' (#1497)
- fix(node): child_process stdio for binary data (#1477)
- fix(node): fix flaky downloadFile test (#1460)
- fix(node): fix process.arch (#1498)
- fix(node): fix string representation of node errors (#1470)
- fix(node): isAlreadyClosed for child_process (#1469)
- fix(node/_tools): Better error and output logging (#1492)
- fix(node/_util): Deno.permissions is no longer called unless it exists.
  (#1520)
- fix(node/events): enable remaining tests for EventEmitter (#1489)
- fix(node/events): make EventEmitter's public methods enumerable (#1530)
- fix(node/process): warn on not implemented event instead of throw (#1510)
- fix(node/querystring): improve `querystring.parse` (#1473)
- fix(node/querystring): Improve querystring.stringify (#1488)
- fix(node/querystring/stringify): invalid surrogate pair throws URIError
  (#1505)
- fix(node/querystring/stringify): Remove initialValue (#1494)
- fix(signal): update signal module for canary API change (#1468)
- fix(testing): show special characters in assertEquals results (#1450)

### 0.113.0 / 2021.10.25

- feat(collections/running_reduce): support `currentIndex` (#1431)
- feat(http/file_server): add color to log message (#1434)
- feat(http/file_server): add breadcrumbs navigation (#1433)
- feat(node): allow require with 'node:' prefix (#1438)
- feat(node/url): add `url.urlToHttpOptions(url)` (#1426)
- feat(testing): add assertIsError (#1376)
- fix(async): fix async/tee concurent .next calls error (#1425)
- fix(crypto): support length option in crypto.subtle.digest (#1386)
- fix(http/file_server): fix encoded url in dir html (#1442)
- fix(http/file_server): fix leak file resource (#1443)
- fix(node): match Node's os.arch values (#1440)
- fix(node): show warning when using import/export in CJS module (#1452)
- fix(node/events): make on and emit methods callable by non-EventEmitter
  objects (#1454)
- fix(node/util): improve util.format (#1181)
- fix(node/_tools): fix node test setup script (#1422)
- chore(node): update Node version from 16.11.1 to 16.12.0 (#1441)

### 0.112.0 / 2021.10.18

- feat(collections): add joinToString (#1223)
- feat(node): CJS-ESM integration (#1412)
- feat(node): add helpers for determining CJS/ESM loader (#1407)
- feat(node): barebones express compatibility (#1398)
- feat(node): define process.mainModule (#1400)
- feat(node/events): implement setMaxListeners (#1414)
- feat(node/http): request & response streams (#1403)
- feat(node/os): add devNull constant (#1397)
- feat(node/url): add `url.format(URL[, options])` (#1420)
- fix(datetime): fix dayOfYear for the southern hemisphere (#1384)
- fix(fs/expand_glob): don't parse root as glob (#1417)
- fix(node): 'Illegal invocation' in 'perf_hooks' module (#1410)
- fix(node): add 'module' to native modules polyfill (#1408)
- fix(node): declare 'global' types inline (#1409)
- fix(node): export util.format() (#1401)
- fix(node): require doesn't throw error (#1399)
- fix(node): use hardcoded versions (#1406)
- fix(std/io): fix readline when catch BufferFullError (#1377)
- fix(testing): improve assertObjectMatch (#1419)
- chore(node): upgrade Node.js version from 15.5.1 to 16.11.1 (#1405)

### 0.111.0 / 2021.10.12

- BREAKING(fs): deprecate exists and existsSync (#1364)
- BREAKING(hash): deprecate std/hash (#1350)
- BREAKING(io): reorganize modules (#813)
- feat: streams utilities (#1141)
- feat(node): Add dns and net modules (#1375)
- feat(node): first iteration of http (#1383)
- feat(node): update built-in modules in node/module.ts (#1378)
- feat(node/crypto): add randomFillSync an randomFill (#1340)
- feat(node/crypto): add randomInt (#1356)
- feat(node/http): Export STATUS_CODES and METHODS (#1357)
- feat(node/url): add support for UNC path (#1365)
- fix(async/delay): reject if signal is already aborted (#1363)
- fix(encoding/base64url): allow passing strings to `encode` (#1361)
- fix(node): typo from #1380 (#1381)
- fix(node/url): improve compatibility of fileURLToPath (#1342)
- perf(bytes): switch equals to simd for large byte arrays (#1349)

### 0.110.0 / 2021.10.04

- feat(node): add missing modules (#1337)
- feat(node): support `Buffer.readUIntLE` (#1326)
- feat(node/buffer): support `Buffer.readUIntBE` (#1321)
- feat(node/crypto): add `scrypt` and `scryptSync` (#1329)
- feat(node/crypto): add `timingSafeEqual` (#1333)
- feat(node/stream/web): export more APIs (#1338)
- feat(std/node): add back os.tmpdir() implementation (#1308)
- feat(std/node/crypto): Add `crypto.randomUUID` (#1332)

### 0.109.0 / 2021.09.28

- feat(std/node/stream): add partial support for `stream/web` (#1297)
- fix(node/_tools): use denoflate to decompress Node test folder (#1299)
- fix(node/events): make `EventEmitter.call` compatible with es5 (#1315)
- fix(std/node/module): treat .mjs files as ESM (#1301)
- perf(crypto): reduce one mircotask (#1307)

### 0.108.0 / 2021.09.21

- fix: use `strict-ts44.tsconfig.json` on release tests (#1278)
- fix(collections): improve handling of arrays containing undefined (#1282)
- feat(testing/asserts): add `assertThrows()` overload to receive error (#1219)
- feat(std/node): add `ParsedUrlQuery` to `querystring` (#1229)
- feat(collections): use function overloading (#1286)
- chore(node/events): remove unnecessary `@ts-ignore` comments (#1280)
- docs(collections): add browser-compatibility comment (#1285)
- docs(encoding): add hex docs (#1287)
- docs(collections): replace console.assert with assertEquals (#1293)

### 0.107.0 / 2021.09.14

- BREAKING(http): cookie headers as params (#1041)
- feat(collection): add findSingle (#1166)
- feat(collections): Add `associatewith` (#1213)
- feat(collections): add `runningReduce` (#1226)
- feat(collections): add `sample` API (#1212)
- feat(collections): add dropWhile (#1185)
- feat(collections): add maxWith (#1170)
- feat(collections): add minWith (#1169)
- feat(collections): add reduceGroups (#1187)
- feat(collections): add slidingWindows (#1191)
- feat(io/streams): propagate cancel in readableStreamFromIterable() (#1274)
- fix(collections/includesValue): prevent enumerable prototype check (#1225)
- fix(testing/asserts): export Constructor type (#1208)
- fix(tests/yaml): expect !!js/function parse/stringify to throw (#1276)
- fix: update to latest signal API changes
- security(encoding/yaml): disable functions (#1275)

### 0.106.0 / 2021.08.23

- feat(async): add abort signal to delay (#1130)
- feat(collection): find_last_index to return undefined on no index found
  (#1072)
- feat(node/buffer): add missing exports (#1140)
- feat(node/buffer): export atob and btoa (#1147)
- fix(node/perf-hooks): add PerformanceEntry to default export (#1152)
- fix(testing): `assertEquals` now considers constructors equal if one is
  nullable and the other is Object (#1159)
- perf(collections): permutations optimisation (#1132)

### 0.105.0 / 2021.08.16

- docs(collections): fix typo in collections docs (#1127)
- feat(collections): compile time guarantee on pure functions (#1119)
- fix: type check examples in README files (#1121)
- fix(collections): intersect does not handle duplicate values in head properly
  (#1131)
- fix(crypto): make crypto bench depend on sibling version of testing module
  (#1135)
- refactor(bytes): rename `contains` to `includes` with optional argument
  `fromIndex` (#1133)

### 0.104.0 / 2021.08.10

- feat: Add `collections` module (#993, #1075, #1103, #1062, #1062, #1109,
  #1108, #1071, #1069, #1104, #1097, #1110, #1116)
- feat(crypto): add std/crypto wrapping and extending runtime WebCrypto (#1025)
- feat(http/file_server): return code 304 based on If-Modified-Since Header
  (#1078)
- feat(node): add remaining Node.js builtin aliases (#1085)
- feat(node): add shim for perf_hooks (#1088)
- feat(node): assert/strict alias (#1084)
- feat(node): fs/promises implementation (#1083)
- feat(testing): add `assertRejects`, deprecate `assertThrowsAsync` (#1101)
- fix(async): make it so exception of `deadline` can be caught (#1105)
- fix(http/file_server): fix flaky 'file_server sets Date header correctly' test
  case (#1095)
- fix(node): assert/strict, fs/promises, perf_hooks modules could not be
  required (#1107)
- fix(node/events): optimize listener management (#1113)
- fix(testing): change `assertThrows` and `assertThrowsAsync` return type to
  `void` and `Promise<void>` (#1052)

### 0.103.0 / 2021.07.26

- feat(async): add status to deferred promises (#1047)
- feat(http): add range request and etag support to `file_server.ts` (#1028)
- fix(async/deferred): rename .status -> .state (#1055)
- fix(encoding/base64url): throw TypeError in case of invalid base64url string
  (#1040)
- fix(encoding/toml): fix inline table and nested array (#1042)
- fix(encoding/yaml): fix `parseAll` type definition by using overloads (#1048)
- fix(testing): `assertThrowsAsync` always reporting `Error` instead of actual
  error class (#1051)
- fix(testing/asserts): cater for different class constructor functions (#1000)

### 0.102.0 / 2021.07.19

- feat: Add std/collections (#993)
- fix(encoding/toml): fix comment line starting with whitespaces (#1017)
- fix(encoding/toml): parse keys correctly (#1019)
- fix(hash): fix handling of non-byte-sized TypedArray views (#1012)
- fix(testing): Don't merge diff when it's not spaces even if it's surrounded by
  word-diff (#1032)

### 0.101.0 / 2021.07.13

- BREAKING(encoding/hex): remove encodedLen, encodeToString, decodedLen,
  decodeString, errInvalidByte, errLength (#733)
- BREAKING(mime/multipart): return array for multiple values with same form name
  (#722)
- BREAKING(std/uuid): rework v4 and v5 module (#971)
- feat(async): add `deadline` to async module (#1022)
- feat(async): add debounce method to async module (#1006)
- feat(encoding/toml): fix bad string format. Improve coverage (#991)
- feat(hash): add BLAKE3 hash support (#994)
- feat(http): Add Cookie domain validation (#1009)
- feat(http): Allow passing path and domain attributes while removing cookies
  (#1005)
- feat(io): add `copy` function (#1016)
- feat(io/streams): add autoClose option to writableStreamFromWriter (#964)
- feat(std/node): add writeBuffer of internal binding fs module (#888)
- fix: improve type safety for browser-compatible modules (#995)
- fix(encoding/toml): serializes mixed array (#1001)
- fix(encoding/toml): throws parse error when toml uses invalid whitespaces
  (#1013)
- fix(http): `setCookie` with `maxAge` of `0` (#992)
- fix(http/server): Swallow NotConnected errors from listener.accept() (#761)
- fix(io/bufio): fix handling of trailing new line (#990)
- fix(node/module): More descriptive error in "createRequire" (#997)
- fix(path): Add question mark as a glob indicator (#1024)
- fix(testing): use return type of never for `fail` (#1002)

### 0.100.0 / 2021.06.29

- feat(testing/asserts): improved strings diff (#948)
- feat(testing/asserts): use assertion signature for "assertExists" (#969)
- fix(node/events): align EventEmitter#addListener with native node tests (#976)
- fix(path): fix type error in glob.ts with noImplicitAny: false config (#977)

### 0.99.0 / 2021.06.15

- feat(mime): make createPart of MultipartWriter public (#960)
- feat(node/util): add inherits (#958)
- fix(node/events): fix EventEmitter#removeAllListeners (#968)
- fix(node/process): make process.env enumerable (#957)
- fix(node/util): fix util.inherits (#959)

### 0.98.0 / 2021.06.08

- feat(async): add async/tee (#919)
- feat(async/mux): take AsyncIterable as source iterator (#923)
- feat(io/bufio): add encoding options to `readLines` and `readStringDelim`
  (#921)
- feat(node/perf_hooks): add perf_hooks module (#945)
- fix(encoding/binary): allow getNBytes to read until EOF (#932)
- fix(encoding/binary): respect non 0 byte offsets (#826)
- fix(node/events): fix EventEmitter#once to pass native node tests (#935)
- fix(node/events): fix getMaxListeners and setMaxListeners to pass native node
  tests (#928)
- fix(node/fs): fix type error in fs.watch impl (#947)
- fix(testing/asserts): fix handling of Weak* objects (#951)

### 0.97.0 / 2021.05.17

- fix(io/buffer): make Buffer compatible with Deploy (#912)
- fix(io/bufio): readDelim returns wrong result if delim strides over chunks
  (#877)
- fix(node/events): accept only functions as listener arguments (#916)
- fix(testing): support array values in assertObjectMatch (#906)

### 0.96.0 / 2021.05.11

- feat(fs/walk): show path in walk error (#875)
- feat(http): allow custom response code (#855)
- feat(io): add readRange, readRangeSync (#884)
- feat(mime/multipart): add options to readForm (#895)
- feat(node): add console module (#892)
- feat(node/assert): add rejects and doesNotReject (#894)
- feat(std/node): add implementation of os.homedir() (#873)
- fix(http/file_server): keep url and name consistent (#908)
- fix(io): Improve readDelims() performance (#867)
- fix(io/streams): don't use a byte ReadableStream (#891)
- fix(node/assert): enable test-assert-fail.js and align assert.fail to it
  (#874)
- fix(node/child_process): Try to fix flaky tests (#876)
- fix(node/stream): make `Stream` the default export (#901)

### 0.95.0 / 2021.04.23

- feat(node): add basic support for child_process.spawn (#785)
- feat(path/glob): add caseInsensitive option (#854)
- fix(node/fs): actually export everything (#862)

### 0.94.0 / 2021.04.20

- feat(node/fs): add fstat and fstatSync (#847)
- feat(streams): add readableStreamFromReader (#852)
- fix(path): reduce circular dependency (#858)
- fix(testing): equals does not differentiate undefined/absent keys (#849)

### 0.93.0 / 2021.04.13

- feat: add iter and iterSync to io/util (#843)
- feat(node/fs): add fdatasync and fdatasyncSync (#841)
- feat(node/fs): add fsync and fsyncSync (#840)
- feat(node/fs): add ftruncate and ftruncateSync (#829)
- feat(node/fs): add futimes and futimesSync (#830)
- fix(testing): Function signature of assertObjectEquals() does not accept
  interfaces (#763)

### 0.92.0 / 2021.04.02

- feat: make bufio compatible to Deno Deploy (#831)
- feat: add symlink adn symlinkSync to node/fs (#825)
- feat: add format and improve deprecate in node/util (#693)
- feat: add io/buffer and io/util module (#808) …
- fix: handle upstream type changes (#834)
- refactor: `Promise<void>` return types are unnecessary boilerplate in
  encoding. (#818)
- chore: remove unused import in http (#817)

### 0.91.0 / 2021.03.21

- chore(codecov): ignore coverage of examples (#798)
- feat(encoding/yaml): add support for JS types and user types (#789)
- feat(io/streams): Add readerFromIterable() (#752)
- feat(std/node): add utimes and utimesSync (#805)
- fix(multipart): support useDefineForClassFields (#807)
- fix(node): fix node/cli.ts (#797)
- fix(node): move `throw error` in fs.writeFile to pass `no-unsafe-finally`
  (#810)
- fix(path): enable and fix file URL tests (#804)
- refactor(node/fs): update fs import (#793)

### 0.90.0 / 2021.03.09

- fix(http): Create a single encoder instance (#790)
- feat(node): Add "module" polyfill (#783)
- feat(node): Add CLI for running Node.js script with std/node (#779)
- feat(node): Fix assert module, enable test cases (#769)

### 0.89.0 / 2021.03.02

- BREAKING(io/streams): Strengthen iterator to readable stream conversion (#735)
- build: collect and upload code coverage (#770)
- feat(node): add constants module (#747)
- feat(node): add crypto.createHash (#757)
- feat(node): add process.hrtime function (#751)
- feat(node): add truncate and truncateSync (#765)
- fix(node): export promisify & callbackify (#748)
- fix(node): fix export items of events (#758)
- fix(node): ignore shebang (#746)
- fix(node): native module needs to be extensible (#745)
- fix(node/process): make process.argv an array (#749)
- fix: fix type errors in canary test (#762)
- refactor: fix codes to pass `no-unused-vars` lint (#764)
- test(path): update test cases for canary (#775)

### 0.88.0 / 2021.02.19

- BREAKING(encoding): remove module utf8.ts (#728)
- chore: fix typo in contributing section (#709)
- docs(bytes): improve README.md (#737)
- feat(node): add native module polyfills: url, crypto (#729)
- feat(node): add tty module (#738)
- feat(node): support conditional exports (#726)
- fix(std/testing) : Handle Symbols correctly in deep equalities (#731)
- test(node): run external tests with --quiet (#732)

### 0.87.0 / 2021.02.12

- BREAKING(http/cookie): remove Cookies and SameSite type aliases (#720)
- docs(fmt): fix examples in fmt/colors.ts (#715)
- docs(io/ioutil): improve jsdoc (#706)
- fix(http/file_server): svg media type (#718)
- refactor(hash/md5): throw `TypeError` for wrong type (#698)
- test(node): enable native node tests (#695)

### 0.86.0 / 2021.02.05

- feat(http/file_server): support do not show dotfiles (#690)
- feat(http/file_server): show ../ if it makes sense & end dirs with / (#691)

Releases notes for previous releases can be found in
[`deno` repository](https://github.com/denoland/deno/releases).
