<!--

@license Apache-2.0

Copyright (c) 2024 The Stdlib Authors.

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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# Cosecant

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Evaluate the [cosecant][trigonometric-functions] of a number.

<section class="intro">

</section>



<section class="usage">

## Usage

To use in Observable,

```javascript
csc = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-csc@umd/browser.js' )
```

To vendor stdlib functionality and avoid installing dependency trees for Node.js, you can use the UMD server build:

```javascript
var csc = require( 'path/to/vendor/umd/math-base-special-csc/index.js' )
```

To include the bundle in a webpage,

```html
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-csc@umd/browser.js"></script>
```

If no recognized module system is present, access bundle contents via the global scope:

```html
<script type="text/javascript">
(function () {
    window.csc;
})();
</script>
```

## csc( x )

Evaluates the [cosecant][trigonometric-functions] of `x` (in radians).

```javascript
var v = csc( 0.0 );
// returns Infinity

v = csc( 3.141592653589793/2.0 );
// returns 1.0

v = csc( -3.141592653589793/6.0 );
// returns ~-2.0

v = csc( 3.141592653589793/6.0 );
// returns ~2.0

v = csc( NaN );
// returns NaN
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/random-array-uniform@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/console-log-each-map@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/constants-float64-two-pi@umd/browser.js"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-csc@umd/browser.js"></script>
<script type="text/javascript">
(function () {

var opts = {
    'dtype': 'float64'
};
var x = uniform( 100, -TWO_PI, TWO_PI, opts );

logEachMap( 'csc(%0.4f) = %0.4f', x, csc );

})();
</script>
</body>
</html>
```

</section>

<!-- /.examples -->

<!-- C interface documentation. -->



<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/math-base/special/cot`][@stdlib/math/base/special/cot]</span><span class="delimiter">: </span><span class="description">evaluate the cotangent of a number.</span>
-   <span class="package-name">[`@stdlib/math-base/special/sin`][@stdlib/math/base/special/sin]</span><span class="delimiter">: </span><span class="description">compute the sine of a number.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2025. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-csc.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-csc

[test-image]: https://github.com/stdlib-js/math-base-special-csc/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/math-base-special-csc/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-csc/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-csc?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-csc.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-csc/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-csc/tree/deno
[deno-readme]: https://github.com/stdlib-js/math-base-special-csc/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/math-base-special-csc/tree/umd
[umd-readme]: https://github.com/stdlib-js/math-base-special-csc/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/math-base-special-csc/tree/esm
[esm-readme]: https://github.com/stdlib-js/math-base-special-csc/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/math-base-special-csc/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-csc/main/LICENSE

[trigonometric-functions]: https://en.wikipedia.org/wiki/Trigonometric_functions

<!-- <related-links> -->

[@stdlib/math/base/special/cot]: https://github.com/stdlib-js/math-base-special-cot/tree/umd

[@stdlib/math/base/special/sin]: https://github.com/stdlib-js/math-base-special-sin/tree/umd

<!-- </related-links> -->

</section>

<!-- /.links -->
