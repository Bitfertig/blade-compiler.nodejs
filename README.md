# Blade Compiler

This package compiles blade templates to HTML.

## Installation

Via NPM:
```console
$ npm install @bitfertig/blade-compiler.nodejs
```

## Usage

Require the package and compile a blade file:
```js
var prop = { title: 'MyTitle' }; // Data
var bladeCompiler = require('@bitfertig/blade-compiler.nodejs');
var compiledHTML = bladeCompiler({ folder: './src', file: '/index' });
console.log(compiledHTML);
```

./src/index.blade.html
```html
<html>
    <head>{{ prop.title }}</head>
    <body>
        @include('partials.header')
    </body>
</html>
```

./src/partials/header.blade.html
```html
<header>Hello World.</header>
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

Cloned from https://github.com/pbelyaev/laravel-blade-compiler
