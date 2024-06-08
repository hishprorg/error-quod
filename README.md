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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# ndarray

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Multidimensional arrays.

<section class="installation">

## Installation

```bash
npm install @hishprorg/error-quod
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm`][esm-url] branch (see [README][esm-readme]).
-   If you are using Deno, visit the [`deno`][deno-url] branch (see [README][deno-readme] for usage intructions).
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd`][umd-url] branch (see [README][umd-readme]).

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

To view installation and usage instructions specific to each branch build, be sure to explicitly navigate to the respective README files on each branch, as linked to above.

</section>

<section class="usage">

## Usage

```javascript
var ns = require( '@hishprorg/error-quod' );
```

#### ns

ndarray namespace.

```javascript
var o = ns;
// returns {...}
```

The namespace exports the following functions to create multidimensional arrays:

<!-- <toc pattern="+(array|ctor)"> -->

<div class="namespace-toc">

-   <span class="signature">[`array( [buffer,] [options] )`][@hishprorg/error-quod/array]</span><span class="delimiter">: </span><span class="description">create a multidimensional array.</span>
-   <span class="signature">[`ndarray( dtype, buffer, shape, strides, offset, order[, options] )`][@hishprorg/error-quod/ctor]</span><span class="delimiter">: </span><span class="description">multidimensional array constructor.</span>

</div>

<!-- </toc> -->

The namespace contains the following sub-namespaces:

<!-- <toc pattern="+(base|iter)"> -->

<div class="namespace-toc">

-   <span class="signature">[`base`][@hishprorg/error-quod/base]</span><span class="delimiter">: </span><span class="description">base ndarray.</span>
-   <span class="signature">[`iter`][@hishprorg/error-quod/iter]</span><span class="delimiter">: </span><span class="description">multidimensional array iterators.</span>

</div>

<!-- </toc> -->

In addition, the namespace contains the following multidimensional array utility functions:

<!-- <toc pattern="*" > -->

<div class="namespace-toc">

-   <span class="signature">[`at( x[, ...indices] )`][@hishprorg/error-quod/at]</span><span class="delimiter">: </span><span class="description">return an `ndarray` element.</span>
-   <span class="signature">[`broadcastArray( x, shape )`][@hishprorg/error-quod/broadcast-array]</span><span class="delimiter">: </span><span class="description">broadcast an ndarray to a specified shape.</span>
-   <span class="signature">[`broadcastArrays( ...arrays )`][@hishprorg/error-quod/broadcast-arrays]</span><span class="delimiter">: </span><span class="description">broadcast ndarrays to a common shape.</span>
-   <span class="signature">[`castingModes()`][@hishprorg/error-quod/casting-modes]</span><span class="delimiter">: </span><span class="description">list of ndarray casting modes.</span>
-   <span class="signature">[`dataBuffer( x )`][@hishprorg/error-quod/data-buffer]</span><span class="delimiter">: </span><span class="description">return the underlying data buffer of a provided ndarray.</span>
-   <span class="signature">[`defaults()`][@hishprorg/error-quod/defaults]</span><span class="delimiter">: </span><span class="description">default ndarray settings.</span>
-   <span class="signature">[`dispatch( fcns, types, data, nargs, nin, nout )`][@hishprorg/error-quod/dispatch]</span><span class="delimiter">: </span><span class="description">create an ndarray function interface which performs multiple dispatch.</span>
-   <span class="signature">[`dtype( x )`][@hishprorg/error-quod/dtype]</span><span class="delimiter">: </span><span class="description">return the data type of a provided ndarray.</span>
-   <span class="signature">[`dtypes( [kind] )`][@hishprorg/error-quod/dtypes]</span><span class="delimiter">: </span><span class="description">list of ndarray data types.</span>
-   <span class="signature">[`emptyLike( x[, options] )`][@hishprorg/error-quod/empty-like]</span><span class="delimiter">: </span><span class="description">create an uninitialized ndarray having the same shape and data type as a provided ndarray.</span>
-   <span class="signature">[`empty( shape[, options] )`][@hishprorg/error-quod/empty]</span><span class="delimiter">: </span><span class="description">create an uninitialized ndarray having a specified shape and data type.</span>
-   <span class="signature">[`FancyArray( dtype, buffer, shape, strides, offset, order[, options] )`][@hishprorg/error-quod/fancy]</span><span class="delimiter">: </span><span class="description">fancy multidimensional array constructor.</span>
-   <span class="signature">[`flag( x, name )`][@hishprorg/error-quod/flag]</span><span class="delimiter">: </span><span class="description">return a specified flag for a provided ndarray.</span>
-   <span class="signature">[`flags( x )`][@hishprorg/error-quod/flags]</span><span class="delimiter">: </span><span class="description">return the flags of a provided ndarray.</span>
-   <span class="signature">[`scalar2ndarray( value[, options] )`][@hishprorg/error-quod/from-scalar]</span><span class="delimiter">: </span><span class="description">convert a scalar value to a zero-dimensional ndarray.</span>
-   <span class="signature">[`ind2sub( shape, idx[, options] )`][@hishprorg/error-quod/ind2sub]</span><span class="delimiter">: </span><span class="description">convert a linear index to an array of subscripts.</span>
-   <span class="signature">[`indexModes()`][@hishprorg/error-quod/index-modes]</span><span class="delimiter">: </span><span class="description">list of ndarray index modes.</span>
-   <span class="signature">[`maybeBroadcastArray( x, shape )`][@hishprorg/error-quod/maybe-broadcast-array]</span><span class="delimiter">: </span><span class="description">broadcast an ndarray to a specified shape if and only if the specified shape differs from the provided ndarray's shape.</span>
-   <span class="signature">[`maybeBroadcastArrays( arrays )`][@hishprorg/error-quod/maybe-broadcast-arrays]</span><span class="delimiter">: </span><span class="description">broadcast ndarrays to a common shape.</span>
-   <span class="signature">[`minDataType( value )`][@hishprorg/error-quod/min-dtype]</span><span class="delimiter">: </span><span class="description">determine the minimum ndarray data type of the closest "kind" necessary for storing a provided scalar value.</span>
-   <span class="signature">[`mostlySafeCasts( [dtype] )`][@hishprorg/error-quod/mostly-safe-casts]</span><span class="delimiter">: </span><span class="description">return a list of ndarray data types to which a provided ndarray data type can be safely cast and, for floating-point data types, can be downcast.</span>
-   <span class="signature">[`ndims( x )`][@hishprorg/error-quod/ndims]</span><span class="delimiter">: </span><span class="description">return the number of ndarray dimensions.</span>
-   <span class="signature">[`nextDataType( [dtype] )`][@hishprorg/error-quod/next-dtype]</span><span class="delimiter">: </span><span class="description">return the next larger ndarray data type of the same kind.</span>
-   <span class="signature">[`numelDimension( x, dim )`][@hishprorg/error-quod/numel-dimension]</span><span class="delimiter">: </span><span class="description">return the size (i.e., number of elements) of a specified dimension for a provided ndarray.</span>
-   <span class="signature">[`numel( x )`][@hishprorg/error-quod/numel]</span><span class="delimiter">: </span><span class="description">return the number of elements in an ndarray.</span>
-   <span class="signature">[`offset( x )`][@hishprorg/error-quod/offset]</span><span class="delimiter">: </span><span class="description">return the index offset specifying the underlying buffer index of the first iterated ndarray element.</span>
-   <span class="signature">[`order( x )`][@hishprorg/error-quod/order]</span><span class="delimiter">: </span><span class="description">return the layout order of a provided ndarray.</span>
-   <span class="signature">[`orders()`][@hishprorg/error-quod/orders]</span><span class="delimiter">: </span><span class="description">list of ndarray orders.</span>
-   <span class="signature">[`outputDataTypePolicies()`][@hishprorg/error-quod/output-dtype-policies]</span><span class="delimiter">: </span><span class="description">list of output ndarray data type policies.</span>
-   <span class="signature">[`promotionRules( [dtype1, dtype2] )`][@hishprorg/error-quod/promotion-rules]</span><span class="delimiter">: </span><span class="description">return the ndarray data type with the smallest size and closest "kind" to which ndarray data types can be **safely** cast.</span>
-   <span class="signature">[`safeCasts( [dtype] )`][@hishprorg/error-quod/safe-casts]</span><span class="delimiter">: </span><span class="description">return a list of ndarray data types to which a provided ndarray data type can be safely cast.</span>
-   <span class="signature">[`sameKindCasts( [dtype] )`][@hishprorg/error-quod/same-kind-casts]</span><span class="delimiter">: </span><span class="description">return a list of ndarray data types to which a provided ndarray data type can be safely cast or cast within the same "kind".</span>
-   <span class="signature">[`shape( x )`][@hishprorg/error-quod/shape]</span><span class="delimiter">: </span><span class="description">return the shape of a provided ndarray.</span>
-   <span class="signature">[`sliceAssign( x, y, ...s[, options] )`][@hishprorg/error-quod/slice-assign]</span><span class="delimiter">: </span><span class="description">assign element values from a broadcasted input `ndarray` to corresponding elements in an output `ndarray` view.</span>
-   <span class="signature">[`sliceDimensionFrom( x, dim, start[, options] )`][@hishprorg/error-quod/slice-dimension-from]</span><span class="delimiter">: </span><span class="description">return a read-only shifted view of an input `ndarray` along a specified dimension.</span>
-   <span class="signature">[`sliceDimensionTo( x, dim, stop[, options] )`][@hishprorg/error-quod/slice-dimension-to]</span><span class="delimiter">: </span><span class="description">return a read-only truncated view of an input `ndarray` along a specified dimension.</span>
-   <span class="signature">[`sliceDimension( x, dim, slice[, options] )`][@hishprorg/error-quod/slice-dimension]</span><span class="delimiter">: </span><span class="description">return a read-only view of an input `ndarray` when sliced along a specified dimension.</span>
-   <span class="signature">[`sliceFrom( x, ...start[, options] )`][@hishprorg/error-quod/slice-from]</span><span class="delimiter">: </span><span class="description">return a read-only shifted view of an input ndarray.</span>
-   <span class="signature">[`sliceTo( x, ...stop[, options] )`][@hishprorg/error-quod/slice-to]</span><span class="delimiter">: </span><span class="description">return a read-only truncated view of an input ndarray.</span>
-   <span class="signature">[`slice( x, ...s[, options] )`][@hishprorg/error-quod/slice]</span><span class="delimiter">: </span><span class="description">return a read-only view of an input `ndarray`.</span>
-   <span class="signature">[`stride( x, dim )`][@hishprorg/error-quod/stride]</span><span class="delimiter">: </span><span class="description">return the stride along a specified dimension for a provided ndarray.</span>
-   <span class="signature">[`strides( x )`][@hishprorg/error-quod/strides]</span><span class="delimiter">: </span><span class="description">return the strides of a provided ndarray.</span>
-   <span class="signature">[`sub2ind( shape, ...subscripts[, options] )`][@hishprorg/error-quod/sub2ind]</span><span class="delimiter">: </span><span class="description">convert subscripts to a linear index.</span>
-   <span class="signature">[`ndarray2array( x )`][@hishprorg/error-quod/to-array]</span><span class="delimiter">: </span><span class="description">convert an ndarray to a generic array.</span>
-   <span class="signature">[`zerosLike( x[, options] )`][@hishprorg/error-quod/zeros-like]</span><span class="delimiter">: </span><span class="description">create a zero-filled ndarray having the same shape and data type as a provided ndarray.</span>
-   <span class="signature">[`zeros( shape[, options] )`][@hishprorg/error-quod/zeros]</span><span class="delimiter">: </span><span class="description">create a zero-filled ndarray having a specified shape and data type.</span>

</div>

<!-- </toc> -->

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better examples -->

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils/keys' );
var ns = require( '@hishprorg/error-quod' );

console.log( objectKeys( ns ) );
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

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

Copyright &copy; 2016-2024. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@hishprorg/error-quod.svg
[npm-url]: https://npmjs.org/package/@hishprorg/error-quod

[test-image]: https://github.com/hishprorg/error-quod/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/hishprorg/error-quod/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/hishprorg/error-quod/main.svg
[coverage-url]: https://codecov.io/github/hishprorg/error-quod?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/hishprorg/error-quod.svg
[dependencies-url]: https://david-dm.org/hishprorg/error-quod/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://app.gitter.im/#/room/#stdlib-js_stdlib:gitter.im

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/hishprorg/error-quod/tree/deno
[deno-readme]: https://github.com/hishprorg/error-quod/blob/deno/README.md
[umd-url]: https://github.com/hishprorg/error-quod/tree/umd
[umd-readme]: https://github.com/hishprorg/error-quod/blob/umd/README.md
[esm-url]: https://github.com/hishprorg/error-quod/tree/esm
[esm-readme]: https://github.com/hishprorg/error-quod/blob/esm/README.md
[branches-url]: https://github.com/hishprorg/error-quod/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/hishprorg/error-quod/main/LICENSE

<!-- <toc-links> -->

[@hishprorg/error-quod/at]: https://github.com/hishprorg/error-quod/tree/main/at

[@hishprorg/error-quod/broadcast-array]: https://github.com/hishprorg/error-quod/tree/main/broadcast-array

[@hishprorg/error-quod/broadcast-arrays]: https://github.com/hishprorg/error-quod/tree/main/broadcast-arrays

[@hishprorg/error-quod/casting-modes]: https://github.com/hishprorg/error-quod/tree/main/casting-modes

[@hishprorg/error-quod/data-buffer]: https://github.com/hishprorg/error-quod/tree/main/data-buffer

[@hishprorg/error-quod/defaults]: https://github.com/hishprorg/error-quod/tree/main/defaults

[@hishprorg/error-quod/dispatch]: https://github.com/hishprorg/error-quod/tree/main/dispatch

[@hishprorg/error-quod/dtype]: https://github.com/hishprorg/error-quod/tree/main/dtype

[@hishprorg/error-quod/dtypes]: https://github.com/hishprorg/error-quod/tree/main/dtypes

[@hishprorg/error-quod/empty-like]: https://github.com/hishprorg/error-quod/tree/main/empty-like

[@hishprorg/error-quod/empty]: https://github.com/hishprorg/error-quod/tree/main/empty

[@hishprorg/error-quod/fancy]: https://github.com/hishprorg/error-quod/tree/main/fancy

[@hishprorg/error-quod/flag]: https://github.com/hishprorg/error-quod/tree/main/flag

[@hishprorg/error-quod/flags]: https://github.com/hishprorg/error-quod/tree/main/flags

[@hishprorg/error-quod/from-scalar]: https://github.com/hishprorg/error-quod/tree/main/from-scalar

[@hishprorg/error-quod/ind2sub]: https://github.com/hishprorg/error-quod/tree/main/ind2sub

[@hishprorg/error-quod/index-modes]: https://github.com/hishprorg/error-quod/tree/main/index-modes

[@hishprorg/error-quod/maybe-broadcast-array]: https://github.com/hishprorg/error-quod/tree/main/maybe-broadcast-array

[@hishprorg/error-quod/maybe-broadcast-arrays]: https://github.com/hishprorg/error-quod/tree/main/maybe-broadcast-arrays

[@hishprorg/error-quod/min-dtype]: https://github.com/hishprorg/error-quod/tree/main/min-dtype

[@hishprorg/error-quod/mostly-safe-casts]: https://github.com/hishprorg/error-quod/tree/main/mostly-safe-casts

[@hishprorg/error-quod/ndims]: https://github.com/hishprorg/error-quod/tree/main/ndims

[@hishprorg/error-quod/next-dtype]: https://github.com/hishprorg/error-quod/tree/main/next-dtype

[@hishprorg/error-quod/numel-dimension]: https://github.com/hishprorg/error-quod/tree/main/numel-dimension

[@hishprorg/error-quod/numel]: https://github.com/hishprorg/error-quod/tree/main/numel

[@hishprorg/error-quod/offset]: https://github.com/hishprorg/error-quod/tree/main/offset

[@hishprorg/error-quod/order]: https://github.com/hishprorg/error-quod/tree/main/order

[@hishprorg/error-quod/orders]: https://github.com/hishprorg/error-quod/tree/main/orders

[@hishprorg/error-quod/output-dtype-policies]: https://github.com/hishprorg/error-quod/tree/main/output-dtype-policies

[@hishprorg/error-quod/promotion-rules]: https://github.com/hishprorg/error-quod/tree/main/promotion-rules

[@hishprorg/error-quod/safe-casts]: https://github.com/hishprorg/error-quod/tree/main/safe-casts

[@hishprorg/error-quod/same-kind-casts]: https://github.com/hishprorg/error-quod/tree/main/same-kind-casts

[@hishprorg/error-quod/shape]: https://github.com/hishprorg/error-quod/tree/main/shape

[@hishprorg/error-quod/slice-assign]: https://github.com/hishprorg/error-quod/tree/main/slice-assign

[@hishprorg/error-quod/slice-dimension-from]: https://github.com/hishprorg/error-quod/tree/main/slice-dimension-from

[@hishprorg/error-quod/slice-dimension-to]: https://github.com/hishprorg/error-quod/tree/main/slice-dimension-to

[@hishprorg/error-quod/slice-dimension]: https://github.com/hishprorg/error-quod/tree/main/slice-dimension

[@hishprorg/error-quod/slice-from]: https://github.com/hishprorg/error-quod/tree/main/slice-from

[@hishprorg/error-quod/slice-to]: https://github.com/hishprorg/error-quod/tree/main/slice-to

[@hishprorg/error-quod/slice]: https://github.com/hishprorg/error-quod/tree/main/slice

[@hishprorg/error-quod/stride]: https://github.com/hishprorg/error-quod/tree/main/stride

[@hishprorg/error-quod/strides]: https://github.com/hishprorg/error-quod/tree/main/strides

[@hishprorg/error-quod/sub2ind]: https://github.com/hishprorg/error-quod/tree/main/sub2ind

[@hishprorg/error-quod/to-array]: https://github.com/hishprorg/error-quod/tree/main/to-array

[@hishprorg/error-quod/zeros-like]: https://github.com/hishprorg/error-quod/tree/main/zeros-like

[@hishprorg/error-quod/zeros]: https://github.com/hishprorg/error-quod/tree/main/zeros

[@hishprorg/error-quod/base]: https://github.com/hishprorg/error-quod/tree/main/base

[@hishprorg/error-quod/iter]: https://github.com/hishprorg/error-quod/tree/main/iter

[@hishprorg/error-quod/array]: https://github.com/hishprorg/error-quod/tree/main/array

[@hishprorg/error-quod/ctor]: https://github.com/hishprorg/error-quod/tree/main/ctor

<!-- </toc-links> -->

</section>

<!-- /.links -->
