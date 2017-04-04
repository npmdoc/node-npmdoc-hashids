# api documentation for  [hashids (v1.1.1)](http://hashids.org/javascript)  [![npm package](https://img.shields.io/npm/v/npmdoc-hashids.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-hashids) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-hashids.svg)](https://travis-ci.org/npmdoc/node-npmdoc-hashids)
#### Generate YouTube-like ids from numbers. Use Hashids when you do not want to expose your database ids to the user.

[![NPM](https://nodei.co/npm/hashids.png?downloads=true)](https://www.npmjs.com/package/hashids)

[![apidoc](https://npmdoc.github.io/node-npmdoc-hashids/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-hashids_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-hashids/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-hashids/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-hashids/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Ivan Akimov",
        "email": "ivan@barreleye.com",
        "url": "https://twitter.com/IvanAkimov"
    },
    "bugs": {
        "url": "https://github.com/ivanakimov/hashids.js/issues"
    },
    "dependencies": {},
    "description": "Generate YouTube-like ids from numbers. Use Hashids when you do not want to expose your database ids to the user.",
    "devDependencies": {
        "babel-cli": "^6.10.1",
        "babel-core": "^6.10.4",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-transform-es2015-modules-umd": "^6.8.0",
        "babel-preset-es2015": "^6.9.0",
        "chai": "^3.5.0",
        "coveralls": "^2.11.9",
        "eslint": "^3.0.1",
        "mocha": "^2.5.3",
        "nyc": "^7.0.0",
        "uglify-js": "^2.7.0"
    },
    "directories": {},
    "dist": {
        "shasum": "3c36fcc5b3ba1a96a8fa67a632eb7877c41c6d3e",
        "tarball": "https://registry.npmjs.org/hashids/-/hashids-1.1.1.tgz"
    },
    "gitHead": "38e8975ecbbed956554ab8ed037f2d2c2549c293",
    "homepage": "http://hashids.org/javascript",
    "keywords": [
        "hashids",
        "hashid",
        "hash",
        "ids",
        "youtube",
        "bitly",
        "obfuscate",
        "encode",
        "decode",
        "encrypt",
        "decrypt"
    ],
    "license": "MIT",
    "main": "dist/hashids.js",
    "maintainers": [
        {
            "name": "ivan",
            "email": "ivan@grather.com"
        }
    ],
    "name": "hashids",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/ivanakimov/hashids.js.git"
    },
    "scripts": {
        "all": "npm run lint && npm run coverage && npm run build && npm run clean",
        "build": "npm run test && npm run build:node && npm run rename:global && npm run minify",
        "build:node": "babel lib/hashids.js -o dist/hashids.js",
        "clean": "rm -rf coverage .nyc_output npm-debug.log",
        "coverage": "nyc npm test && nyc report --reporter=text-lcov | coveralls",
        "lint": "eslint lib tests",
        "minify": "uglifyjs dist/hashids.js -o dist/hashids.min.js --source-map dist/hashids.min.map --compress --mangle",
        "rename:global": "sed -i '' 's/global.hashids/global.Hashids/g' dist/hashids.js",
        "test": "mocha tests --compilers js:babel-core/register"
    },
    "version": "1.1.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module hashids](#apidoc.module.hashids)



# <a name="apidoc.module.hashids"></a>[module hashids](#apidoc.module.hashids)



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
