# SUIT CSS utilities: after

[![Build Status](https://travis-ci.org/suitcss/utils-after.svg?branch=master)](https://travis-ci.org/suitcss/utils-after)

SUIT CSS trailing offset utilities.

Read more about [SUIT CSS's design principles](https://github.com/suitcss/suit/).

## Installation

* [npm](http://npmjs.org/): `npm install suitcss-utils-after`
* Download: [zip](https://github.com/suitcss/utils-after/releases/latest)

## Available classes

* `u-afterXofY` (numerous) - Specify the proportional offset after an object.

`X` must be an integer less than `Y`.

`Y` can be any of the following numbers: 2, 3, 4, 5, 6, 8, 10, 12.

### Plugins

Utilities that can be limited to specific Media Query breakpoints.

* `u-sm-afterXofY` - To use at the smallest Media Query breakpoint.
* `u-md-afterXofY` - To use at the medium Media Query breakpoint.
* `u-lg-afterXofY` - To use at the large Media Query breakpoint.

### Configuration

There are 3 Media Query breakpoints:

* `--sm-viewport`
* `--md-viewport`
* `--lg-viewport`

When using the [SUIT CSS preprocessor](https://github.com/suitcss/preprocessor),
breakpoints can be configured using `@custom-media`. For example:

```css
@custom-media --sm-viewport (min-width:320px) and (max-width:640px);
@custom-media --md-viewport (min-width:640px) and (max-width:960px);
@custom-media --lg-viewport (min-width:960px);
```

## Usage

Please refer to the README for [SUIT CSS utils](https://github.com/suitcss/utils/)

## Testing

Install [Node](http://nodejs.org) (comes with npm).

```
npm install
```

To generate a build:

```
npm run build
```

To lint code with [postcss-bem-linter](https://github.com/postcss/postcss-bem-linter) and [stylelint](http://stylelint.io/)

```
npm run lint
```

To generate the testing build.

```
npm run build-test
```

To watch the files for making changes to test:

```
npm run watch
```

Basic visual tests are in `test/index.html`.

## Browser support

* Google Chrome (latest)
* Opera (latest)
* Firefox 4+
* Safari 5+
* Internet Explorer 8+
