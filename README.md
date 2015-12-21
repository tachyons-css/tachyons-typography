# tachyons-typography 1.1.0

Performance based css module.

#### Stats

279 | 12 | 28
---|---|---
bytes | selectors | declarations

## Installation

#### With [npm](https://npmjs.com)

```
npm install --save-dev tachyons-typography
```

#### With Git

```
git clone https://github.com/tachyons-css/tachyons-typography
```

## Usage

#### Using with [PostCSS](https://github.com/postcss/postcss)

Import the css module

```css
@import "tachyons-typography";
```

Then process the CSS using the [`tachyons-cli`](https://github.com/tachyons-css/tachyons-cli)

```sh
$ npm i -g tachyons-cli
$ tachyons-cli path/to/css-file.css > dist/t.css
```

#### Using the CSS

The built CSS is located in the `css` directory. It contains an unminified and minified version.
You can either cut and paste that css or link to it directly in your html.

```html
<link rel="stylesheet" href="path/to/module/css/tachyons-typography">
```

#### Development

The source CSS files can be found in the `src` directory.
Running `$ npm start` will process the source CSS and place the built CSS in the `css` directory.

## The CSS

```css
/*

   TYPOGRAPHY

*/
.measure { max-width: 30em; }
.indent { text-indent: 1em; margin-top: 0; margin-bottom: 0; }
/* Combine this class with a width to truncate text */
.truncate { white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }
@media screen and (min-width: 48em) {
 .measure-ns { max-width: 30em; }
 .indent-ns { text-indent: 1em; margin-top: 0; margin-bottom: 0; }
 .truncate-ns { white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }
}
@media screen and (min-width: 48em) and (max-width: 64em) {
 .measure-m { max-width: 30em; }
 .indent-m { text-indent: 1em; margin-top: 0; margin-bottom: 0; }
 .truncate-m { white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }
}
@media screen and (min-width: 64em) {
 .measure-l { max-width: 30em; }
 .indent-l { text-indent: 1em; margin-top: 0; margin-bottom: 0; }
 .truncate-l { white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }
}
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## Authors

* [mrmrs](http://mrmrs.io)
* [johno](http://johnotander.com)

## License

MIT

