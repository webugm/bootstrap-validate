# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [v2.0.0] - 2018-01-31

This is a big one! Dropping Bootstrap v3 for that bright'n'shiny Bootstrap 4!

### Added

- Feature: You can now use HTML in your error messages. You do need to escape it yourself for the moment.

```javascript
bootstrapValidate('#prename', 'min:20:Enter at least <strong>20</strong> characters.');
```

- Feature: You can now pass an Array of Elements or Selectors as first Argument, for example:

```javascript
bootstrapValidate(['#prename', '#lastname'], 'min:20:Enter at least 20 characters!');
```

This can come in handy when you are applying identical sets of rules and options to multiple input elements.

- Rule: startsWith [fff8678](https://github.com/PascaleBeier/bootstrap-validate/commit/fff867887914a97876ae66c0b4867d46c17a02b6)
- Rule: endsWith [aa51798](https://github.com/PascaleBeier/bootstrap-validate/commit/aa51798fd7702183c683021a60fb8705e0306d2b)
- Rule: matches [208a5cf](https://github.com/PascaleBeier/bootstrap-validate/commit/208a5cf7ab17add9da153addcdcf90eefb9529be)
- Rule: alpha

### Removed

- Polyfills for element.closest() and element.classList().

### Other

- Documentation cleaning
- Housekeeping: Removed most handmade helpers and replaced them with the battle-proven lodash helpers. This drastically improves maintainability and stability.

## [1.0.11] - 2017-08-07

### Added

- Rule: contains

## [1.0.10] - 2017-07-27

### Added

- Rule: alphanum
- Rule: numeric
- Rule: url
- Rule: integer

## [1.0.9] - 2017-07-20

### Added

- Unit Tests

### Fixed

- Fix adding .has-error class to parent element ([#8](https://github.com/PascaleBeier/bootstrap-validate/issues/8))

## [1.0.8] - 2017-07-19

### Added

- Support QuerySelector Notation for Reference Element, enabling you to write

```js
bootstrapValidate('#email', ...)
```

instead of

```js
bootstrapValidate(document.querySelector('#email'), ...)
```

This is a non-breaking change - the old notation is still possible.


## [1.0.7] - 2017-06-16

## [1.0.6] - 2017-06-14

## [1.0.5] - 2017-06-07

## [1.0.4] - 2017-06-07

## [1.0.3] - 2017-06-06

## [1.0.2] - 2017-06-06

## [1.0.1] - 2017-06-06


[v2.0.0]: https://github.com/PascaleBeier/bootstrap-validate/compare/1.0.11...v2.0.0
[1.0.11]: https://github.com/PascaleBeier/bootstrap-validate/compare/1.0.10...1.0.11
[1.0.10]: https://github.com/PascaleBeier/bootstrap-validate/compare/1.0.9...1.0.10
[1.0.9]: https://github.com/PascaleBeier/bootstrap-validate/compare/1.0.8...1.0.9
[1.0.8]: https://github.com/PascaleBeier/bootstrap-validate/compare/1.0.7...1.0.8
[1.0.7]: https://github.com/PascaleBeier/bootstrap-validate/compare/1.0.6...1.0.7
[1.0.6]: https://github.com/PascaleBeier/bootstrap-validate/compare/1.0.5...1.0.6
[1.0.5]: https://github.com/PascaleBeier/bootstrap-validate/compare/1.0.4...1.0.5
[1.0.4]: https://github.com/PascaleBeier/bootstrap-validate/compare/1.0.3...1.0.4
[1.0.3]: https://github.com/PascaleBeier/bootstrap-validate/compare/1.0.2...1.0.3
[1.0.2]: https://github.com/PascaleBeier/bootstrap-validate/compare/1.0.1...1.0.2
[1.0.1]: https://github.com/PascaleBeier/bootstrap-validate/compare/1.0.0...1.0.1
[1.0.0]: https://github.com/PascaleBeier/bootstrap-validate/commit/aa4fbffa625dc389292cc1246bd04573f9371e93

## [1.0.0] - 2017-06-06

> Initial Release
