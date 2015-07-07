
The arrow function `() => {}` makes writing functions shorter.
And maintains `this` from the outer scope.
```js
function Kata() {
  this.name = 'kata';
  setTimeout(() => {
    alert(this.name); // => 'kata'
  }, 1);
}
new Kata();
```
