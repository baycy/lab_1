```js
'use strict';

const array = [
    true, 'hello', 25, false, -14, 'JavaScript',
    3.14, true, 'world', 100, false, -7.5,
    'test', 42, true, 'random string', 0, false,
    18.9, 'word', -200, true, 56, 'another text'
];

const coll = {};

for (const item of array) {
    const type = typeof item;

    if (!(type in coll)) {
        coll[type] = 0
    }

    coll[type] += 1;
}

console.dir(coll);
```
