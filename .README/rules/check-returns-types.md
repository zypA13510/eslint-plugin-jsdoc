### `check-returns-types`

Reports discrepancies between the claimed in JSDoc and actual type if both exist (code scan).

The following patterns are considered problems:

```js
/**
 * @returns {string}
 */
function quux () {
    return true;
}
```

The following patterns are not considered problems:

```js
/**
 * @returns {string}
 */
function quux () {
    return 'corge';
}
```