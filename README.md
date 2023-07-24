<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# isGeneratorObject

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Test if a value is a [`generator`][mdn-generator-object] object.



<section class="usage">

## Usage

```javascript
import isGeneratorObject from 'https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-generator-object@deno/mod.js';
```

#### isGeneratorObject( value )

Tests if a `value` is a [`generator`][mdn-generator-object] object.

<!-- eslint-disable no-restricted-syntax -->

```javascript
function* generateID() {
    var idx = 0;
    while ( idx < idx+1 ) {
        yield idx;
        idx += 1;
    }
}

var bool = isGeneratorObject( generateID() );
// returns true

bool = isGeneratorObject( generateID );
// returns false

bool = isGeneratorObject( {} );
// returns false
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint-disable no-restricted-syntax -->

<!-- eslint no-undef: "error" -->

```javascript
import isGeneratorObject from 'https://cdn.jsdelivr.net/gh/stdlib-js/assert-is-generator-object@deno/mod.js';

function* generator() {
    while ( true ) {
        yield 1.0;
    }
}

var bool = isGeneratorObject( generator() );
// returns true

bool = isGeneratorObject( {} );
// returns false

bool = isGeneratorObject( [] );
// returns false

bool = isGeneratorObject( null );
// returns false
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/assert-has-generator-support`][@stdlib/assert/has-generator-support]</span><span class="delimiter">: </span><span class="description">detect native generator function support.</span>
-   <span class="package-name">[`@stdlib/assert-is-generator-object-like`][@stdlib/assert/is-generator-object-like]</span><span class="delimiter">: </span><span class="description">test if a value is generator object-like.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2023. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/assert-is-generator-object.svg
[npm-url]: https://npmjs.org/package/@stdlib/assert-is-generator-object

[test-image]: https://github.com/stdlib-js/assert-is-generator-object/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/assert-is-generator-object/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/assert-is-generator-object/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/assert-is-generator-object?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/assert-is-generator-object.svg
[dependencies-url]: https://david-dm.org/stdlib-js/assert-is-generator-object/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/assert-is-generator-object/tree/deno
[umd-url]: https://github.com/stdlib-js/assert-is-generator-object/tree/umd
[esm-url]: https://github.com/stdlib-js/assert-is-generator-object/tree/esm
[branches-url]: https://github.com/stdlib-js/assert-is-generator-object/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/assert-is-generator-object/main/LICENSE

[mdn-generator-object]: https://developer.mozilla.org/de/docs/Web/JavaScript/Reference/Global_Objects/Generator

<!-- <related-links> -->

[@stdlib/assert/has-generator-support]: https://github.com/stdlib-js/assert-has-generator-support/tree/deno

[@stdlib/assert/is-generator-object-like]: https://github.com/stdlib-js/assert-is-generator-object-like/tree/deno

<!-- </related-links> -->

</section>

<!-- /.links -->
