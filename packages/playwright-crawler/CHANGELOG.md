# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## 3.10.6 (2024-07-10)


### Bug Fixes

* `utils.playwright.blockRequests` warning message ([#1632](https://github.com/apify/crawlee/issues/1632)) ([76549eb](https://github.com/apify/crawlee/commit/76549eb250a39e961b7f567ad0610af136d1c79f))
* **adaptive-crawler:** log only once for the committed request handler execution ([#2524](https://github.com/apify/crawlee/issues/2524)) ([533bd3f](https://github.com/apify/crawlee/commit/533bd3f04671d54273f0861664d316269d08fbfb))
* add `skipNavigation` option to `enqueueLinks` ([#2153](https://github.com/apify/crawlee/issues/2153)) ([118515d](https://github.com/apify/crawlee/commit/118515d2ba534b99be2f23436f6abe41d66a8e07))
* allow `userData` option in `enqueueLinksByClickingElements` ([#1749](https://github.com/apify/crawlee/issues/1749)) ([736f85d](https://github.com/apify/crawlee/commit/736f85d4a3b99a06d0f99f91e33e71976a9458a3)), closes [#1617](https://github.com/apify/crawlee/issues/1617)
* allow creating new adaptive crawler instance without any parameters ([9b7f595](https://github.com/apify/crawlee/commit/9b7f595a2d70cab5c50e188581b21b0ef7e51780))
* allow to use any version of puppeteer or playwright ([#2102](https://github.com/apify/crawlee/issues/2102)) ([0cafceb](https://github.com/apify/crawlee/commit/0cafceb2966d430dd1b2a1b619fe66da1c951f4c)), closes [#2101](https://github.com/apify/crawlee/issues/2101)
* cookie monster is no more ([#1414](https://github.com/apify/crawlee/issues/1414)) ([a361147](https://github.com/apify/crawlee/commit/a361147dd711b74221c631c0ced9daaefc19d0f0))
* declare missing dependency on `tslib` ([27e96c8](https://github.com/apify/crawlee/commit/27e96c80c26e7fc31809a4b518d699573cb8c662)), closes [#1747](https://github.com/apify/crawlee/issues/1747)
* do not drop statistics on migration/resurrection/resume ([#2462](https://github.com/apify/crawlee/issues/2462)) ([8ce7dd4](https://github.com/apify/crawlee/commit/8ce7dd4ae6a3718dac95e784a53bd5661c827edc))
* fix detection of HTTP site when using the `useState` in adaptive crawler ([#2530](https://github.com/apify/crawlee/issues/2530)) ([7e195c1](https://github.com/apify/crawlee/commit/7e195c17cf1d9beae7f6f068fe505f1334a3a5b3))
* infiniteScroll() not working in Firefox ([#1826](https://github.com/apify/crawlee/issues/1826)) ([4286c5d](https://github.com/apify/crawlee/commit/4286c5d29b94aec3f4d3835bbf36b7fafcaec8f0)), closes [#1821](https://github.com/apify/crawlee/issues/1821)
* injectJQuery in context does not survive navs ([#1661](https://github.com/apify/crawlee/issues/1661)) ([493a7cf](https://github.com/apify/crawlee/commit/493a7cff569cb12cfd9aa5e0f4fcb9de686eb41f))
* **jsdom:** delay closing of the window and add some polyfills ([2e81618](https://github.com/apify/crawlee/commit/2e81618afb5f3890495e3e5fcfa037eb3319edc9))
* mark `context.request.loadedUrl` and `id` as required inside the request handler ([#2531](https://github.com/apify/crawlee/issues/2531)) ([2b54660](https://github.com/apify/crawlee/commit/2b546600691d84852a2f9ef42f273cecf818d66d))
* pin all internal dependencies ([#2041](https://github.com/apify/crawlee/issues/2041)) ([d6f2b17](https://github.com/apify/crawlee/commit/d6f2b172d4a6776137c7893ca798d5b4a9408e79)), closes [#2040](https://github.com/apify/crawlee/issues/2040)
* **playwright:** allow passing new context options in `launchOptions` on type level ([0519d40](https://github.com/apify/crawlee/commit/0519d4099d257bbc40ed091c131a674ea5f8d731)), closes [#1849](https://github.com/apify/crawlee/issues/1849)
* remove undeclared dependency on core package from puppeteer utils ([827ae60](https://github.com/apify/crawlee/commit/827ae60d6c77e8c7271408493c3750a67ef8a9b4))
* respect `headless` option in browser crawlers ([#1455](https://github.com/apify/crawlee/issues/1455)) ([46f6e4c](https://github.com/apify/crawlee/commit/46f6e4cb542feae4a360b72e6d637fcc53876712))
* respect implicit router when no `requestHandler` is provided in `AdaptiveCrawler` ([#2518](https://github.com/apify/crawlee/issues/2518)) ([31083aa](https://github.com/apify/crawlee/commit/31083aa27ddd51827f73c7ac4290379ec7a81283))
* shallow clone browserPoolOptions before normalization ([#1665](https://github.com/apify/crawlee/issues/1665)) ([22467ca](https://github.com/apify/crawlee/commit/22467ca81ad9464d528495333f62a60f2ea0487c))
* update playwright to 1.29.2 and make peer dep. less strict ([#1735](https://github.com/apify/crawlee/issues/1735)) ([c654fcd](https://github.com/apify/crawlee/commit/c654fcdea06fb203b7952ed97650190cc0e74394)), closes [#1723](https://github.com/apify/crawlee/issues/1723)
* various helpers opening KVS now respect Configuration ([#2071](https://github.com/apify/crawlee/issues/2071)) ([59dbb16](https://github.com/apify/crawlee/commit/59dbb164699774e5a6718e98d0a4e8f630f35323))


### Features

* `createAdaptivePlaywrightRouter` utility ([#2415](https://github.com/apify/crawlee/issues/2415)) ([cee4778](https://github.com/apify/crawlee/commit/cee477814e4901d025c5376205ad884c2fe08e0e)), closes [#2407](https://github.com/apify/crawlee/issues/2407)
* adaptive playwright crawler ([#2316](https://github.com/apify/crawlee/issues/2316)) ([8e4218a](https://github.com/apify/crawlee/commit/8e4218ada03cf485751def46f8c465b2d2a825c7))
* add `closeCookieModals` context helper for Playwright and Puppeteer ([#1927](https://github.com/apify/crawlee/issues/1927)) ([98d93bb](https://github.com/apify/crawlee/commit/98d93bb6713ec219baa83db2ad2cd1d7621a3339))
* add `forefront` option to all `enqueueLinks` variants ([#1760](https://github.com/apify/crawlee/issues/1760)) ([a01459d](https://github.com/apify/crawlee/commit/a01459dffb51162e676354f0aa4811a1d36affa9)), closes [#1483](https://github.com/apify/crawlee/issues/1483)
* add `iframe` expansion to `parseWithCheerio` in browsers ([#2542](https://github.com/apify/crawlee/issues/2542)) ([328d085](https://github.com/apify/crawlee/commit/328d08598807782b3712bd543e394fe9a000a85d)), closes [#2507](https://github.com/apify/crawlee/issues/2507)
* add `ignoreIframes` opt-out from the Cheerio iframe expansion ([#2562](https://github.com/apify/crawlee/issues/2562)) ([474a8dc](https://github.com/apify/crawlee/commit/474a8dc06a567cde0651d385fdac9c350ddf4508))
* add `parseWithCheerio` for puppeteer & playwright ([#1418](https://github.com/apify/crawlee/issues/1418)) ([02b0aeb](https://github.com/apify/crawlee/commit/02b0aeb52e09c5c0ccfdd34b6330481d62f627a6))
* add `utils.playwright.blockRequests()` ([#1447](https://github.com/apify/crawlee/issues/1447)) ([1c6a8e4](https://github.com/apify/crawlee/commit/1c6a8e412f4f519db3216f92ad093c906a23ccda))
* add `utils.playwright.compileScript` ([#1559](https://github.com/apify/crawlee/issues/1559)) ([2e14162](https://github.com/apify/crawlee/commit/2e141625f27aa58e2195ab37ed2e31691b58f4c0))
* add `utils.playwright.infiniteScroll` ([#1543](https://github.com/apify/crawlee/issues/1543)) ([60c8289](https://github.com/apify/crawlee/commit/60c8289571f3b6bce908ef7d1636b59faebdbf87)), closes [#1528](https://github.com/apify/crawlee/issues/1528)
* add `utils.playwright.saveSnapshot` ([#1544](https://github.com/apify/crawlee/issues/1544)) ([a4ceef0](https://github.com/apify/crawlee/commit/a4ceef044f0c5afdfd964dd1163a260463a60f52))
* add `waitForSelector` context helper + `parseWithCheerio` in adaptive crawler ([#2522](https://github.com/apify/crawlee/issues/2522)) ([6f88e73](https://github.com/apify/crawlee/commit/6f88e738d43ab4774dc4ef3f78775a5d88728e0d))
* **core:** use `RequestQueue.addBatchedRequests()` in `enqueueLinks` helper ([4d61ca9](https://github.com/apify/crawlee/commit/4d61ca934072f8bbb680c842d8b1c9a4452ee73a)), closes [#1995](https://github.com/apify/crawlee/issues/1995)
* enable tab-as-a-container for Firefox ([#1456](https://github.com/apify/crawlee/issues/1456)) ([ae5ba4f](https://github.com/apify/crawlee/commit/ae5ba4f15fd6d14f444486234753ce1781c74cc8))
* enqueue links by clicking for Playwright ([#1545](https://github.com/apify/crawlee/issues/1545)) ([3d25ade](https://github.com/apify/crawlee/commit/3d25adefa7570433a9fa636941684bc2701b8ddd))
* expand #shadow-root elements automatically in `parseWithCheerio` helper ([#2396](https://github.com/apify/crawlee/issues/2396)) ([a05b3a9](https://github.com/apify/crawlee/commit/a05b3a93a9b57926b353df0e79d846b5024c42ac))
* implement global storage access checking and use it to prevent unwanted side effects in adaptive crawler ([#2371](https://github.com/apify/crawlee/issues/2371)) ([fb3b7da](https://github.com/apify/crawlee/commit/fb3b7da402522ddff8c7394ac1253ba8aeac984c)), closes [#2364](https://github.com/apify/crawlee/issues/2364)
* infiniteScroll has maxScrollHeight limit ([#1945](https://github.com/apify/crawlee/issues/1945)) ([44997bb](https://github.com/apify/crawlee/commit/44997bba5bbf33ddb7dbac2f3e26d4bee60d4f47))
* initial crawlee commit ([#1384](https://github.com/apify/crawlee/issues/1384)) ([3a59bfc](https://github.com/apify/crawlee/commit/3a59bfc0b7199b2742478dd0f8bee80d3a62f3d3))
* **playwright:** disable animations when taking screenshots ([#1601](https://github.com/apify/crawlee/issues/1601)) ([4e63034](https://github.com/apify/crawlee/commit/4e63034c7b87de405edbd84f9b1803aa101f5c78))
* **puppeteer:** enable `new` headless mode ([#1910](https://github.com/apify/crawlee/issues/1910)) ([7fc999c](https://github.com/apify/crawlee/commit/7fc999cf4658ca69b97f16d434444081998470f4))
* Request Queue v2 ([#1975](https://github.com/apify/crawlee/issues/1975)) ([70a77ee](https://github.com/apify/crawlee/commit/70a77ee15f984e9ae67cd584fc58ace7e55346db)), closes [#1365](https://github.com/apify/crawlee/issues/1365)
* **router:** allow inline router definition ([#1877](https://github.com/apify/crawlee/issues/1877)) ([2d241c9](https://github.com/apify/crawlee/commit/2d241c9f88964ebd41a181069c378b6b7b5bf262))
* tab as a container + proxy per page ([#1417](https://github.com/apify/crawlee/issues/1417)) ([71a755d](https://github.com/apify/crawlee/commit/71a755de4ef0b9f9db2efd94bd41b186b7fc05b8))


### Reverts

* Revert "chore(release): v3.1.0" ([762d345](https://github.com/apify/crawlee/commit/762d345b48f3c308e574541e5737fe7423d55238))





## [3.10.5](https://github.com/apify/crawlee/compare/v3.10.4...v3.10.5) (2024-06-12)


### Bug Fixes

* allow creating new adaptive crawler instance without any parameters ([9b7f595](https://github.com/apify/crawlee/commit/9b7f595a2d70cab5c50e188581b21b0ef7e51780))
* fix detection of HTTP site when using the `useState` in adaptive crawler ([#2530](https://github.com/apify/crawlee/issues/2530)) ([7e195c1](https://github.com/apify/crawlee/commit/7e195c17cf1d9beae7f6f068fe505f1334a3a5b3))
* mark `context.request.loadedUrl` and `id` as required inside the request handler ([#2531](https://github.com/apify/crawlee/issues/2531)) ([2b54660](https://github.com/apify/crawlee/commit/2b546600691d84852a2f9ef42f273cecf818d66d))





## [3.10.4](https://github.com/apify/crawlee/compare/v3.10.3...v3.10.4) (2024-06-11)


### Bug Fixes

* **playwright:** allow passing new context options in `launchOptions` on type level ([0519d40](https://github.com/apify/crawlee/commit/0519d4099d257bbc40ed091c131a674ea5f8d731)), closes [#1849](https://github.com/apify/crawlee/issues/1849)





## [3.10.3](https://github.com/apify/crawlee/compare/v3.10.2...v3.10.3) (2024-06-07)


### Bug Fixes

* **adaptive-crawler:** log only once for the committed request handler execution ([#2524](https://github.com/apify/crawlee/issues/2524)) ([533bd3f](https://github.com/apify/crawlee/commit/533bd3f04671d54273f0861664d316269d08fbfb))
* respect implicit router when no `requestHandler` is provided in `AdaptiveCrawler` ([#2518](https://github.com/apify/crawlee/issues/2518)) ([31083aa](https://github.com/apify/crawlee/commit/31083aa27ddd51827f73c7ac4290379ec7a81283))


### Features

* add `waitForSelector` context helper + `parseWithCheerio` in adaptive crawler ([#2522](https://github.com/apify/crawlee/issues/2522)) ([6f88e73](https://github.com/apify/crawlee/commit/6f88e738d43ab4774dc4ef3f78775a5d88728e0d))





## [3.10.2](https://github.com/apify/crawlee/compare/v3.10.1...v3.10.2) (2024-06-03)

**Note:** Version bump only for package @crawlee/playwright





## [3.10.1](https://github.com/apify/crawlee/compare/v3.10.0...v3.10.1) (2024-05-23)

**Note:** Version bump only for package @crawlee/playwright





# [3.10.0](https://github.com/apify/crawlee/compare/v3.9.2...v3.10.0) (2024-05-16)


### Bug Fixes

* do not drop statistics on migration/resurrection/resume ([#2462](https://github.com/apify/crawlee/issues/2462)) ([8ce7dd4](https://github.com/apify/crawlee/commit/8ce7dd4ae6a3718dac95e784a53bd5661c827edc))





## [3.9.2](https://github.com/apify/crawlee/compare/v3.9.1...v3.9.2) (2024-04-17)

**Note:** Version bump only for package @crawlee/playwright





## [3.9.1](https://github.com/apify/crawlee/compare/v3.9.0...v3.9.1) (2024-04-11)

**Note:** Version bump only for package @crawlee/playwright





# [3.9.0](https://github.com/apify/crawlee/compare/v3.8.2...v3.9.0) (2024-04-10)


### Features

* `createAdaptivePlaywrightRouter` utility ([#2415](https://github.com/apify/crawlee/issues/2415)) ([cee4778](https://github.com/apify/crawlee/commit/cee477814e4901d025c5376205ad884c2fe08e0e)), closes [#2407](https://github.com/apify/crawlee/issues/2407)
* expand #shadow-root elements automatically in `parseWithCheerio` helper ([#2396](https://github.com/apify/crawlee/issues/2396)) ([a05b3a9](https://github.com/apify/crawlee/commit/a05b3a93a9b57926b353df0e79d846b5024c42ac))





## [3.8.2](https://github.com/apify/crawlee/compare/v3.8.1...v3.8.2) (2024-03-21)


### Features

* implement global storage access checking and use it to prevent unwanted side effects in adaptive crawler ([#2371](https://github.com/apify/crawlee/issues/2371)) ([fb3b7da](https://github.com/apify/crawlee/commit/fb3b7da402522ddff8c7394ac1253ba8aeac984c)), closes [#2364](https://github.com/apify/crawlee/issues/2364)





## [3.8.1](https://github.com/apify/crawlee/compare/v3.8.0...v3.8.1) (2024-02-22)

**Note:** Version bump only for package @crawlee/playwright





# [3.8.0](https://github.com/apify/crawlee/compare/v3.7.3...v3.8.0) (2024-02-21)


### Features

* adaptive playwright crawler ([#2316](https://github.com/apify/crawlee/issues/2316)) ([8e4218a](https://github.com/apify/crawlee/commit/8e4218ada03cf485751def46f8c465b2d2a825c7))





## [3.7.3](https://github.com/apify/crawlee/compare/v3.7.2...v3.7.3) (2024-01-30)

**Note:** Version bump only for package @crawlee/playwright





## [3.7.2](https://github.com/apify/crawlee/compare/v3.7.1...v3.7.2) (2024-01-09)

**Note:** Version bump only for package @crawlee/playwright





## [3.7.1](https://github.com/apify/crawlee/compare/v3.7.0...v3.7.1) (2024-01-02)

**Note:** Version bump only for package @crawlee/playwright





# [3.7.0](https://github.com/apify/crawlee/compare/v3.6.2...v3.7.0) (2023-12-21)

**Note:** Version bump only for package @crawlee/playwright





## [3.6.2](https://github.com/apify/crawlee/compare/v3.6.1...v3.6.2) (2023-11-26)

**Note:** Version bump only for package @crawlee/playwright





## [3.6.1](https://github.com/apify/crawlee/compare/v3.6.0...v3.6.1) (2023-11-15)


### Features

* **puppeteer:** enable `new` headless mode ([#1910](https://github.com/apify/crawlee/issues/1910)) ([7fc999c](https://github.com/apify/crawlee/commit/7fc999cf4658ca69b97f16d434444081998470f4))





# [3.6.0](https://github.com/apify/crawlee/compare/v3.5.8...v3.6.0) (2023-11-15)


### Bug Fixes

* add `skipNavigation` option to `enqueueLinks` ([#2153](https://github.com/apify/crawlee/issues/2153)) ([118515d](https://github.com/apify/crawlee/commit/118515d2ba534b99be2f23436f6abe41d66a8e07))





## [3.5.8](https://github.com/apify/crawlee/compare/v3.5.7...v3.5.8) (2023-10-17)

**Note:** Version bump only for package @crawlee/playwright





## [3.5.7](https://github.com/apify/crawlee/compare/v3.5.6...v3.5.7) (2023-10-05)

**Note:** Version bump only for package @crawlee/playwright





## [3.5.6](https://github.com/apify/crawlee/compare/v3.5.5...v3.5.6) (2023-10-04)

**Note:** Version bump only for package @crawlee/playwright





## [3.5.5](https://github.com/apify/crawlee/compare/v3.5.4...v3.5.5) (2023-10-02)


### Bug Fixes

* allow to use any version of puppeteer or playwright ([#2102](https://github.com/apify/crawlee/issues/2102)) ([0cafceb](https://github.com/apify/crawlee/commit/0cafceb2966d430dd1b2a1b619fe66da1c951f4c)), closes [#2101](https://github.com/apify/crawlee/issues/2101)


### Features

* Request Queue v2 ([#1975](https://github.com/apify/crawlee/issues/1975)) ([70a77ee](https://github.com/apify/crawlee/commit/70a77ee15f984e9ae67cd584fc58ace7e55346db)), closes [#1365](https://github.com/apify/crawlee/issues/1365)





## [3.5.4](https://github.com/apify/crawlee/compare/v3.5.3...v3.5.4) (2023-09-11)


### Bug Fixes

* various helpers opening KVS now respect Configuration ([#2071](https://github.com/apify/crawlee/issues/2071)) ([59dbb16](https://github.com/apify/crawlee/commit/59dbb164699774e5a6718e98d0a4e8f630f35323))





## [3.5.3](https://github.com/apify/crawlee/compare/v3.5.2...v3.5.3) (2023-08-31)


### Bug Fixes

* pin all internal dependencies ([#2041](https://github.com/apify/crawlee/issues/2041)) ([d6f2b17](https://github.com/apify/crawlee/commit/d6f2b172d4a6776137c7893ca798d5b4a9408e79)), closes [#2040](https://github.com/apify/crawlee/issues/2040)





## [3.5.2](https://github.com/apify/crawlee/compare/v3.5.1...v3.5.2) (2023-08-21)

**Note:** Version bump only for package @crawlee/playwright





## [3.5.1](https://github.com/apify/crawlee/compare/v3.5.0...v3.5.1) (2023-08-16)

**Note:** Version bump only for package @crawlee/playwright





# [3.5.0](https://github.com/apify/crawlee/compare/v3.4.2...v3.5.0) (2023-07-31)


### Features

* add `closeCookieModals` context helper for Playwright and Puppeteer ([#1927](https://github.com/apify/crawlee/issues/1927)) ([98d93bb](https://github.com/apify/crawlee/commit/98d93bb6713ec219baa83db2ad2cd1d7621a3339))
* **core:** use `RequestQueue.addBatchedRequests()` in `enqueueLinks` helper ([4d61ca9](https://github.com/apify/crawlee/commit/4d61ca934072f8bbb680c842d8b1c9a4452ee73a)), closes [#1995](https://github.com/apify/crawlee/issues/1995)





## [3.4.2](https://github.com/apify/crawlee/compare/v3.4.1...v3.4.2) (2023-07-19)

**Note:** Version bump only for package @crawlee/playwright





## [3.4.1](https://github.com/apify/crawlee/compare/v3.4.0...v3.4.1) (2023-07-13)

**Note:** Version bump only for package @crawlee/playwright





# [3.4.0](https://github.com/apify/crawlee/compare/v3.3.3...v3.4.0) (2023-06-12)


### Features

* infiniteScroll has maxScrollHeight limit ([#1945](https://github.com/apify/crawlee/issues/1945)) ([44997bb](https://github.com/apify/crawlee/commit/44997bba5bbf33ddb7dbac2f3e26d4bee60d4f47))





## [3.3.3](https://github.com/apify/crawlee/compare/v3.3.2...v3.3.3) (2023-05-31)

**Note:** Version bump only for package @crawlee/playwright





## [3.3.2](https://github.com/apify/crawlee/compare/v3.3.1...v3.3.2) (2023-05-11)


### Features

* **router:** allow inline router definition ([#1877](https://github.com/apify/crawlee/issues/1877)) ([2d241c9](https://github.com/apify/crawlee/commit/2d241c9f88964ebd41a181069c378b6b7b5bf262))





## [3.3.1](https://github.com/apify/crawlee/compare/v3.3.0...v3.3.1) (2023-04-11)


### Bug Fixes

* infiniteScroll() not working in Firefox ([#1826](https://github.com/apify/crawlee/issues/1826)) ([4286c5d](https://github.com/apify/crawlee/commit/4286c5d29b94aec3f4d3835bbf36b7fafcaec8f0)), closes [#1821](https://github.com/apify/crawlee/issues/1821)
* **jsdom:** delay closing of the window and add some polyfills ([2e81618](https://github.com/apify/crawlee/commit/2e81618afb5f3890495e3e5fcfa037eb3319edc9))





# [3.3.0](https://github.com/apify/crawlee/compare/v3.2.2...v3.3.0) (2023-03-09)

**Note:** Version bump only for package @crawlee/playwright





## [3.2.2](https://github.com/apify/crawlee/compare/v3.2.1...v3.2.2) (2023-02-08)

**Note:** Version bump only for package @crawlee/playwright





## [3.2.1](https://github.com/apify/crawlee/compare/v3.2.0...v3.2.1) (2023-02-07)

**Note:** Version bump only for package @crawlee/playwright





# [3.2.0](https://github.com/apify/crawlee/compare/v3.1.4...v3.2.0) (2023-02-07)


### Bug Fixes

* allow `userData` option in `enqueueLinksByClickingElements` ([#1749](https://github.com/apify/crawlee/issues/1749)) ([736f85d](https://github.com/apify/crawlee/commit/736f85d4a3b99a06d0f99f91e33e71976a9458a3)), closes [#1617](https://github.com/apify/crawlee/issues/1617)
* declare missing dependency on `tslib` ([27e96c8](https://github.com/apify/crawlee/commit/27e96c80c26e7fc31809a4b518d699573cb8c662)), closes [#1747](https://github.com/apify/crawlee/issues/1747)
* update playwright to 1.29.2 and make peer dep. less strict ([#1735](https://github.com/apify/crawlee/issues/1735)) ([c654fcd](https://github.com/apify/crawlee/commit/c654fcdea06fb203b7952ed97650190cc0e74394)), closes [#1723](https://github.com/apify/crawlee/issues/1723)


### Features

* add `forefront` option to all `enqueueLinks` variants ([#1760](https://github.com/apify/crawlee/issues/1760)) ([a01459d](https://github.com/apify/crawlee/commit/a01459dffb51162e676354f0aa4811a1d36affa9)), closes [#1483](https://github.com/apify/crawlee/issues/1483)





## [3.1.4](https://github.com/apify/crawlee/compare/v3.1.3...v3.1.4) (2022-12-14)

**Note:** Version bump only for package @crawlee/playwright





## [3.1.3](https://github.com/apify/crawlee/compare/v3.1.2...v3.1.3) (2022-12-07)

**Note:** Version bump only for package @crawlee/playwright





## 3.1.2 (2022-11-15)

**Note:** Version bump only for package @crawlee/playwright





## 3.1.1 (2022-11-07)

**Note:** Version bump only for package @crawlee/playwright





# 3.1.0 (2022-10-13)

**Note:** Version bump only for package @crawlee/playwright





## [3.0.4](https://github.com/apify/crawlee/compare/v3.0.3...v3.0.4) (2022-08-22)


### Features

* enable tab-as-a-container for Firefox ([#1456](https://github.com/apify/crawlee/issues/1456)) ([ae5ba4f](https://github.com/apify/crawlee/commit/ae5ba4f15fd6d14f444486234753ce1781c74cc8))
