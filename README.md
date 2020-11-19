ATTENTION: FORKED REPO, NOT READY FOR PRODUCTION!


# Blade Parser

This package compiles blade templates to HTML.
 
## Installation
 
Via NPM:
```console
$ npm install @bitfertig/blade-compiler.nodejs
```

## Usage

Require the package:
```js
var bladeCompiler = require('@bitfertig/blade-compiler.nodejs');
```

Then you can use the package like so:
```js
var compiledHTML = bladeCompiler({ folder: './src', file: '/index' });
```

## Options

| Name | Type | Default value | Description |
|---|---|---|---|
| encoding | string | utf8 | Blade templates encoding |
| extends | boolean | true | Enable/disable compiling @extends directives |
| folder | string | ./src | Path to the views directory |
| file | string | /index | Path to the compiled blade template file |
| extension | string | .blade.html | Blade file extension |


## Author
Aurelian Hermand, www.bitfertig.de
