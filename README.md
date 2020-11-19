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
var compiledHTML = bladeCompiler({
    extension: '.blade.html',
    folder: 'src/',
    path: 'src/index.blade.html'
});
```

## Options

| Name | Type | Default value | Description |
|---|---|---|---|
| extension | string | .blade.html | Blade file extension |
| extends | boolean | true | Enable/disable compiling @extends directives |
| folder | string | ./resources/views | Path to the views directory |
| encoding | string | utf8 | Blade templates encoding |
| path | string | ./resources/views/welcome.blade.php | Path to the compiled blade template file |


## Author
Aurelian Hermand, www.bitfertig.de
