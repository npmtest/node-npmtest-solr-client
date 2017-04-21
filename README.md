# npmtest-solr-client

#### basic test coverage for  solr-client (v0.6.0)  [![npm package](https://img.shields.io/npm/v/npmtest-solr-client.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-solr-client) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-solr-client.svg)](https://travis-ci.org/npmtest/node-npmtest-solr-client)

####  A Solr client library for indexing, adding, deleting, committing, optimizing and searching documents within an Apache Solr installation (version>=3.2)

[![NPM](https://nodei.co/npm/solr-client.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/solr-client)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-solr-client/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-solr-client/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-solr-client/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-solr-client/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-solr-client/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-solr-client/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-solr-client/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-solr-client/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-solr-client/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-solr-client/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-solr-client/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-solr-client/build/test-report.html](https://npmtest.github.io/node-npmtest-solr-client/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-solr-client/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-solr-client/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-solr-client/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-solr-client/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-solr-client/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-solr-client/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-solr-client/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-solr-client/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Remy Loubradou",
        "url": "https://twitter.com/#!/lbdremy"
    },
    "name": "solr-client",
    "main": "./main",
    "description": " A Solr client library for indexing, adding, deleting, committing, optimizing and searching documents within an Apache Solr installation (version>=3.2)",
    "version": "0.6.0",
    "repository": {
        "type": "git",
        "url": "https://github.com/lbdremy/solr-node-client"
    },
    "engines": {
        "node": ">= 0.4.7"
    },
    "dependencies": {
        "JSONStream": "~1.0.6",
        "duplexer": "~0.1.1",
        "httperror": "~0.2.3",
        "json-bigint": "~0.1.4",
        "request": "~2.63.0"
    },
    "devDependencies": {
        "chai": "~3.3.0",
        "bignumber.js": "~2.0.7",
        "minimist": "~1.2.0",
        "csv-stream": "~0.1.3",
        "mocha": "~2.3.3",
        "figc": "~0.0.3"
    },
    "scripts": {
        "test": "./node_modules/mocha/bin/mocha -R spec test/*-test.js && ./node_modules/mocha/bin/mocha -R spec test/*-test.js --client.bigint=true",
        "test-cov": "jscoverage lib lib-cov && ./node_modules/mocha/bin/mocha -R html-cov test/*-test.js > coverage.html && rm -r lib-cov",
        "report": "rm -rf report && mkdir report && plato -r -d report main.js lib/*"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
