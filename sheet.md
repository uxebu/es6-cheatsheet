ECMAScript 6 has classes built-in.
It is a shorter notation for the well-known prototype approach.

```js
class Kata {
  constructor(name) {
    // initialize instance properties in the constructor
    this.name = name;
  }
  // instance method
  addTest() {}
  // static method
  static create(name) {}
  // getter+setter
  set isAwesome(isAweseome) {}
  get isAwesome() {}
}
Kata.LEVEL = 'high'; // static property
```

The arrow function `() => {}` makes writing functions shorter.
And maintains `this` from the outer scope.
```js
function Kata() {
  this.name = 'kata';
  setTimeout(() => {
    alert(this.kata); // => 'kata'
  }, 1);
}
new Kata();
```

Default values for function parameters
```js
function xhr(method = 'GET') {
  return method;
}
xhr();       // => 'GET
xhr('POST'); // => 'POST'
```

Rest operator can replace `arguments`
```js
function combine(...numbers) {
  return numbers;
}
combine(1, 2, 3, 4); // => [1, 2, 3, 4]
```

Spread operator expands an array
```js
x = [1, ...[2, 3, 4], 5]; // => [1,2,3,4,5]
```

Destructuring allows for more flexible and compact assignments
```js
let x = 'why', y = 'ex';
[y, x] = [x, y];
// x = 'ex', y = 'why'

const pages = [{title: 'Home'}, {title: 'Footer'}];
const [{title}, {title: secondTitle}] = pages;
// title = 'Home', secondTitle = 'Footer'
```
