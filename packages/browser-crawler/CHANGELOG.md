# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## 3.10.6 (2024-07-10)


### Bug Fixes

* `enqueueLinks` should respect full URL of the current request for relative link resolution ([#1427](https://github.com/apify/crawlee/issues/1427)) ([e72d02c](https://github.com/apify/crawlee/commit/e72d02c1e7c4d871914956d3e5c025b1a82ce12c))
* `retryOnBlocked` doesn't override the blocked HTTP codes ([#2243](https://github.com/apify/crawlee/issues/2243)) ([81672c3](https://github.com/apify/crawlee/commit/81672c3d1db1dcdcffb868de5740addff82cf112))
* add `headless` option to `BrowserCrawlerOptions` ([#1412](https://github.com/apify/crawlee/issues/1412)) ([7896839](https://github.com/apify/crawlee/commit/7896839dee7a26a002458a3643e1c847dfb50e78))
* calling enqueueLinks in browser crawler on page without any links ([385ca27](https://github.com/apify/crawlee/commit/385ca27c4c50096f2e28bf0da369d6aaf849a73b))
* cookie monster is no more ([#1414](https://github.com/apify/crawlee/issues/1414)) ([a361147](https://github.com/apify/crawlee/commit/a361147dd711b74221c631c0ced9daaefc19d0f0))
* declare missing dependency on `tslib` ([27e96c8](https://github.com/apify/crawlee/commit/27e96c80c26e7fc31809a4b518d699573cb8c662)), closes [#1747](https://github.com/apify/crawlee/issues/1747)
* declare missing peer dependencies in `@crawlee/browser` package ([#2532](https://github.com/apify/crawlee/issues/2532)) ([3357c7f](https://github.com/apify/crawlee/commit/3357c7fc5ab071b12f72097c190dbee9990e3751))
* enqueue link not finding relative links if the checked page is redirected ([#1416](https://github.com/apify/crawlee/issues/1416)) ([b78b37b](https://github.com/apify/crawlee/commit/b78b37b98ed961c03bb619d379e58f3641dd1fb0))
* ignore invalid URLs in `enqueueLinks` in browser crawlers ([#1803](https://github.com/apify/crawlee/issues/1803)) ([5ac336c](https://github.com/apify/crawlee/commit/5ac336c5b83b212fd6281659b8ceee091e259ff1))
* injectJQuery in context does not survive navs ([#1661](https://github.com/apify/crawlee/issues/1661)) ([493a7cf](https://github.com/apify/crawlee/commit/493a7cff569cb12cfd9aa5e0f4fcb9de686eb41f))
* log original error message on session rotation ([#2022](https://github.com/apify/crawlee/issues/2022)) ([8a11ffb](https://github.com/apify/crawlee/commit/8a11ffbdaef6b2fe8603aac570c3038f84c2f203))
* mark `context.request.loadedUrl` and `id` as required inside the request handler ([#2531](https://github.com/apify/crawlee/issues/2531)) ([2b54660](https://github.com/apify/crawlee/commit/2b546600691d84852a2f9ef42f273cecf818d66d))
* pin all internal dependencies ([#2041](https://github.com/apify/crawlee/issues/2041)) ([d6f2b17](https://github.com/apify/crawlee/commit/d6f2b172d4a6776137c7893ca798d5b4a9408e79)), closes [#2040](https://github.com/apify/crawlee/issues/2040)
* remove undeclared dependency on core package from puppeteer utils ([827ae60](https://github.com/apify/crawlee/commit/827ae60d6c77e8c7271408493c3750a67ef8a9b4))
* requestHandlerTimeout timing ([#1660](https://github.com/apify/crawlee/issues/1660)) ([493ea0c](https://github.com/apify/crawlee/commit/493ea0ce80e55ece5a8881a6aea6674918873b35))
* respect `<base>` when enqueuing ([#1936](https://github.com/apify/crawlee/issues/1936)) ([aeef572](https://github.com/apify/crawlee/commit/aeef57231c84671374ed0309b7b95fa9ce9a6e8b))
* respect `headless` option in browser crawlers ([#1455](https://github.com/apify/crawlee/issues/1455)) ([46f6e4c](https://github.com/apify/crawlee/commit/46f6e4cb542feae4a360b72e6d637fcc53876712))
* support TypeScript 4.8 ([#1507](https://github.com/apify/crawlee/issues/1507)) ([4c3a504](https://github.com/apify/crawlee/commit/4c3a5045931a7f270bf8eda8a6417466b32fc99b))


### Features

* `browserPerProxy` browser launch option ([#2418](https://github.com/apify/crawlee/issues/2418)) ([df57b29](https://github.com/apify/crawlee/commit/df57b2965ac8c8b3adf807e3bad8a649814fa213))
* `tieredProxyUrls` for ProxyConfiguration ([#2348](https://github.com/apify/crawlee/issues/2348)) ([5408c7f](https://github.com/apify/crawlee/commit/5408c7f60a5bf4dbdba92f2d7440e0946b94ea6e))
* adaptive playwright crawler ([#2316](https://github.com/apify/crawlee/issues/2316)) ([8e4218a](https://github.com/apify/crawlee/commit/8e4218ada03cf485751def46f8c465b2d2a825c7))
* add `iframe` expansion to `parseWithCheerio` in browsers ([#2542](https://github.com/apify/crawlee/issues/2542)) ([328d085](https://github.com/apify/crawlee/commit/328d08598807782b3712bd543e394fe9a000a85d)), closes [#2507](https://github.com/apify/crawlee/issues/2507)
* add `ignoreIframes` opt-out from the Cheerio iframe expansion ([#2562](https://github.com/apify/crawlee/issues/2562)) ([474a8dc](https://github.com/apify/crawlee/commit/474a8dc06a567cde0651d385fdac9c350ddf4508))
* better `newUrlFunction` for ProxyConfiguration ([#2392](https://github.com/apify/crawlee/issues/2392)) ([330598b](https://github.com/apify/crawlee/commit/330598b348ad27bc7c73732294a14b655ccd3507)), closes [#2348](https://github.com/apify/crawlee/issues/2348) [#2065](https://github.com/apify/crawlee/issues/2065)
* check enqueue link strategy post redirect ([#2238](https://github.com/apify/crawlee/issues/2238)) ([3c5f9d6](https://github.com/apify/crawlee/commit/3c5f9d6056158e042e12d75b2b1b21ef6c32e618)), closes [#2173](https://github.com/apify/crawlee/issues/2173)
* don't close page before calling errorHandler ([#1548](https://github.com/apify/crawlee/issues/1548)) ([1c8cd82](https://github.com/apify/crawlee/commit/1c8cd82611e93e4991b49b8ba2f1842457875680))
* enable tab-as-a-container for Firefox ([#1456](https://github.com/apify/crawlee/issues/1456)) ([ae5ba4f](https://github.com/apify/crawlee/commit/ae5ba4f15fd6d14f444486234753ce1781c74cc8))
* error tracker ([#1467](https://github.com/apify/crawlee/issues/1467)) ([6bfe1ce](https://github.com/apify/crawlee/commit/6bfe1ce0161f1e26f97e2b8e5c02ec9ca608fe30))
* expand #shadow-root elements automatically in `parseWithCheerio` helper ([#2396](https://github.com/apify/crawlee/issues/2396)) ([a05b3a9](https://github.com/apify/crawlee/commit/a05b3a93a9b57926b353df0e79d846b5024c42ac))
* initial crawlee commit ([#1384](https://github.com/apify/crawlee/issues/1384)) ([3a59bfc](https://github.com/apify/crawlee/commit/3a59bfc0b7199b2742478dd0f8bee80d3a62f3d3))
* log cause with `retryOnBlocked` ([#2252](https://github.com/apify/crawlee/issues/2252)) ([e19a773](https://github.com/apify/crawlee/commit/e19a773693cfc5e65c1e2321bfc8b73c9844ea8b)), closes [#2249](https://github.com/apify/crawlee/issues/2249)
* **puppeteer:** enable `new` headless mode ([#1910](https://github.com/apify/crawlee/issues/1910)) ([7fc999c](https://github.com/apify/crawlee/commit/7fc999cf4658ca69b97f16d434444081998470f4))
* Request Queue v2 ([#1975](https://github.com/apify/crawlee/issues/1975)) ([70a77ee](https://github.com/apify/crawlee/commit/70a77ee15f984e9ae67cd584fc58ace7e55346db)), closes [#1365](https://github.com/apify/crawlee/issues/1365)
* retire session on proxy error ([#2002](https://github.com/apify/crawlee/issues/2002)) ([8c0928b](https://github.com/apify/crawlee/commit/8c0928b24ceabefc454f8114ac30a27023709010)), closes [#1912](https://github.com/apify/crawlee/issues/1912)
* retryOnBlocked detects blocked webpage ([#1956](https://github.com/apify/crawlee/issues/1956)) ([766fa9b](https://github.com/apify/crawlee/commit/766fa9b88029e9243a7427075384c1abe85c70c8))
* tab as a container + proxy per page ([#1417](https://github.com/apify/crawlee/issues/1417)) ([71a755d](https://github.com/apify/crawlee/commit/71a755de4ef0b9f9db2efd94bd41b186b7fc05b8))


### Reverts

* Revert "chore(release): v3.1.0" ([762d345](https://github.com/apify/crawlee/commit/762d345b48f3c308e574541e5737fe7423d55238))





## [3.10.5](https://github.com/apify/crawlee/compare/v3.10.4...v3.10.5) (2024-06-12)


### Bug Fixes

* declare missing peer dependencies in `@crawlee/browser` package ([#2532](https://github.com/apify/crawlee/issues/2532)) ([3357c7f](https://github.com/apify/crawlee/commit/3357c7fc5ab071b12f72097c190dbee9990e3751))
* mark `context.request.loadedUrl` and `id` as required inside the request handler ([#2531](https://github.com/apify/crawlee/issues/2531)) ([2b54660](https://github.com/apify/crawlee/commit/2b546600691d84852a2f9ef42f273cecf818d66d))





## [3.10.4](https://github.com/apify/crawlee/compare/v3.10.3...v3.10.4) (2024-06-11)

**Note:** Version bump only for package @crawlee/browser





## [3.10.3](https://github.com/apify/crawlee/compare/v3.10.2...v3.10.3) (2024-06-07)

**Note:** Version bump only for package @crawlee/browser





## [3.10.2](https://github.com/apify/crawlee/compare/v3.10.1...v3.10.2) (2024-06-03)

**Note:** Version bump only for package @crawlee/browser





## [3.10.1](https://github.com/apify/crawlee/compare/v3.10.0...v3.10.1) (2024-05-23)

**Note:** Version bump only for package @crawlee/browser





# [3.10.0](https://github.com/apify/crawlee/compare/v3.9.2...v3.10.0) (2024-05-16)

**Note:** Version bump only for package @crawlee/browser





## [3.9.2](https://github.com/apify/crawlee/compare/v3.9.1...v3.9.2) (2024-04-17)

**Note:** Version bump only for package @crawlee/browser





## [3.9.1](https://github.com/apify/crawlee/compare/v3.9.0...v3.9.1) (2024-04-11)


### Features

* `browserPerProxy` browser launch option ([#2418](https://github.com/apify/crawlee/issues/2418)) ([df57b29](https://github.com/apify/crawlee/commit/df57b2965ac8c8b3adf807e3bad8a649814fa213))





# [3.9.0](https://github.com/apify/crawlee/compare/v3.8.2...v3.9.0) (2024-04-10)


### Features

* `tieredProxyUrls` for ProxyConfiguration ([#2348](https://github.com/apify/crawlee/issues/2348)) ([5408c7f](https://github.com/apify/crawlee/commit/5408c7f60a5bf4dbdba92f2d7440e0946b94ea6e))
* better `newUrlFunction` for ProxyConfiguration ([#2392](https://github.com/apify/crawlee/issues/2392)) ([330598b](https://github.com/apify/crawlee/commit/330598b348ad27bc7c73732294a14b655ccd3507)), closes [#2348](https://github.com/apify/crawlee/issues/2348) [#2065](https://github.com/apify/crawlee/issues/2065)
* expand #shadow-root elements automatically in `parseWithCheerio` helper ([#2396](https://github.com/apify/crawlee/issues/2396)) ([a05b3a9](https://github.com/apify/crawlee/commit/a05b3a93a9b57926b353df0e79d846b5024c42ac))





## [3.8.2](https://github.com/apify/crawlee/compare/v3.8.1...v3.8.2) (2024-03-21)

**Note:** Version bump only for package @crawlee/browser





## [3.8.1](https://github.com/apify/crawlee/compare/v3.8.0...v3.8.1) (2024-02-22)

**Note:** Version bump only for package @crawlee/browser





# [3.8.0](https://github.com/apify/crawlee/compare/v3.7.3...v3.8.0) (2024-02-21)


### Features

* adaptive playwright crawler ([#2316](https://github.com/apify/crawlee/issues/2316)) ([8e4218a](https://github.com/apify/crawlee/commit/8e4218ada03cf485751def46f8c465b2d2a825c7))





## [3.7.3](https://github.com/apify/crawlee/compare/v3.7.2...v3.7.3) (2024-01-30)

**Note:** Version bump only for package @crawlee/browser





## [3.7.2](https://github.com/apify/crawlee/compare/v3.7.1...v3.7.2) (2024-01-09)

**Note:** Version bump only for package @crawlee/browser





## [3.7.1](https://github.com/apify/crawlee/compare/v3.7.0...v3.7.1) (2024-01-02)

**Note:** Version bump only for package @crawlee/browser





# [3.7.0](https://github.com/apify/crawlee/compare/v3.6.2...v3.7.0) (2023-12-21)


### Bug Fixes

* `retryOnBlocked` doesn't override the blocked HTTP codes ([#2243](https://github.com/apify/crawlee/issues/2243)) ([81672c3](https://github.com/apify/crawlee/commit/81672c3d1db1dcdcffb868de5740addff82cf112))


### Features

* check enqueue link strategy post redirect ([#2238](https://github.com/apify/crawlee/issues/2238)) ([3c5f9d6](https://github.com/apify/crawlee/commit/3c5f9d6056158e042e12d75b2b1b21ef6c32e618)), closes [#2173](https://github.com/apify/crawlee/issues/2173)
* log cause with `retryOnBlocked` ([#2252](https://github.com/apify/crawlee/issues/2252)) ([e19a773](https://github.com/apify/crawlee/commit/e19a773693cfc5e65c1e2321bfc8b73c9844ea8b)), closes [#2249](https://github.com/apify/crawlee/issues/2249)





## [3.6.2](https://github.com/apify/crawlee/compare/v3.6.1...v3.6.2) (2023-11-26)

**Note:** Version bump only for package @crawlee/browser





## [3.6.1](https://github.com/apify/crawlee/compare/v3.6.0...v3.6.1) (2023-11-15)


### Features

* **puppeteer:** enable `new` headless mode ([#1910](https://github.com/apify/crawlee/issues/1910)) ([7fc999c](https://github.com/apify/crawlee/commit/7fc999cf4658ca69b97f16d434444081998470f4))





# [3.6.0](https://github.com/apify/crawlee/compare/v3.5.8...v3.6.0) (2023-11-15)

**Note:** Version bump only for package @crawlee/browser





## [3.5.8](https://github.com/apify/crawlee/compare/v3.5.7...v3.5.8) (2023-10-17)

**Note:** Version bump only for package @crawlee/browser





## [3.5.7](https://github.com/apify/crawlee/compare/v3.5.6...v3.5.7) (2023-10-05)

**Note:** Version bump only for package @crawlee/browser





## [3.5.6](https://github.com/apify/crawlee/compare/v3.5.5...v3.5.6) (2023-10-04)

**Note:** Version bump only for package @crawlee/browser





## [3.5.5](https://github.com/apify/crawlee/compare/v3.5.4...v3.5.5) (2023-10-02)


### Features

* Request Queue v2 ([#1975](https://github.com/apify/crawlee/issues/1975)) ([70a77ee](https://github.com/apify/crawlee/commit/70a77ee15f984e9ae67cd584fc58ace7e55346db)), closes [#1365](https://github.com/apify/crawlee/issues/1365)





## [3.5.4](https://github.com/apify/crawlee/compare/v3.5.3...v3.5.4) (2023-09-11)

**Note:** Version bump only for package @crawlee/browser





## [3.5.3](https://github.com/apify/crawlee/compare/v3.5.2...v3.5.3) (2023-08-31)


### Bug Fixes

* pin all internal dependencies ([#2041](https://github.com/apify/crawlee/issues/2041)) ([d6f2b17](https://github.com/apify/crawlee/commit/d6f2b172d4a6776137c7893ca798d5b4a9408e79)), closes [#2040](https://github.com/apify/crawlee/issues/2040)





## [3.5.2](https://github.com/apify/crawlee/compare/v3.5.1...v3.5.2) (2023-08-21)

**Note:** Version bump only for package @crawlee/browser





## [3.5.1](https://github.com/apify/crawlee/compare/v3.5.0...v3.5.1) (2023-08-16)


### Bug Fixes

* log original error message on session rotation ([#2022](https://github.com/apify/crawlee/issues/2022)) ([8a11ffb](https://github.com/apify/crawlee/commit/8a11ffbdaef6b2fe8603aac570c3038f84c2f203))





# [3.5.0](https://github.com/apify/crawlee/compare/v3.4.2...v3.5.0) (2023-07-31)


### Features

* retire session on proxy error ([#2002](https://github.com/apify/crawlee/issues/2002)) ([8c0928b](https://github.com/apify/crawlee/commit/8c0928b24ceabefc454f8114ac30a27023709010)), closes [#1912](https://github.com/apify/crawlee/issues/1912)





## [3.4.2](https://github.com/apify/crawlee/compare/v3.4.1...v3.4.2) (2023-07-19)


### Features

* retryOnBlocked detects blocked webpage ([#1956](https://github.com/apify/crawlee/issues/1956)) ([766fa9b](https://github.com/apify/crawlee/commit/766fa9b88029e9243a7427075384c1abe85c70c8))





## [3.4.1](https://github.com/apify/crawlee/compare/v3.4.0...v3.4.1) (2023-07-13)

**Note:** Version bump only for package @crawlee/browser





# [3.4.0](https://github.com/apify/crawlee/compare/v3.3.3...v3.4.0) (2023-06-12)


### Bug Fixes

* respect `<base>` when enqueuing ([#1936](https://github.com/apify/crawlee/issues/1936)) ([aeef572](https://github.com/apify/crawlee/commit/aeef57231c84671374ed0309b7b95fa9ce9a6e8b))





## [3.3.3](https://github.com/apify/crawlee/compare/v3.3.2...v3.3.3) (2023-05-31)

**Note:** Version bump only for package @crawlee/browser





## [3.3.2](https://github.com/apify/crawlee/compare/v3.3.1...v3.3.2) (2023-05-11)

**Note:** Version bump only for package @crawlee/browser





## [3.3.1](https://github.com/apify/crawlee/compare/v3.3.0...v3.3.1) (2023-04-11)

**Note:** Version bump only for package @crawlee/browser





# [3.3.0](https://github.com/apify/crawlee/compare/v3.2.2...v3.3.0) (2023-03-09)


### Bug Fixes

* ignore invalid URLs in `enqueueLinks` in browser crawlers ([#1803](https://github.com/apify/crawlee/issues/1803)) ([5ac336c](https://github.com/apify/crawlee/commit/5ac336c5b83b212fd6281659b8ceee091e259ff1))





## [3.2.2](https://github.com/apify/crawlee/compare/v3.2.1...v3.2.2) (2023-02-08)

**Note:** Version bump only for package @crawlee/browser





## [3.2.1](https://github.com/apify/crawlee/compare/v3.2.0...v3.2.1) (2023-02-07)

**Note:** Version bump only for package @crawlee/browser





# [3.2.0](https://github.com/apify/crawlee/compare/v3.1.4...v3.2.0) (2023-02-07)


### Bug Fixes

* declare missing dependency on `tslib` ([27e96c8](https://github.com/apify/crawlee/commit/27e96c80c26e7fc31809a4b518d699573cb8c662)), closes [#1747](https://github.com/apify/crawlee/issues/1747)





## [3.1.4](https://github.com/apify/crawlee/compare/v3.1.3...v3.1.4) (2022-12-14)

**Note:** Version bump only for package @crawlee/browser





## [3.1.3](https://github.com/apify/crawlee/compare/v3.1.2...v3.1.3) (2022-12-07)

**Note:** Version bump only for package @crawlee/browser





## 3.1.2 (2022-11-15)

**Note:** Version bump only for package @crawlee/browser





## 3.1.1 (2022-11-07)

**Note:** Version bump only for package @crawlee/browser





# 3.1.0 (2022-10-13)

**Note:** Version bump only for package @crawlee/browser





## [3.0.4](https://github.com/apify/crawlee/compare/v3.0.3...v3.0.4) (2022-08-22)


### Features

* enable tab-as-a-container for Firefox ([#1456](https://github.com/apify/crawlee/issues/1456)) ([ae5ba4f](https://github.com/apify/crawlee/commit/ae5ba4f15fd6d14f444486234753ce1781c74cc8))
