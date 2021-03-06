# frontsize

[![Version](http://img.shields.io/:version-4.0.4-E7C04B.svg)](https://github.com/ideatosrl/frontsize/releases/tag/4.0.4)
[![TravisCI](https://travis-ci.org/ideatosrl/frontsize.svg?branch=master)](https://travis-ci.org/ideatosrl/frontsize/builds)
[![Built with SASS](http://img.shields.io/:language-SASS-ff6799.svg)](http://badges.github.io/badgerbadgerbadger/)
[![MIT licence](http://img.shields.io/:license-MIT-00AFFF.svg)](https://github.com/ideatosrl/frontsize/blob/master/LICENSE.md)
[![Join the chat at Gitter](http://img.shields.io/:gitter-chat-00AFFF.svg)](https://gitter.im/ideatosrl/frontsize)

>  Frontsize is not a set of widgets ready to be used in your website, it's a set
>  of mixins and functions to build BEM widgets, it's  a tool to generate your sets.

## Main features

- It's [BEM][bem] ready
- It's build to work with [multiple themes][themes] in the same project
- It's born to be flexible and customization oriented
- It's covered by [tests][test]

The project was [originally developed in LESS][less], now only the SASS version is mantained.

--------------------------------------------------------------------------------

## Release 4.0.4

- Folder `widgets` is renamed to `blocks` necause of frontsize's BEM based nature

## Release 4.0.3

- Adds `$invalidate-cache` var to let `theme` functions for background images generates also a random unique id

## Release 4.0.2

- Fix `vertical-gradient` mixin

## Release 4.0.1

- Adds `$frontsize-release-infos` to theme config
- Removes `a-pollo` module from node dependencies

---
## Install

#### NPM way:

```
npm install --save frontsize
```

#### YARN way:

```
yarn add frontsize
```

--------------------------------------------------------------------------------

## Documentation

Run this command inside frontsize module:

```
cd node_modules/frontsize && npm run styleguideServe
```

This will open a browser window with the documented code.

--------------------------------------------------------------------------------

## Theme installation

Once you have downloaded it, copy your theme to the project front-end development folder:

```
cp -r node_modules/frontsize/themes frontend/frontsize
```

Then change core references to let it point to module folder:

In `frontend/frontsize/_config/import.scss` file:

```sass
@import '../../node_modules/frontsize/core/import';
```

Now the core can be easily upgraded with `npm update frontsize-sass --save` when a new release is available.

--------------------------------------------------------------------------------

To test frontsize:

```
npm install && npm run test
```

Created by [Vittorio Vittori][vitto] and [Alessandro Minoccheri][minompi] @ [ideato srl][ideato]

[bem]: https://github.com/ideatosrl/frontsize/blob/master/test/js/components-bem.js
[ideato]: http://www.ideato.it
[less]: https://github.com/ideatosrl/frontsize-less
[minompi]: https://twitter.com/minompi
[test]: https://github.com/ideatosrl/frontsize/blob/master/test/js/
[themes]: https://github.com/ideatosrl/frontsize/tree/master/themes
[vitto]: https://twitter.com/vttrx
