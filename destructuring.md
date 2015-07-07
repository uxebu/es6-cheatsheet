Destructuring allows for more flexible and compact assignments
```js
let x = 'why', y = 'ex';
[y, x] = [x, y];
// x = 'ex', y = 'why'

const pages = [{title: 'Home'}, {title: 'Footer'}];
const [{title}, {title: secondTitle}] = pages;
// title = 'Home', secondTitle = 'Footer'
```
