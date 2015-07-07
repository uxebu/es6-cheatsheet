Default values for function parameters
```js
function xhr(method = 'GET') {
  return method;
}
xhr();       // => 'GET
xhr('POST'); // => 'POST'
```
