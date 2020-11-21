# promiseObject
wrapper class for promises in object form


```javascript

Promise.object = require('rajeshrenato/promiseObject')

let s = Promise.resolve(1);
let r = {
    k: Promise.resolve(2),
    j: Promise.resolve(3)
  };
let q = [Promise.resolve(4), Promise.resolve(5)]

let a = {s,r,q}

return Promise.object(a).then(res=>{
    console.log(res)
})
```
