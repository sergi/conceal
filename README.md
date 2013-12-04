# conceal <a href="http://flattr.com/thing/1452098/" target="_blank"><img src="http://api.flattr.com/button/flattr-badge-large.png" alt="Flattr this" title="Flattr this" border="0" /></a>

[![NPM](https://nodei.co/npm/conceal.png)](https://nodei.co/npm/conceal/)

Node.js module for obfuscating a string or a part of it. I've needed this functionality several
times now and I've decided to make a micro-module for it. It is useful to
conceal sensitive strings such as passwords, or parts of a string, e.g. a
credit card to show the user.

``` js
var conceal = require('conceal');

var str = 'Big Secret';

conceal(str);
// '**********'

conceal(str, { ch: '^' });
// '^^^^^^^^^^'

conceal(str, { start: 4, end: 6 });
// 'Big ***ret'

```

## Install

```
npm install conceal
```

## License

MIT
