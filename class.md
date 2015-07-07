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
  set isAwesome(isAwesome) {}
  get isAwesome() {}
}
Kata.LEVEL = 'high'; // static property
```
