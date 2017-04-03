# api documentation for  [postcss-loader (v1.3.3)](https://github.com/postcss/postcss-loader#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-postcss-loader.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-postcss-loader) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-postcss-loader.svg)](https://travis-ci.org/npmdoc/node-npmdoc-postcss-loader)
#### PostCSS loader for webpack

[![NPM](https://nodei.co/npm/postcss-loader.png?downloads=true)](https://www.npmjs.com/package/postcss-loader)

[![apidoc](https://npmdoc.github.io/node-npmdoc-postcss-loader/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-postcss-loader_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-postcss-loader/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-postcss-loader/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-postcss-loader/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Andrey Sitnik",
        "email": "andrey@sitnik.ru"
    },
    "bugs": {
        "url": "https://github.com/postcss/postcss-loader/issues"
    },
    "dependencies": {
        "loader-utils": "^1.0.2",
        "object-assign": "^4.1.1",
        "postcss": "^5.2.15",
        "postcss-load-config": "^1.2.0"
    },
    "description": "PostCSS loader for webpack",
    "devDependencies": {
        "eslint": "^3.16.1",
        "eslint-config-postcss": "^2.0.2",
        "fs-extra": "^2.0.0",
        "gulp": "^3.9.1",
        "gulp-eslint": "^3.0.1",
        "gulp-jest": "^1.0.0",
        "jest-cli": "^19.0.2",
        "json-loader": "^0.5.4",
        "lint-staged": "^3.3.1",
        "postcss-js": "^0.3.0",
        "postcss-safe-parser": "^2.0.0",
        "pre-commit": "^1.2.2",
        "raw-loader": "^0.5.1",
        "sugarss": "^0.2.0",
        "webpack-stream": "^3.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "a621ea1fa29062a83972a46f54486771301916eb",
        "tarball": "https://registry.npmjs.org/postcss-loader/-/postcss-loader-1.3.3.tgz"
    },
    "engines": {
        "node": ">=0.12"
    },
    "eslintConfig": {
        "extends": "eslint-config-postcss/es5",
        "env": {
            "jest": true
        }
    },
    "gitHead": "e101b845eaa8e7ad006e9a8294c3d64b9061b86c",
    "homepage": "https://github.com/postcss/postcss-loader#readme",
    "keywords": [
        "webpack",
        "loader",
        "css",
        "postcss",
        "postcss-runner"
    ],
    "license": "MIT",
    "lint-staged": {
        "*.js": "eslint"
    },
    "maintainers": [
        {
            "name": "ai",
            "email": "andrey@sitnik.ru"
        }
    ],
    "name": "postcss-loader",
    "optionalDependencies": {},
    "pre-commit": [
        "lint-staged"
    ],
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/postcss/postcss-loader.git"
    },
    "scripts": {
        "lint-staged": "lint-staged",
        "test": "gulp"
    },
    "version": "1.3.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module postcss-loader](#apidoc.module.postcss-loader)
1.  [function <span class="apidocSignatureSpan">postcss-loader.</span>error (error)](#apidoc.element.postcss-loader.error)
1.  object <span class="apidocSignatureSpan">postcss-loader.</span>error.prototype

#### [module postcss-loader.error](#apidoc.module.postcss-loader.error)
1.  [function <span class="apidocSignatureSpan">postcss-loader.</span>error (error)](#apidoc.element.postcss-loader.error.error)

#### [module postcss-loader.error.prototype](#apidoc.module.postcss-loader.error.prototype)
1.  [function <span class="apidocSignatureSpan">postcss-loader.error.prototype.</span>constructor (error)](#apidoc.element.postcss-loader.error.prototype.constructor)



# <a name="apidoc.module.postcss-loader"></a>[module postcss-loader](#apidoc.module.postcss-loader)

#### <a name="apidoc.element.postcss-loader.error"></a>[function <span class="apidocSignatureSpan">postcss-loader.</span>error (error)](#apidoc.element.postcss-loader.error)
- description and source-code
```javascript
function PostCSSLoaderError(error) {
    Error.call(this);
    Error.captureStackTrace(this, PostCSSLoaderError);
    this.name = 'Syntax Error';
    this.error = error.input.source;
    this.message = error.reason;
    if ( error.line ) {
        this.message += ' (' + error.line + ':' + error.column + ')';
    }
    if ( error.line && error.input.source ) {
        this.message += '\n\n' + error.showSourceCode() + '\n';
    }
    this.hideStack = true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss-loader.error"></a>[module postcss-loader.error](#apidoc.module.postcss-loader.error)

#### <a name="apidoc.element.postcss-loader.error.error"></a>[function <span class="apidocSignatureSpan">postcss-loader.</span>error (error)](#apidoc.element.postcss-loader.error.error)
- description and source-code
```javascript
function PostCSSLoaderError(error) {
    Error.call(this);
    Error.captureStackTrace(this, PostCSSLoaderError);
    this.name = 'Syntax Error';
    this.error = error.input.source;
    this.message = error.reason;
    if ( error.line ) {
        this.message += ' (' + error.line + ':' + error.column + ')';
    }
    if ( error.line && error.input.source ) {
        this.message += '\n\n' + error.showSourceCode() + '\n';
    }
    this.hideStack = true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.postcss-loader.error.prototype"></a>[module postcss-loader.error.prototype](#apidoc.module.postcss-loader.error.prototype)

#### <a name="apidoc.element.postcss-loader.error.prototype.constructor"></a>[function <span class="apidocSignatureSpan">postcss-loader.error.prototype.</span>constructor (error)](#apidoc.element.postcss-loader.error.prototype.constructor)
- description and source-code
```javascript
function PostCSSLoaderError(error) {
    Error.call(this);
    Error.captureStackTrace(this, PostCSSLoaderError);
    this.name = 'Syntax Error';
    this.error = error.input.source;
    this.message = error.reason;
    if ( error.line ) {
        this.message += ' (' + error.line + ':' + error.column + ')';
    }
    if ( error.line && error.input.source ) {
        this.message += '\n\n' + error.showSourceCode() + '\n';
    }
    this.hideStack = true;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
