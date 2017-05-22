[![js-semistandard-style](https://img.shields.io/badge/code%20style-semistandard-brightgreen.svg?style=flat-square)](https://github.com/Flet/semistandard)
# NO:DOM
fake DOM for [RE:DOM](https://redom.js.org)

## installing
```
npm install nodom
```

## usage
```js
const { Document } = require('nodom');
global.document = new Document();
const { el, mount } = require('redom');

mount(document.body, el('h1', 'Hello world!'));

console.log(document.body.outerHTML); // <body><h1>Hello world!</h1></body>
```
