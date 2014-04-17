*This repository is a mirror of the [component](http://component.io) module [sindresorhus/strip-indent](http://github.com/sindresorhus/strip-indent). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/sindresorhus-strip-indent`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# strip-indent [![Build Status](https://travis-ci.org/sindresorhus/strip-indent.svg?branch=master)](https://travis-ci.org/sindresorhus/strip-indent)

> Strip leading whitespace from every line in a string

The line with the least number of leading whitespace, ignoring empty lines, determines the number to remove.

Useful for removing redundant indentation.


## Install

```bash
$ npm install --save strip-indent
```

```bash
$ bower install --save strip-indent
```

```bash
$ component install sindresorhus/strip-indent
```


## Usage

```js
var str = '\tunicorn\n\t\tcake';
/*
	unicorn
		cake
*/

stripIndent('\tunicorn\n\t\tcake');
/*
unicorn
	cake
*/
```


## CLI

```bash
$ npm install --global strip-indent
```

```bash
$ strip-indent --help

Usage
  $ strip-indent <file>
  $ echo <string> | strip-indent

Example
  $ echo '\tunicorn\n\t\tcake' | strip-indent
  unicorn
  	cake
```


## License

[MIT](http://opensource.org/licenses/MIT) © [Sindre Sorhus](http://sindresorhus.com)
