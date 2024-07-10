# Change Log

All notable changes to this project will be documented in this file.
See [Conventional Commits](https://conventionalcommits.org) for commit guidelines.

## 3.10.6 (2024-07-10)


### Bug Fixes

* add `UserData` type argument to `CheerioCrawlingContext` and related interfaces ([#1424](https://github.com/apify/crawlee/issues/1424)) ([a062cb7](https://github.com/apify/crawlee/commit/a062cb752e3ef6294762da75a2de2ea0bb122445))
* add missing configuration to CheerioCrawler constructor ([#1432](https://github.com/apify/crawlee/issues/1432)) ([6e4ab1c](https://github.com/apify/crawlee/commit/6e4ab1c132edf0b98407be7c667463f20e47eb89))
* **CheerioCrawler:** pass ixXml down to response parser ([#1807](https://github.com/apify/crawlee/issues/1807)) ([af7a5c4](https://github.com/apify/crawlee/commit/af7a5c4efa94a53e5bdfeca340a9d7223d7dfda4)), closes [#1794](https://github.com/apify/crawlee/issues/1794)
* cookie monster is no more ([#1414](https://github.com/apify/crawlee/issues/1414)) ([a361147](https://github.com/apify/crawlee/commit/a361147dd711b74221c631c0ced9daaefc19d0f0))
* declare dependency on `ow` in cheerio package ([be59f99](https://github.com/apify/crawlee/commit/be59f992d2897ce5c02349bbcc62472d99bb2718))
* declare missing dependency on `tslib` ([27e96c8](https://github.com/apify/crawlee/commit/27e96c80c26e7fc31809a4b518d699573cb8c662)), closes [#1747](https://github.com/apify/crawlee/issues/1747)
* enqueue link not finding relative links if the checked page is redirected ([#1416](https://github.com/apify/crawlee/issues/1416)) ([b78b37b](https://github.com/apify/crawlee/commit/b78b37b98ed961c03bb619d379e58f3641dd1fb0))
* ensure default route is not ignored in `CheerioCrawler` ([#1411](https://github.com/apify/crawlee/issues/1411)) ([6475628](https://github.com/apify/crawlee/commit/6475628eb0fa895868ea75486ecc39cfee66cd92))
* fix building projects with TS when puppeteer and playwright are not installed ([#1404](https://github.com/apify/crawlee/issues/1404)) ([3e1218b](https://github.com/apify/crawlee/commit/3e1218b6e39b1cb94577ce438b4e88081969adc1))
* ignore invalid URLs in `enqueueLinks` in browser crawlers ([#1803](https://github.com/apify/crawlee/issues/1803)) ([5ac336c](https://github.com/apify/crawlee/commit/5ac336c5b83b212fd6281659b8ceee091e259ff1))
* make `CheerioCrawlerOptions` type more loose ([d871d8c](https://github.com/apify/crawlee/commit/d871d8caf22bc8d8ca1041e4975f3c95eae4b487))
* pin all internal dependencies ([#2041](https://github.com/apify/crawlee/issues/2041)) ([d6f2b17](https://github.com/apify/crawlee/commit/d6f2b172d4a6776137c7893ca798d5b4a9408e79)), closes [#2040](https://github.com/apify/crawlee/issues/2040)
* remove `JSONData` generic type arg from `CheerioCrawler` ([#1402](https://github.com/apify/crawlee/issues/1402)) ([f8d486e](https://github.com/apify/crawlee/commit/f8d486ed7492123f6f77306ef0a7e41d3544f0a0))
* rename interface `FailedRequestHandler` to `ErrorHandler` ([#1410](https://github.com/apify/crawlee/issues/1410)) ([c5b74c6](https://github.com/apify/crawlee/commit/c5b74c6a741fc789e8a0b486aed17067783b0826))
* respect `<base>` when enqueuing ([#1936](https://github.com/apify/crawlee/issues/1936)) ([aeef572](https://github.com/apify/crawlee/commit/aeef57231c84671374ed0309b7b95fa9ce9a6e8b))
* use `desiredConcurrency: 10` as the default for `CheerioCrawler` ([#1428](https://github.com/apify/crawlee/issues/1428)) ([0aca5b5](https://github.com/apify/crawlee/commit/0aca5b55057a0c5150c3c7e11946008c0dcc542d))
* using explicitly typed router with `CheerioCrawler` ([07b7e69](https://github.com/apify/crawlee/commit/07b7e69e1a7b7c89b8a5538279eb6de8be0effde))


### Features

* add `parseWithCheerio` context helper to cheerio crawler ([b336a73](https://github.com/apify/crawlee/commit/b336a739117a6e4180492ec9915ddce128376a2c))
* add `waitForSelector` context helper + `parseWithCheerio` in adaptive crawler ([#2522](https://github.com/apify/crawlee/issues/2522)) ([6f88e73](https://github.com/apify/crawlee/commit/6f88e738d43ab4774dc4ef3f78775a5d88728e0d))
* http-crawler ([#1440](https://github.com/apify/crawlee/issues/1440)) ([8c303f7](https://github.com/apify/crawlee/commit/8c303f7fd718b217cea3108409b6092711d1183b))
* initial crawlee commit ([#1384](https://github.com/apify/crawlee/issues/1384)) ([3a59bfc](https://github.com/apify/crawlee/commit/3a59bfc0b7199b2742478dd0f8bee80d3a62f3d3))
* **jsdom:** add `parseWithCheerio` context helper ([c8f0796](https://github.com/apify/crawlee/commit/c8f0796aebc0dfa6e6d04740a0bb7d8ddd5b2d96))
* Request Queue v2 ([#1975](https://github.com/apify/crawlee/issues/1975)) ([70a77ee](https://github.com/apify/crawlee/commit/70a77ee15f984e9ae67cd584fc58ace7e55346db)), closes [#1365](https://github.com/apify/crawlee/issues/1365)
* **router:** allow inline router definition ([#1877](https://github.com/apify/crawlee/issues/1877)) ([2d241c9](https://github.com/apify/crawlee/commit/2d241c9f88964ebd41a181069c378b6b7b5bf262))


### Reverts

* Revert "chore(release): v3.1.0" ([762d345](https://github.com/apify/crawlee/commit/762d345b48f3c308e574541e5737fe7423d55238))





## [3.10.5](https://github.com/apify/crawlee/compare/v3.10.4...v3.10.5) (2024-06-12)

**Note:** Version bump only for package @crawlee/cheerio





## [3.10.4](https://github.com/apify/crawlee/compare/v3.10.3...v3.10.4) (2024-06-11)

**Note:** Version bump only for package @crawlee/cheerio





## [3.10.3](https://github.com/apify/crawlee/compare/v3.10.2...v3.10.3) (2024-06-07)


### Features

* add `waitForSelector` context helper + `parseWithCheerio` in adaptive crawler ([#2522](https://github.com/apify/crawlee/issues/2522)) ([6f88e73](https://github.com/apify/crawlee/commit/6f88e738d43ab4774dc4ef3f78775a5d88728e0d))





## [3.10.2](https://github.com/apify/crawlee/compare/v3.10.1...v3.10.2) (2024-06-03)

**Note:** Version bump only for package @crawlee/cheerio





## [3.10.1](https://github.com/apify/crawlee/compare/v3.10.0...v3.10.1) (2024-05-23)

**Note:** Version bump only for package @crawlee/cheerio





# [3.10.0](https://github.com/apify/crawlee/compare/v3.9.2...v3.10.0) (2024-05-16)

**Note:** Version bump only for package @crawlee/cheerio





## [3.9.2](https://github.com/apify/crawlee/compare/v3.9.1...v3.9.2) (2024-04-17)

**Note:** Version bump only for package @crawlee/cheerio





## [3.9.1](https://github.com/apify/crawlee/compare/v3.9.0...v3.9.1) (2024-04-11)

**Note:** Version bump only for package @crawlee/cheerio





# [3.9.0](https://github.com/apify/crawlee/compare/v3.8.2...v3.9.0) (2024-04-10)

**Note:** Version bump only for package @crawlee/cheerio





## [3.8.2](https://github.com/apify/crawlee/compare/v3.8.1...v3.8.2) (2024-03-21)

**Note:** Version bump only for package @crawlee/cheerio





## [3.8.1](https://github.com/apify/crawlee/compare/v3.8.0...v3.8.1) (2024-02-22)

**Note:** Version bump only for package @crawlee/cheerio





# [3.8.0](https://github.com/apify/crawlee/compare/v3.7.3...v3.8.0) (2024-02-21)

**Note:** Version bump only for package @crawlee/cheerio





## [3.7.3](https://github.com/apify/crawlee/compare/v3.7.2...v3.7.3) (2024-01-30)

**Note:** Version bump only for package @crawlee/cheerio





## [3.7.2](https://github.com/apify/crawlee/compare/v3.7.1...v3.7.2) (2024-01-09)

**Note:** Version bump only for package @crawlee/cheerio





## [3.7.1](https://github.com/apify/crawlee/compare/v3.7.0...v3.7.1) (2024-01-02)

**Note:** Version bump only for package @crawlee/cheerio





# [3.7.0](https://github.com/apify/crawlee/compare/v3.6.2...v3.7.0) (2023-12-21)

**Note:** Version bump only for package @crawlee/cheerio





## [3.6.2](https://github.com/apify/crawlee/compare/v3.6.1...v3.6.2) (2023-11-26)

**Note:** Version bump only for package @crawlee/cheerio





## [3.6.1](https://github.com/apify/crawlee/compare/v3.6.0...v3.6.1) (2023-11-15)

**Note:** Version bump only for package @crawlee/cheerio





# [3.6.0](https://github.com/apify/crawlee/compare/v3.5.8...v3.6.0) (2023-11-15)

**Note:** Version bump only for package @crawlee/cheerio





## [3.5.8](https://github.com/apify/crawlee/compare/v3.5.7...v3.5.8) (2023-10-17)

**Note:** Version bump only for package @crawlee/cheerio





## [3.5.7](https://github.com/apify/crawlee/compare/v3.5.6...v3.5.7) (2023-10-05)

**Note:** Version bump only for package @crawlee/cheerio





## [3.5.6](https://github.com/apify/crawlee/compare/v3.5.5...v3.5.6) (2023-10-04)

**Note:** Version bump only for package @crawlee/cheerio





## [3.5.5](https://github.com/apify/crawlee/compare/v3.5.4...v3.5.5) (2023-10-02)


### Features

* Request Queue v2 ([#1975](https://github.com/apify/crawlee/issues/1975)) ([70a77ee](https://github.com/apify/crawlee/commit/70a77ee15f984e9ae67cd584fc58ace7e55346db)), closes [#1365](https://github.com/apify/crawlee/issues/1365)





## [3.5.4](https://github.com/apify/crawlee/compare/v3.5.3...v3.5.4) (2023-09-11)

**Note:** Version bump only for package @crawlee/cheerio





## [3.5.3](https://github.com/apify/crawlee/compare/v3.5.2...v3.5.3) (2023-08-31)


### Bug Fixes

* pin all internal dependencies ([#2041](https://github.com/apify/crawlee/issues/2041)) ([d6f2b17](https://github.com/apify/crawlee/commit/d6f2b172d4a6776137c7893ca798d5b4a9408e79)), closes [#2040](https://github.com/apify/crawlee/issues/2040)





## [3.5.2](https://github.com/apify/crawlee/compare/v3.5.1...v3.5.2) (2023-08-21)

**Note:** Version bump only for package @crawlee/cheerio





## [3.5.1](https://github.com/apify/crawlee/compare/v3.5.0...v3.5.1) (2023-08-16)

**Note:** Version bump only for package @crawlee/cheerio





# [3.5.0](https://github.com/apify/crawlee/compare/v3.4.2...v3.5.0) (2023-07-31)

**Note:** Version bump only for package @crawlee/cheerio





## [3.4.2](https://github.com/apify/crawlee/compare/v3.4.1...v3.4.2) (2023-07-19)

**Note:** Version bump only for package @crawlee/cheerio





## [3.4.1](https://github.com/apify/crawlee/compare/v3.4.0...v3.4.1) (2023-07-13)

**Note:** Version bump only for package @crawlee/cheerio





# [3.4.0](https://github.com/apify/crawlee/compare/v3.3.3...v3.4.0) (2023-06-12)


### Bug Fixes

* respect `<base>` when enqueuing ([#1936](https://github.com/apify/crawlee/issues/1936)) ([aeef572](https://github.com/apify/crawlee/commit/aeef57231c84671374ed0309b7b95fa9ce9a6e8b))





## [3.3.3](https://github.com/apify/crawlee/compare/v3.3.2...v3.3.3) (2023-05-31)

**Note:** Version bump only for package @crawlee/cheerio





## [3.3.2](https://github.com/apify/crawlee/compare/v3.3.1...v3.3.2) (2023-05-11)


### Features

* **router:** allow inline router definition ([#1877](https://github.com/apify/crawlee/issues/1877)) ([2d241c9](https://github.com/apify/crawlee/commit/2d241c9f88964ebd41a181069c378b6b7b5bf262))





## [3.3.1](https://github.com/apify/crawlee/compare/v3.3.0...v3.3.1) (2023-04-11)


### Features

* add `parseWithCheerio` context helper to cheerio crawler ([b336a73](https://github.com/apify/crawlee/commit/b336a739117a6e4180492ec9915ddce128376a2c))
* **jsdom:** add `parseWithCheerio` context helper ([c8f0796](https://github.com/apify/crawlee/commit/c8f0796aebc0dfa6e6d04740a0bb7d8ddd5b2d96))





# [3.3.0](https://github.com/apify/crawlee/compare/v3.2.2...v3.3.0) (2023-03-09)


### Bug Fixes

* **CheerioCrawler:** pass ixXml down to response parser ([#1807](https://github.com/apify/crawlee/issues/1807)) ([af7a5c4](https://github.com/apify/crawlee/commit/af7a5c4efa94a53e5bdfeca340a9d7223d7dfda4)), closes [#1794](https://github.com/apify/crawlee/issues/1794)
* ignore invalid URLs in `enqueueLinks` in browser crawlers ([#1803](https://github.com/apify/crawlee/issues/1803)) ([5ac336c](https://github.com/apify/crawlee/commit/5ac336c5b83b212fd6281659b8ceee091e259ff1))





## [3.2.2](https://github.com/apify/crawlee/compare/v3.2.1...v3.2.2) (2023-02-08)

**Note:** Version bump only for package @crawlee/cheerio





## [3.2.1](https://github.com/apify/crawlee/compare/v3.2.0...v3.2.1) (2023-02-07)

**Note:** Version bump only for package @crawlee/cheerio





# [3.2.0](https://github.com/apify/crawlee/compare/v3.1.4...v3.2.0) (2023-02-07)


### Bug Fixes

* declare missing dependency on `tslib` ([27e96c8](https://github.com/apify/crawlee/commit/27e96c80c26e7fc31809a4b518d699573cb8c662)), closes [#1747](https://github.com/apify/crawlee/issues/1747)





## [3.1.4](https://github.com/apify/crawlee/compare/v3.1.3...v3.1.4) (2022-12-14)

**Note:** Version bump only for package @crawlee/cheerio





## [3.1.3](https://github.com/apify/crawlee/compare/v3.1.2...v3.1.3) (2022-12-07)

**Note:** Version bump only for package @crawlee/cheerio





## 3.1.2 (2022-11-15)

**Note:** Version bump only for package @crawlee/cheerio





## 3.1.1 (2022-11-07)

**Note:** Version bump only for package @crawlee/cheerio





# 3.1.0 (2022-10-13)

**Note:** Version bump only for package @crawlee/cheerio





## [3.0.4](https://github.com/apify/crawlee/compare/v3.0.3...v3.0.4) (2022-08-22)

**Note:** Version bump only for package @crawlee/cheerio
