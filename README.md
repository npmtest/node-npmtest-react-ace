# npmtest-react-ace

#### test coverage for  [react-ace (v4.2.1)](https://github.com/securingsincity/react-ace#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-react-ace.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-react-ace) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-react-ace.svg)](https://travis-ci.org/npmtest/node-npmtest-react-ace)

#### A react component for Ace Editor

[![NPM](https://nodei.co/npm/react-ace.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-ace)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-react-ace/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-ace/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-react-ace/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-react-ace/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-react-ace/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-react-ace/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-react-ace/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-react-ace/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-react-ace/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-ace/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-react-ace/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-react-ace/build/test-report.html](https://npmtest.github.io/node-npmtest-react-ace/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-react-ace/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-react-ace/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-react-ace/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-ace/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-ace/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-ace/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-react-ace/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-react-ace/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "James Hrisho"
    },
    "babel": {
        "presets": [
            "es2015",
            "react"
        ],
        "plugins": [
            "transform-object-rest-spread"
        ]
    },
    "bugs": {
        "url": "https://github.com/securingsincity/react-ace/issues"
    },
    "dependencies": {
        "brace": "^0.9.1",
        "lodash.isequal": "^4.1.1",
        "prop-types": "^15.5.8"
    },
    "description": "A react component for Ace Editor",
    "devDependencies": {
        "babel-cli": "^6.6.5",
        "babel-core": "^6.7.5",
        "babel-loader": "^6.2.4",
        "babel-plugin-transform-object-rest-spread": "^6.8.0",
        "babel-preset-es2015": "^6.6.0",
        "babel-preset-react": "^6.5.0",
        "chai": "^3.5.0",
        "enzyme": "^2.4.1",
        "eslint": "^1.10.3",
        "eslint-config-airbnb": "^2.1.1",
        "eslint-plugin-react": "^3.13.1",
        "jest": "^0.1.37",
        "jsdom": "^9.6.0",
        "mocha": "^3.1.2",
        "nyc": "^8.3.1",
        "react-addons-test-utils": "^15.3.2",
        "react-test-renderer": "^15.5.4",
        "rimraf": "^2.5.2",
        "sinon": "^1.17.6",
        "webpack": "^1.12.14"
    },
    "directories": {},
    "dist": {
        "shasum": "dbc91e19d1ef9ae6333eb153675249761926699b",
        "tarball": "https://registry.npmjs.org/react-ace/-/react-ace-4.2.1.tgz"
    },
    "gitHead": "e4b3aa65799a7f31a27174236b8d9a7d50d414d6",
    "homepage": "https://github.com/securingsincity/react-ace#readme",
    "keywords": [
        "ace",
        "ace editor",
        "react-component",
        "react",
        "brace"
    ],
    "license": "MIT",
    "main": "lib/ace.js",
    "maintainers": [
        {
            "name": "securingsincity"
        }
    ],
    "name": "react-ace",
    "nyc": {
        "exclude": [
            "**/*.spec.js",
            "node_modules"
        ],
        "extension": [
            ".js",
            ".jsx"
        ],
        "reporter": [
            "lcov",
            "text",
            "html"
        ]
    },
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "^0.13.0 || ^0.14.0 || ^15.0.1",
        "react-dom": "^0.13.0 || ^0.14.0 || ^15.0.1"
    },
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/securingsincity/react-ace.git"
    },
    "scripts": {
        "build": "npm run build:lib && npm run build:umd && npm run build:umd:min",
        "build:example": "cd example && npm install",
        "build:lib": "babel src --out-dir lib",
        "build:umd": "webpack src/ace.jsx dist/react-ace.js --config webpack.config.development.js",
        "build:umd:min": "webpack src/ace.jsx dist/react-ace.min.js --config webpack.config.production.js",
        "check": "npm run lint",
        "clean": "rimraf lib dist",
        "coverage": "nyc npm run test",
        "lint": "eslint src/ace.jsx",
        "postversion": "git push && git push --tags && npm run clean",
        "prepublish": "npm run clean && npm run build",
        "preversion": "npm run clean && npm run check",
        "test": "mocha --compilers js:babel-core/register --require tests/setup.js --recursive tests/**/*.spec.js",
        "version": "npm run build"
    },
    "types": "types.d.ts",
    "version": "4.2.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
