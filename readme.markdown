[![NPM version](http://img.shields.io/npm/v/insert-css2.svg)](https://www.npmjs.org/package/insert-css2)

# insert-css2

insert a string of css into the `<head>`. Maintenance fork.

# example

``` js
    var insertCss = require('insert-css');
    var styleElement = insertCss('body { background:blue; }');
```

# api

``` js
    var insertCss = require('insert-css');
```

## var styleElement = insertCss(css, opts);

Insert some CSS into the page.

* `opts.container` - Which HTMLElement to use as the base mounting point, defaults to
`document.querySelector('head')`.

* `opts.prepend` - Add the CSS at the top level of the container instead of at the bottom level (default).

This is particullary useful for library creators where you may want your default CSS to be prepended so it
can be easily overriden by user styles.

# development

## example

``` sh
npm run example
```

## test

``` sh
npm test
```
