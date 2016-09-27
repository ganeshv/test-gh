# test-gh
Testing automatic gh-pages

```js
var run = require('gentrify').run;

function* getQuote(sym) {
    /* invoke a promise-based API */
    const qstr = yield rp(`https://www.google.com/finance/info?q=${sym}`),
        quote = JSON.parse(qstr.slice(qstr.indexOf('[')));
    return +quote[0].l_cur;
}
```
