# npmtest-electron-forge

#### basic test coverage for  [electron-forge (v2.10.0)](https://github.com/electron-userland/electron-forge#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-electron-forge.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-electron-forge) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-electron-forge.svg)](https://travis-ci.org/npmtest/node-npmtest-electron-forge)

#### A complete tool for building modern Electron applications

[![NPM](https://nodei.co/npm/electron-forge.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/electron-forge)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-electron-forge/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-electron-forge/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-electron-forge/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-electron-forge/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-electron-forge/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-electron-forge/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-electron-forge/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-electron-forge/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-electron-forge/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-electron-forge/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-electron-forge/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-electron-forge/build/test-report.html](https://npmtest.github.io/node-npmtest-electron-forge/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-electron-forge/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-electron-forge/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-electron-forge/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-electron-forge/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-electron-forge/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-electron-forge/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-electron-forge/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-electron-forge/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Samuel Attard"
    },
    "babel": {
        "env": {
            "test": {
                "plugins": [
                    "istanbul"
                ]
            }
        },
        "presets": [
            "es2015"
        ],
        "plugins": [
            "transform-runtime",
            "syntax-async-functions",
            [
                "transform-async-to-module-method",
                {
                    "module": "bluebird",
                    "method": "coroutine"
                }
            ]
        ]
    },
    "bin": {
        "electron-forge": "dist/electron-forge.js",
        "forge": "dist/electron-forge.js",
        "electron-forge-vscode-nix": "script/vscode.sh",
        "electron-forge-vscode-win": "script/vscode.cmd"
    },
    "bugs": {
        "url": "https://github.com/electron-userland/electron-forge/issues"
    },
    "config": {
        "commitizen": {
            "path": "./node_modules/cz-customizable"
        },
        "cz-customizable": {
            "config": "./.cz.js"
        }
    },
    "dependencies": {
        "aws-sdk": "^2.9.0",
        "babel-register": "^6.16.3",
        "bluebird": "^3.4.6",
        "colors": "^1.1.2",
        "commander": "^2.9.0",
        "debug": "^2.3.3",
        "electron-forge-template-angular2": "^1.0.3",
        "electron-forge-template-react": "^1.0.2",
        "electron-forge-template-react-typescript": "^1.0.3",
        "electron-forge-template-vue": "^1.0.2",
        "electron-installer-debian": "^0.5.0",
        "electron-installer-dmg": "^0.2.0",
        "electron-installer-flatpak": "^0.4.0",
        "electron-installer-redhat": "^0.4.0",
        "electron-packager": "^8.5.2",
        "electron-rebuild": "^1.5.7",
        "electron-sudo": "github:malept/electron-sudo#fix-linux-sudo-detection",
        "electron-windows-store": "^0.10.1",
        "electron-winstaller": "^2.5.0",
        "fs-promise": "^2.0.0",
        "github": "^9.0.0",
        "glob": "^7.1.1",
        "inquirer": "^3.0.1 ",
        "lodash.template": "^4.4.0",
        "log-symbols": "^1.0.2",
        "node-fetch": "^1.6.3",
        "node-gyp": "^3.4.0",
        "nugget": "^2.0.1",
        "opn": "^4.0.2",
        "ora": "^1.1.0",
        "pify": "^2.3.0",
        "resolve-package": "^1.0.1",
        "s3": "^4.4.0",
        "semver": "^5.3.0",
        "spawn-rx": "^2.0.7",
        "sudo-prompt": "^7.0.0",
        "tabtab": "^2.2.1",
        "username": "^2.2.2",
        "yarn-or-npm": "^2.0.2",
        "zip-folder": "^1.0.0"
    },
    "description": "A complete tool for building modern Electron applications",
    "devDependencies": {
        "babel-eslint": "^7.0.0",
        "babel-plugin-istanbul": "^4.0.0",
        "babel-plugin-syntax-async-functions": "^6.13.0",
        "babel-plugin-transform-async-to-module-method": "^6.16.0",
        "babel-plugin-transform-runtime": "^6.15.0",
        "babel-preset-es2015": "^6.16.0",
        "chai": "^3.5.0",
        "chai-as-promised": "^6.0.0",
        "chai-fetch-mock": "^1.0.0",
        "commitizen": "^2.8.6",
        "coveralls": "^2.11.15",
        "cross-env": "^4.0.0",
        "cz-customizable": "4.0.0",
        "esdoc": "^0.5.1",
        "esdoc-importpath-plugin": "^0.1.0",
        "eslint": "^3.7.1",
        "eslint-config-airbnb-base": "^8.0.0",
        "eslint-plugin-import": "^2.2.0",
        "eslint-plugin-mocha": "^4.8.0",
        "fetch-mock": "^5.8.1",
        "generate-changelog": "^1.0.2",
        "gulp": "^3.9.1",
        "gulp-babel": "^6.1.2",
        "mocha": "^3.2.0",
        "nodemon": "^1.11.0",
        "nyc": "^10.0.0",
        "proxyquire": "^1.7.10",
        "sinon": "^2.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "151ef2f86b677b7f7513a21d3cebed93eae854a0",
        "tarball": "https://registry.npmjs.org/electron-forge/-/electron-forge-2.10.0.tgz"
    },
    "engines": {
        "node": ">= 6.0"
    },
    "gitHead": "c23bfdfef842f08376ca96ed9644bcff61369d24",
    "homepage": "https://github.com/electron-userland/electron-forge#readme",
    "license": "MIT",
    "main": "dist/api/index.js",
    "maintainers": [
        {
            "name": "malept"
        },
        {
            "name": "marshallofsound"
        }
    ],
    "name": "electron-forge",
    "nyc": {
        "reporter": [
            "lcov",
            "text-summary",
            "html"
        ],
        "sourceMap": false,
        "instrument": false,
        "cache": true
    },
    "optionalDependencies": {
        "electron-installer-debian": "^0.5.0",
        "electron-installer-flatpak": "^0.4.0",
        "electron-installer-redhat": "^0.4.0"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/electron-userland/electron-forge.git"
    },
    "scripts": {
        "build": "gulp build",
        "commit": "git-cz",
        "docs": "esdoc",
        "install": "node tabtab-install.js",
        "lint": "eslint src test gulpfile.babel.js",
        "precommit": "npm run lint",
        "prepublish": "gulp build",
        "pretest": "gulp build",
        "release:major": "changelog -M && node ci/fix-changelog.js && git add CHANGELOG.md && git commit -m \"updated CHANGELOG.md\" && npm version major && git push origin && git push origin --tags",
        "release:minor": "changelog -m && node ci/fix-changelog.js && git add CHANGELOG.md && git commit -m \"updated CHANGELOG.md\" && npm version minor && git push origin && git push origin --tags",
        "release:patch": "changelog -p && node ci/fix-changelog.js && git add CHANGELOG.md && git commit -m \"updated CHANGELOG.md\" && npm version patch && git push origin && git push origin --tags",
        "test": "npm run lint && npm run test-all",
        "test-all": "mocha test/**/*_spec*.js --compilers js:babel-register --timeout=300000",
        "test-all-coverage": "cross-env NODE_ENV=test nyc npm run test-all",
        "test-coverage": "npm run lint && npm run test-all-coverage",
        "test-fast": "mocha test/**/*_spec.js --compilers js:babel-register --timeout=10000",
        "test-fast-coverage": "cross-env NODE_ENV=test nyc npm run test-fast",
        "watch": "gulp watch",
        "watch-link": "nodemon --watch src --exec \"npm link\""
    },
    "version": "2.10.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
