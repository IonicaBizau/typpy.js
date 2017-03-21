
[![typpy](http://i.imgur.com/FkoAc5n.png)](#)

# typpy

 [![Support me on Patreon][badge_patreon]][patreon] [![Buy me a book][badge_amazon]][amazon] [![PayPal][badge_paypal_donate]][paypal-donations] [![Travis](https://img.shields.io/travis/IonicaBizau/typpy.svg)](https://travis-ci.org/IonicaBizau/typpy/) [![Version](https://img.shields.io/npm/v/typpy.svg)](https://www.npmjs.com/package/typpy) [![Downloads](https://img.shields.io/npm/dt/typpy.svg)](https://www.npmjs.com/package/typpy)

> A better typeof for JavaScript.

## :cloud: Installation

```sh
$ npm i --save typpy
```


## :clipboard: Example



```js
// Dependencies
var Typpy = require("typpy");

console.log(Typpy(0));
// => "number"

console.log(Typpy("", String));
// => true

console.log(Typpy.is(null, "null"));
// => true

console.log(Typpy.get([]));
// => Array

console.log(Typpy({}, true));
// => "object"

console.log(Typpy({}, Object));
// => true
```

## :memo: Documentation


### `Typpy(input, target)`
Gets the type of the input value or compares it
with a provided type.

Usage:

```js
Typpy({}) // => "object"
Typpy(42, Number); // => true
Typpy.get([], "array"); => true
```

#### Params
- **Anything** `input`: The input value.
- **Constructor|String** `target`: The target type. It could be a string (e.g. `"array"`) or a
constructor (e.g. `Array`).

#### Return
- **String|Boolean** It returns `true` if the input has the provided type `target` (if was provided),
`false` if the input type does *not* have the provided type
`target` or the stringified type of the input (always lowercase).

### `Typpy.is(input, target)`
Checks if the input value has a specified type.

#### Params
- **Anything** `input`: The input value.
- **Constructor|String** `target`: The target type. It could be a string (e.g. `"array"`) or a
constructor (e.g. `Array`).

#### Return
- **Boolean** `true`, if the input has the same type with the target or `false` otherwise.

### `Typpy.get(input, str)`
Gets the type of the input value. This is used internally.

#### Params
- **Anything** `input`: The input value.
- **Boolean** `str`: A flag to indicate if the return value should be a string or not.

#### Return
- **Constructor|String** The input value constructor (if any) or the stringified type (always lowercase).



## :yum: How to contribute
Have an idea? Found a bug? See [how to contribute][contributing].


## :sparkling_heart: Support my projects

I open-source almost everything I can, and I try to reply everyone needing help using these projects. Obviously,
this takes time. You can integrate and use these projects in your applications *for free*! You can even change the source code and redistribute (even resell it).

However, if you get some profit from this or just want to encourage me to continue creating stuff, there are few ways you can do it:

 - Starring and sharing the projects you like :rocket:
 - [![PayPal][badge_paypal]][paypal-donations]—You can make one-time donations via PayPal. I'll probably buy a ~~coffee~~ tea. :tea:
 - [![Support me on Patreon][badge_patreon]][patreon]—Set up a recurring monthly donation and you will get interesting news about what I'm doing (things that I don't share with everyone).
 - **Bitcoin**—You can send me bitcoins at this address (or scanning the code below): `1P9BRsmazNQcuyTxEqveUsnf5CERdq35V6`

    ![](https://i.imgur.com/z6OQI95.png)

Thanks! :heart:


## :dizzy: Where is this library used?
If you are using this library in one of your projects, add it in this list. :sparkles:


 - [`animato`](https://github.com/IonicaBizau/animato.js#readme)—Simple way to animate anything (even simple values).
 - [`asyncer.js`](https://github.com/IonicaBizau/asyncer.js#readme)—Run groups of (a)sync functions.
 - [`auto-parse`](https://github.com/greenpioneersolutions/auto-parse#readme) (by Green Pioneer)—auto-parse any value you happen to send in (String, Number, Boolean,Array, Object, Function, undefined and null). You send it we will try to find a way to parse it.support sending in a string of what type (e.g. boolean) or constructor (e.g. Boolean)
 - [`babel-it`](https://github.com/IonicaBizau/babel-it#readme)—Babelify your code before `npm publish`.
 - [`barbe`](https://github.com/IonicaBizau/barbe)—Like mustache, but simple, tiny and fast.
 - [`blah`](https://github.com/IonicaBizau/blah)—A command line tool to optimize the repetitive actions.
 - [`bloggify-ajs-renderer`](https://github.com/IonicaBizau/bloggify-ajs-renderer#readme)—ajs renderer for Bloggify.
 - [`bloggify-flexible-router`](https://github.com/Bloggify/flexible-router#readme) (by Bloggify)—A flexible router for Bloggify apps.
 - [`bug-killer`](https://github.com/IonicaBizau/node-bug-killer)—Simple way to log messages in stdout or other stream.
 - [`cli-circle`](https://github.com/IonicaBizau/node-cli-circle)—Generate ASCII circles with NodeJS.
 - [`cli-gh-cal`](https://github.com/IonicaBizau/cli-gh-cal)—GitHub like calendar graphs in command line.
 - [`color-it`](https://github.com/IonicaBizau/node-color-it#readme)—Flat colors for your Node.js strings.
 - [`couleurs`](https://github.com/IonicaBizau/node-couleurs)—Add some color and styles to your Node.JS strings.
 - [`deffy`](https://github.com/IonicaBizau/deffy.js)—Small and fast library to set default values.
 - [`diable`](https://github.com/IonicaBizau/diable)—Daemonize the things out.
 - [`dom-repeater`](https://github.com/IonicaBizau/dom-repeater#readme)—Render lists in DOM easily.
 - [`elm-select`](https://github.com/IonicaBizau/elm-select)—Select DOM elements and optionally call a function.
 - [`engine-builder`](https://github.com/IonicaBizau/engine-parser) (by jillix)—Engine composition parser.
 - [`engine-flow-types`](https://github.com/jillix/engine-flow-types#readme) (by jillix)—Low level library providing Engine flow types.
 - [`engine-parser`](https://github.com/IonicaBizau/engine-parser) (by jillix)—Engine composition parser.
 - [`enny`](https://github.com/IonicaBizau/enny) (by jillix)—Generate Engine compositions from human-readable inputs.
 - [`err`](https://github.com/IonicaBizau/err#readme)—A tiny library to create custom errors in JavaScript.
 - [`exec-limiter`](https://github.com/IonicaBizau/exec-limiter)—Limit the shell execution commands to <x> calls same time.
 - [`flattenize`](https://github.com/IonicaBizau/node-flattenize)—An experiment for converting images in flat equivalents.
 - [`gh-repos`](https://github.com/IonicaBizau/gh-repos#readme)—Get one or all the owner repositories from GitHub.
 - [`ghcal`](https://github.com/IonicaBizau/ghcal)—See the GitHub contributions calendar of a user in the command line.
 - [`ghosty`](https://github.com/IonicaBizau/ghosty#readme)—A wrapper around PhantomJS, downloading the Phantom binary.
 - [`git-stats`](https://github.com/IonicaBizau/git-stats)—Local git statistics including GitHub-like contributions calendars.
 - [`git-stats-importer`](https://github.com/IonicaBizau/git-stats-importer)—Imports your commits from a repository into git-stats history.
 - [`limit-it`](https://github.com/IonicaBizau/node-limit-it)—Run in parallel as many functions you want, but not more than <x> functions at the time.
 - [`obj-flatten`](https://github.com/IonicaBizau/obj-flatten#readme)—Convert nested objects in flatten ones.
 - [`page-changed`](https://github.com/IonicaBizau/node-page-changed)—Call a function when the page body is changed.
 - [`regarde`](https://github.com/IonicaBizau/regarde)—A tiny tool and library to watch commands.
 - [`scrape-it`](https://github.com/IonicaBizau/scrape-it#readme)—A Node.js scraper for humans.
 - [`tilda`](https://github.com/IonicaBizau/tilda)—Tiny module for building command line tools.
 - [`transformer`](https://github.com/IonicaBizau/transformer#readme)—Transform data using synchronous and asynchronous functions.
 - [`ul`](https://github.com/IonicaBizau/node-ul)—A minimalist utility library.
 - [`validify`](https://github.com/IonicaBizau/validify#readme)—Validation made easy.
 - [`write-file-p`](https://github.com/IonicaBizau/write-file-p#readme)—Create the directory structure and then create the file.

## :scroll: License

[MIT][license] © [Ionică Bizău][website]

[badge_patreon]: http://ionicabizau.github.io/badges/patreon.svg
[badge_amazon]: http://ionicabizau.github.io/badges/amazon.svg
[badge_paypal]: http://ionicabizau.github.io/badges/paypal.svg
[badge_paypal_donate]: http://ionicabizau.github.io/badges/paypal_donate.svg
[patreon]: https://www.patreon.com/ionicabizau
[amazon]: http://amzn.eu/hRo9sIZ
[paypal-donations]: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=RVXDDLKKLQRJW
[donate-now]: http://i.imgur.com/6cMbHOC.png

[license]: http://showalicense.com/?fullname=Ionic%C4%83%20Biz%C4%83u%20%3Cbizauionica%40gmail.com%3E%20(https%3A%2F%2Fionicabizau.net)&year=2015#license-mit
[website]: https://ionicabizau.net
[contributing]: /CONTRIBUTING.md
[docs]: /DOCUMENTATION.md
