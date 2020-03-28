# ESM Matrix Functions

This library is a collection of matrix functions provided as an ESM module.

It is split into mutable and immutable pairs, the mutable ones provide better
performance as they avoid allocations and mutate the input matrix, the immutable
ones make for a cleaner, better composable code, but come at a performance cost.

## Status

This library is not seriously maintained.

## Installation

```js
import $name from 'https://tomashubelbauer.github.io/esm/matrix/$kind/$name.js';
```

Substitute `$name` for the function name you want to use and `$kind` for either
`mutable` or `immutable` depending on the variant you prefer to use.

## API

Not all functions have parity between the mutable and immutable variants yet.

### `immutable/add3x1To3x1.js`: `(matrix, otherMatrix)`

Returns a matrix which is the result of addition of two 3x3 matrices.

### `immutable/multiply3x3By3x1To3x1.js`: `(matrix, otherMatrix)`

Returns a matrix which is the result of multiplication of a 3x3 by 3x1 matrix.

### `immutable/multiply3x3By3x3.js`: `(matrix, otherMatrix)`

Returns a matrix which is the result of multiplication of two 3x3 matrices.

### `immutable/subtract3x1From3x1.js`: `(matrix, otherMatrix)`

Returns a matrix which is the result of subtraction of two 3x1 matrices.

### `immutable/subtract3x3From3x3.js`: `(matrix, otherMatrix)`

Returns a matrix which is the result of subtraction of two 3x3 matrices.

## To-Do

### Finalize the mutable versions

### Add more invariant checks

### Avoid running the tests on each `import`, pull them out for running ad-hoc
