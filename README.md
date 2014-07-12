# condense-newlines [![NPM version](https://badge.fury.io/js/condense-newlines.png)](http://badge.fury.io/js/condense-newlines)

> Replace extraneous newlines with a single newline, or pass a specified number of newlines to use.

## Install
Install with [npm](npmjs.org):

```bash
npm i condense-newlines --save-dev
```

## Usage

```js
var condense = require('condense-newlines');
console.log(condense('\n\na\n\n\nb\nc\r\n\r\nd\n\n\n'));
//=> 'a\nb\nc\nd';
```

### Specify number of newlines

```js
console.log(condense('\n\na\n\n\nb\nc\r\n\r\nd\n\n\n', '\n\n'));
//=> 'a\n\nb\n\nc\n\nd';
```

Note that leading and trailing newlines are also removed.

## Author

**Jon Schlinkert**
 
+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert) 

## License
Copyright (c) 2014 Jon Schlinkert, contributors.  
Released under the MIT license

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on July 12, 2014._